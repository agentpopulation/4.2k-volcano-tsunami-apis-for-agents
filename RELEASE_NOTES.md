## Volcano and tsunami API endpoints, snapshot 15 Nov 2026

- 4,256 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 686 services · 46 country codes · 2,347 keyless JSON rows

### Download

- `Volcano_Tsunami_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 4,256 rows, 210.5 kB gzipped (1.3 MB as CSV), SHA-256 `5cabe2479d1de915aea41878430dd10f0f1334e94075a21b5a80437ff85c0b96`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Volcano_Tsunami_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Volcano_Tsunami_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 1,611 · Wrap one ArcGIS layer as a get_hazard_zone tool: pass a point as `geometry=lon,lat&geometryType=esriGeometryPoint&spatialRel=esriSpatialRelIntersects` and return the tsunami evacuation, lava-flow or lahar zone it falls in, with a timeout; CKAN, Socrata and OpenDataSoft rows return the zone table without a point filter.
- 📱 App features: 402 · Draw evacuation zones, assembly points and hazard areas on a map card; show the zone a user stands in and the nearest safe area, with the layer date.
- 🧠 Grounding and data pipelines: 226 · Load eruption and tsunami event lists, station lists and model-grid descriptions on a schedule into your own store, so answers about past events and exposure cite a dated source.
- 🧪 Evals and testing: 4,256 · Run your hazard tool against a fixed set of URLs across hosts; check that zone names, volcano names, dates or wave heights parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 5,280 endpoints from 903 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 4,256 endpoints from 686 services, 1,024 fewer endpoints than first published under this snapshot (5,280 from 903 services), tested 10–15 Nov 2026 (IST).
- Left out: 69 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 609 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 4 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 61 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 2 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 1 ArcGIS layer that is a record about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 6 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 17 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 341 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 88 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 653 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 15 rows that repeat an address already in the pack.
- Left out: 14 copies of population-distribution and shelter-access layers, many with initials or a person's name added to the title.
- Overlap: 45 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 64 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 157 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 33 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 122 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 2 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 61 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 26 of these URLs are also in 22k-maritime-apis-for-agents.
- Overlap: 5 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 2,311 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 79 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 3,984 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 6 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 1 of these URLs is also in 10k-parking-apis-for-agents.
- Overlap: 346 of these URLs are also in 7.8k-earthquake-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Volcano and tsunami API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
