---
id: OBS-2
title: Real Wages in Spain Chart
status: To-do
labels: Viz
---

Check real wages since 2000s
Has to be comparative with other countries and average or median
Probably line chart
Single source (ie, Eurostat or OECD would be best) TBD

## Source Research

Identify high-confidence free sources for a comparative real-wages chart for Spain since the 2000s, prioritizing official data portals with open access and API-backed downloads.

### Links

https://economy-finance.ec.europa.eu/economic-research-and-databases/economic-databases/ameco-database_en
https://economy-finance.ec.europa.eu/economic-research-and-databases/economic-databases/ameco-database/download-annual-data-set-macro-economic-database-ameco_en
https://webgate.ec.europa.eu/ecfin/redisstat/databrowser/explore/all/AMECO?display=card&lang=en&sort=category
https://data.oecd.org/index.htm
https://www.oecd.org/en/data/datasets/oecd-DE.html
https://data-explorer.oecd.org/
https://www.oecd.org/en/data/indicators/average-annual-wages.html
https://www.oecd.org/en/data/indicators/inflation-cpi.html
https://ec.europa.eu/eurostat/web/hicp/information-data
https://ec.europa.eu/eurostat/web/hicp/visualisations
https://ec.europa.eu/eurostat/cache/metadata/en/nama_10_fte_esms.htm
https://ec.europa.eu/eurostat/web/labour-market/information-data/earnings
https://ec.europa.eu/eurostat/web/labour-market/information-data/labour-costs

### Notes

- AMECO is the strongest single-source candidate here: it explicitly includes `real compensation per employee`, free bulk downloads, and a new interface with API access.
- OECD is also viable: its Data Explorer is explicit about API access, and the wage/inflation indicators are easy to combine if a direct real-wage series is not used.
- Eurostat is a good EU-harmonised fallback: `nama_10_fte` gives nominal salary, while HICP provides the deflator needed to build real wages.
- I excluded non-official sources and anything that looked like it would require scraping or opaque wrangling.
