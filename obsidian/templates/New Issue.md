<%*
const backlogFolder = "backlog";
const disallowed = /[:\[\]#/\\!]/g;

const files = app.vault.getFiles().filter(f =>
  f.path.startsWith(backlogFolder + "/") && /^OBS-(\d+)/.test(f.name)
);

let maxId = 0;
for (const file of files) {
  const match = file.name.match(/^OBS-(\d+)/);
  if (match) maxId = Math.max(maxId, parseInt(match[1], 10));
}

const nextId = maxId + 1;

const rawTitle = await tp.system.prompt("Issue title");
if (!rawTitle) {
  new Notice("Aborted: no title provided.");
  return;
}

const title = rawTitle.replace(disallowed, "").trim();
if (!title) {
  new Notice("Aborted: title contains only disallowed characters.");
  return;
}

await tp.file.move(`${backlogFolder}/OBS-${nextId} ${title}`);
_%>
---
id: OBS-<% nextId %>
title: <% title %>
status: Backlog
labels:
---
