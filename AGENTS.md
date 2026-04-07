Observa is a platform that aggregates data about the Spanish economy and society.

It consists of:
- A website that offers:
	- Interactive visualizations and simulations
	- Reports
- A data pipeline that allows:
	- Rapid exploration for the analyst
	- Automated and reliable updates for the website

It is inspired by sites like Our World in Data, but with a singular focus on Spain. It seeks to aggregate data from a disjoint data landscape, create novel analysis, and also offer comparison benchmarks with other countries.

The core of the website and pipeline will be open source. That will include not only code, but also organizational aspects such as research, processes, and architecture. This repo will therefore contain a maximum of publishable information about the company - pretty much everything except credentials, sensitive information or drafts not worth committing.

A central theme of the project is Artificial Intelligence, in at least these aspects:

1. As means to produce code
2. As means to produce non-technical info (research, docs on process and architecture, etc)
3. As means of interaction for end-users (ie, being able to query the data with AI)
4. In that it's meant to help track the impact of AI in the economy

To emphasize: we will publish not only the code and website, but also the methods employed to achieve the results. We hope the project may serve as inspiration for people trying to build similar projects or even new enterprises and non-profits with new ways of working.

We ambition to have stellar UX and DX and adopt a radical innovation posture, in particular in the adoption of AI technologies and processes.

We *may* in the future add sources of revenue such as a premium API for enterprises or consulting services, but this is not a concern right now. The project may as well fully free and open-source forever.

For now, the repo's official language is English. That includes code as well as non-code artifacts. The default public language (for the website, chart legends, social media communications, etc.) is Spanish. This decision is still under review.

Right now, we are working with the following tooling:

**Obsidian** as a vault matching the root for superior markdown editing and usage of Bases. We will favor the Obsidian (and Notion) model of "documents-as-records", with lists (in our case, Bases) sporadically laid on top. 

**Claude Cowork** as the main interface for non-code operations, such as research.

**Codex CLI**  as the main driver for code generation.

**Jetbrains IDEs** as the main driver for code editing.

Obsidian is currently set up so that all images are stored in `doc-media` folders adjacent to the data sources. Bear that in mind if you manipulate docs.



