# Reading Alaska's STIP

A plain-language guide to the Alaska Department of Transportation & Public Facilities (DOT&PF) draft **2027–2030 Statewide Transportation Improvement Program (STIP)**, written for Ketchikan.

The STIP is the four-year list of road, bridge, ferry, and trail projects DOT&PF expects to pay for with federal money. A project that is not in the STIP cannot use federal highway or transit funds. Being listed means DOT&PF expects to move the project forward. It is a plan, not a construction schedule and not a guarantee that the money will arrive on time.

This repository is the whole site: one file, [`index.html`](index.html). There is no build step, no package manager, and no server code. Open that file in a browser and the guide is the page.

This is an independent guide, built in Ketchikan by [Mitchel Turner Dev](https://mitchelturner.dev). It is not a DOT&PF publication. The draft can change before federal approval, so check [dot.alaska.gov/stip](https://dot.alaska.gov/stip) before citing a figure.

Public comments on this draft are due **October 29, 2026, at 5 p.m. Alaska time**.

## Open the guide

The page is static HTML. Any of these works:

- Double-click `index.html`, or open it from your browser’s File menu.
- From this folder, serve it locally:

  ```bash
  python3 -m http.server 8000
  ```

  Then visit `http://localhost:8000`.

The only outside request is the typefaces (Overpass, Overpass Mono, and Source Serif 4) from Google Fonts. If that request fails, the page falls back to Helvetica, Georgia, and a system monospace font. The Saxman concept drawing is embedded in the file, so it does not need a network.

The “Copy address” button next to `dot.stip@alaska.gov` uses the clipboard API. On a `file://` page that API is often blocked, and the button then selects the address so it can be copied with Ctrl+C or Command+C. Serving the file over `localhost` avoids that.

## What the page covers

A sticky section nav jumps between eight parts. On a narrow screen the same list is a “Jump to” menu. The nav highlights the section in view.

| Section | What it shows |
| --- | --- |
| Overview | What the STIP is, about **$191.7 million** for the Ketchikan projects in this draft, **$5.63 billion** statewide, and a live countdown to the comment deadline. |
| Map | The same projects drawn north to south along Tongass, from Ward Cove to Herring Cove. Schematic, not to scale. |
| Bridges | Federal 0–9 ratings for the five Ketchikan bridges named in the plan. A score of 4 or lower is “Poor.” That means the bridge needs significant repair or replacement. It does not mean the bridge is closed. |
| Projects | Every Ketchikan line in the draft, with dollars by federal fiscal year and by phase. Desktop is a sideways-scrolling grid. Phones get one card per project. “What is it?” opens the description. |
| Timeline | Construction money only, by the year it is funded. Outlined blocks are on Tongass itself. A short history of the airport ferry berths sits under the calendar. |
| Questions | Five places where the draft’s own numbers raise a question worth putting in a comment. |
| Comment | Email, the online form, the Juneau mailing address, the phone number, two QR codes, and the dates from draft release through the federal-approval target. |
| Background | What the STIP is and is not, the phase codes, a short glossary, and statewide charts for purpose, region, and year. |

The Ketchikan headline is calculated from the project list when the page loads. The statewide $5.63 billion figure is written into the page from Volume 3 of the draft.

### How the money is labeled

Years are **federal fiscal years**. FY27 runs from October 1, 2026, through September 30, 2027. “Construction funded FY28” means the contract money is set aside between October 2027 and September 2028, so work would likely happen in the 2028 season or later, and it can slip.

Each dollar in the project grid is tagged with a phase, matching the chips on the page:

| Code | Name on the page | Meaning |
| --- | --- | --- |
| Phase 2 | Design | Engineering and environmental review. This is when public comment changes a project the most. |
| Phase 3 | Buying land | Surveying, appraising, and buying property the project needs. |
| Phase 4 | Construction | Building, rebuilding, or repairing the road, bridge, or terminal. |
| Phase 7 | Utilities | Moving power, water, sewer, and phone lines. |
| ACC | Paying back earlier work | The state already started the job and this line is the later federal reimbursement. |
| Unlabeled | Phase not listed | The Revilla airport-ferry amount comes from the Volume 3 tables and has no phase on a project page. |

Totals on the page cover only these four years. Several projects also have money spent before 2027 or planned after 2030. Those amounts are described in the text, and they are not inside the $191.7 million.

Across the 14 funded lines (11 stops on the map; the airport berths and the viaduct corridor are split into stages):

- **$191.7 million** in the four-year window
- **$158.1 million** of that is construction (Phase 4)
- **$11.8 million** pays back work already underway or already built

### Bridges in the plan

Ratings and build years come from Volume 2 of the draft. The scale is the Federal Highway Administration’s National Bridge Inventory.

| Bridge | Built | Rating | Map stop |
| --- | --- | --- | --- |
| Water Street Viaduct #797 | 1955 | Poor, 4 / 9 | 6 |
| Hoadley Creek Bridge #725 | 1957 | Poor, 4 / 9 | 4 |
| Tongass Avenue Viaduct #997 | 1956 | Fair, 6 / 9 | 6 |
| Ward Creek Bridge #747 | 1975 | Fair, 6 / 9 | 1 |
| Herring Cove Bridge #253 | 2022 | Good, 9 / 9 | 11 |

Ward Creek’s project page describes the bridge’s condition as poor and says the north abutment is settling, even though the inventory score on the page is 6. The guide prints both.

## Ketchikan projects in this draft

Dollars are millions, federal fiscal years 2027–2030, from each project’s page in Volume 2 unless noted. Map numbers match the strip map and the project grid.

| Map | STIP | Project | Where | Four-year total | What the draft funds |
| --- | --- | --- | --- | --- | --- |
| 1 | 31469 | Ward Creek Bridge replacement | Bridge #747, North Tongass Highway, milepost 11 | $36.2M | Design, construction, and utilities in FY27. Built in 1975. The project page expects construction from late fall 2026 through the 2028 season. Page V2-175. |
| 2 | 30834 | Gravina airport ferry berth refurbishment | Gravina Island airport ferry terminal | $5.6M | Construction in FY27: berth, loading ramp, terminal, landside, electrical, and utility work. Page V2-76. |
| 2 | 30831 | Revilla airport ferry berth refurbishment | Revilla side of the airport ferry | $1.4M | FY27. No Volume 2 page; the amount is from the Volume 3 funding tables, and no phase is listed. |
| 3 | 34750 | Ketchikan Shipyard receiving slab | State-owned shipyard | $10.1M | Design in FY27, construction in FY28. Repairs the slab, foundations, and rail used to maintain the state ferry fleet. Page V2-91. |
| 4 | 31718 | Hoadley Creek Bridge replacement | Bridge #725, Tongass Avenue | $5.9M | Land in FY27, construction in FY28. Built in 1957 and rated Poor. Page V2-155. |
| 5 | 27766 | Tongass resurfacing | Hoadley Creek to Elliott Street | $11.5M | Advance-construction payback in FY29. About $25 million was obligated before FY27. This line reimburses the state. Page V2-258. |
| 6 | 31719 | Viaduct corridor, parent and final stage | Tongass Avenue and Water Street viaducts and the tunnel | $11.9M | Design in FY27, land and utilities in FY28, construction in FY29. A further $25 million stage is scheduled for 2031 or later. Page V2-152. |
| 6 | 34457 | Viaduct corridor, Stage 1 | Same corridor, first early-work package | $5.8M | Construction in FY28. Page V2-153. |
| 6 | 34785 | Water Street Viaduct #797 replacement | Worn-out sections of viaduct #797 | $10.3M | Design only, in FY27. No construction money in this STIP. Page V2-176. |
| 7 | 34248 | Spruce Mill Promenade | Along the Lumberjack Show pavilion | $6.0M | A small land line in FY27 and construction in FY28. Timber deck, railing, and lighting, from the 2023 Transportation Alternatives round. Page V2-157. |
| 8 | 21114 | Deermount to Saxman reconstruction | Deermount Street to Saxman | $42.8M | Design in FY27, construction in FY29. Sidewalks, bike facilities, parking, drainage, and guardrail. The project page lists pavement condition as “Not Available.” About $15 million was spent before this draft. Page V2-154. |
| 9 | 35275 | South Tongass Ferry Terminal (new) | Saxman Seaport | $25.8M | Design in FY27 and FY28, construction in FY29. See below. Page V2-151. |
| 10 | 23455 | Saxman to Surf Street reconstruction | Saxman to Surf Street | $18.1M | Construction and a small utilities line in FY28. Page V2-156. |
| 11 | 28810 | Herring Cove Bridge | Bridge #253 | $0.3M | Payback in FY30. The bridge was replaced in 2022 and is rated Good. Page V2-255. |

DOT&PF’s “South Tongass Highway” starts in the West End, near Hoadley Creek at milepost 0.2. Some projects with “South Tongass” in the name are north of downtown.

### The new ferry terminal at Saxman Seaport

STIP **35275** is the longest section on the page, because the draft’s price and the last published design do not line up cleanly.

The draft sets aside **$25.8 million**, mostly from a federal rural ferry grant, to move the M/V Lituya’s Ketchikan landing from the West End terminal to Saxman Seaport. DOT&PF ties the move to the ferry system’s 2045 long-range plan (Volume 6, page 187). Saxman and the Metlakatla Indian Community asked for a terminal in a 1997 joint resolution.

The page includes PND Engineers’ Concept 3 drawing from the July 31, 2023 *South Tongass Highway Ferry Terminal Concept Scoping Report* (Southeast Conference; PDF page 16, drawing sheet 6 of 7). The drawing shows the Lituya inside the existing breakwater, a 140-foot transfer bridge, a 24-by-36-foot terminal building, and parking shared with Three Bears. The preferred scheme, Concept 3A, keeps that layout and changes the berth from fixed pilings to a floating berth anchored to bedrock.

Figures the page puts next to the drawing:

- The crossing to Annette Bay is about **6.7 miles and 45 minutes** from the West End terminal, and about **3.0 miles and 15 minutes** from Saxman Seaport.
- Early 2023 Lituya service was 2 round trips a day, 5 days a week. A 2010 DOT&PF site study said a Saxman terminal could allow 7 round trips in a 10-hour day.
- The January 2023 engineers’ estimate for the berth and parking under Concept 3 was **$16.2 million**. The 2023 report has no cost estimate for the floating-berth Concept 3A. The draft STIP line is **$25.8 million**.
- Concept 3A also describes three 250-foot vehicle lanes, about 130 parking spaces, 290 feet of small-boat moorage, and space reserved for battery storage for future electric ferries. The site could be a backup berth for the Inter-Island Ferry.
- The land would be leased from the City of Saxman, so it stays with the city. Saxman voters rejected a sale of 7.57 acres to the state in 2007. Much of the uplands is leased to Three Bears.
- January 2023 hearings in Saxman (about 45 people) and Metlakatla (about 60) mostly supported the shorter run. Concerns on the record include the trip into Ketchikan without a car, cab cost, a small waiting room, sailing times, fares, and Pennock Island residents who use the Saxman floats.
- An earlier design project, STIP 33972, put $500,000 on the books in 2022. Southeast Conference says the 2024–2027 STIP funded it toward 35% design. That number does not appear in this draft, and project 35275 shows $0 spent before 2027.

The comment prompt on the page asks whether $25.8 million is based on the floating-berth design, whether sailings would actually increase, whether a shuttle into Ketchikan is funded, and what happened to the earlier design work.

## Questions the page suggests asking

Each one is tied to a project number so a comment can name it.

1. **Viaducts (31719, 34785).** Bridge #797 was built in 1955 and is rated Poor. The funded work is spot repair, plus a new Jim Creek culvert, meant to hold the viaducts until they are replaced. A $25 million repair stage sits in 2031 or later, and the replacement project has design money only. How long are the spot repairs expected to last, and when will replacement be funded?
2. **Tongass closures (map stops 4, 6, and 8–10).** Hoadley Creek, the first viaduct stage, and Saxman to Surf Street are funded for construction in FY28. FY29 adds Deermount to Saxman ($42.5 million of construction), the final viaduct stage, and the new Saxman terminal. Is there a plan to stagger the jobs, and will major closures avoid cruise season?
3. **Deermount to Saxman (21114).** About $15 million is already spent and $42.5 million is set for construction, while the project page lists pavement condition as “Not Available.” What data supports the rebuild, and will the design consider narrower lanes and wider sidewalks? A chart on the page, from Tefft’s 2011 AAA Foundation study, shows how pedestrian risk of death rises with impact speed.
4. **Saxman terminal (35275).** The questions in the section above.
5. **Statewide fiscal constraint (Volume 3, pages 3 and 5).** FY27 through FY29 are over-scheduled by a combined $401 million, with room in FY30. The four-year plan is about $130 million over what DOT&PF expects to have. The Southcoast Region, which includes Ketchikan, is about $7 of every $100 of new spending commitments, and the ferry system is about $13. If money runs short, which Ketchikan projects would slip first?

## How to comment

The comment period closes **October 29, 2026, at 5 p.m. Alaska time**. The countdown on the page treats that instant as 01:00 UTC on October 30, 2026 (AKDT, UTC−8). After the deadline the countdown reads “Closed.” Comments sent later are still accepted for future planning.

| How | Where |
| --- | --- |
| Email | [dot.stip@alaska.gov](mailto:dot.stip@alaska.gov) |
| Online form | [dot.alaska.gov/stip](https://dot.alaska.gov/stip) |
| Mail, must arrive by the deadline | Alaska DOT&PF, Division of Statewide Planning, ATTN: STIP, P.O. Box 112500, Juneau, AK 99811-2500 |
| Questions or help | 907-465-4070. Alaska Relay: dial 711. |

The page’s two QR codes point at the comment form and at this guide.

DOT&PF says a useful comment names the project and its STIP number, says what should change (scope, schedule, funding, or design), and explains why in a sentence or two. One comment per project is easier for the department to track. DOT&PF says it will publish comments and its responses in Volume 5 of the final STIP.

Dates printed on the page, from the draft and from reporting on the September 2026 Senate Transportation Committee hearing:

- **September 14, 2026.** Draft released.
- **October 29, 2026, 5 p.m.** Comment period closes.
- **Early December 2026.** A new governor takes office.
- **Mid-December 2026.** DOT&PF’s target for federal approval.

After the deadline, DOT&PF reviews comments, revises the draft, and sends the final STIP to federal highway and transit officials (draft Volume 1, page 50).

## How the page is built

`index.html` is self-contained. Roughly the first 330 lines are CSS, the middle is the article, and the last 200 lines are one script. The file is about 520 KB because the Saxman drawing is a progressive JPEG stored as a `data:` URL (1,700 × 963 pixels, about 327 KB of image data).

The script builds four parts of the page from data at the top of that script:

- `P`, the Ketchikan project list. Each record has a map number (`m`), a zone (`z`), a STIP id, a name, a place, a Volume 2 page, a kind (`road`, `ferry`, `walk`, or `pb` for payback), a short description, and `fy`: an object whose keys are fiscal years and whose values are `[phase, millions]` pairs. A corridor that has stages uses `rows` instead of a single `fy`.
- `B`, the five bridge ratings.
- The construction calendar, which reads Phase 4 (and the unlabeled Revilla amount) back out of `P`. Projects in `onRoad` (`21114`, `23455`, `31719`, `34457`, `31718`) are drawn as the outlined “on Tongass” blocks.
- The statewide bar charts, the year-by-year fiscal-constraint table, and the 100-cell waffle. Those numbers are separate arrays, copied from Volume 3, and they do not come from `P`.

The hero’s Ketchikan total, the three summary figures above the project grid, the strip map, the desktop grid, and the phone cards are all rendered from `P`. Change a number in `P` and those pieces follow. The question essays, the Saxman card, the airport-ferry timeline, the glossary, and the footer do not. They are ordinary HTML and have to be edited on their own.

Other behavior in the script:

- The countdown and the section highlighter run once on load. The highlighter uses `IntersectionObserver` where the browser has it.
- The pedestrian-risk chart is drawn as inline SVG from five points in the Tefft study: 10% at 23 mph, 25% at 32, 50% at 42, 75% at 50, and 90% at 58.
- Colors are fixed in CSS custom properties: highway-sign green, work-zone orange for construction, marine blue for ferries. The page is light-only on purpose (`color-scheme: light`).
- Desktop and phone layouts are switched with `.d-only` and `.m-only`. Both are in the HTML; CSS shows one of them.

### Changing a project

1. Find the record in the `P` array near the bottom of `index.html`.
2. Edit the name, the page citation, the description, or the `fy` amounts. Amounts are millions of dollars. Phases are `P2`, `P3`, `P4`, `P7`, `ACC`, or `?` when Volume 3 lists money and no phase.
3. Reload the page. The map dot, the grid, the phone card, the hero total, and the construction calendar recompute.
4. If the prose in “Questions the draft raises” quotes that project, update that HTML too. It will not change by itself.
5. If you add or remove a bridge, edit the `B` array. Ratings of 4 and below render as Poor, 5–6 as Fair, and 7–9 as Good.
6. To replace the Saxman drawing, swap the `src` of the image inside `<figure class="sx-fig">`. A normal image file also works if you would rather not embed it. Keep the caption’s citation with the figure.

Statewide charts live in the `bars(...)` calls and the `yrs` array further down the script. Those are Volume 3 figures for the whole state, not sums of the Ketchikan list.

## Sources

The draft cited throughout is Alaska DOT&PF, *Proposed FFY2027–2030 Statewide Transportation Improvement Program, Public Comment Draft*, September 14, 2026.

- Volume 1: V1-12 (what the STIP is), V1-26, V1-33, V1-49, V1-50 (approval steps).
- Volume 2 project pages: V2-76, V2-91, V2-151 through V2-157, V2-175, V2-176, V2-255, V2-258.
- Volume 3: V3-3 through V3-10, including the funding schedules and the regional split.
- Volume 6 selection register, including V6-187 for the ferry system’s long-range plan.

Project and background pages linked from the footer:

- [Ketchikan Tongass Avenue & Water Street Viaducts](https://dot.alaska.gov/sereg/projects/water-street-viaducts/) (SFHWY00196). Questions: contact@ketchikanviaducts.com. DOT&PF says it answers within five business days.
- [Ward Creek Bridge](https://dot.alaska.gov/sereg/projects/ward-creek-bridge/) (SFHWY00160).
- [Ketchikan Airport Ferry Facility Improvements](https://dot.alaska.gov/sereg/projects/ktn_revilla_upland_berth/index.shtml) and its [project development](https://dot.alaska.gov/sereg/projects/ktn_revilla_upland_berth/project_development.shtml) page. The 2020 bid notice is [Alaska Online Public Notices, id 197324](https://aws.state.ak.us/OnlinePublicNotices/Notices/View.aspx?id=197324).
- [AMHS Ketchikan terminal](https://dot.alaska.gov/amhs/comm/ketchikan.shtml).
- Tefft, B.C., [*Impact Speed and a Pedestrian’s Risk of Severe Injury or Death*](https://aaafoundation.org/impact-speed-pedestrians-risk-severe-injury-death/), AAA Foundation for Traffic Safety, 2011.
- Bridge locations and traffic: [Hoadley Creek Bridge record](https://bridgelookup.com/bridge/16522) (National Bridge Inventory data). Rating scale via [BridgeCondition.com](https://bridgecondition.com/condition/poor).
- Route layout: [Alaska Route 7](https://en.wikipedia.org/wiki/Alaska_Route_7) on Wikipedia.
- Saxman terminal: PND Engineers, [*South Tongass Highway Ferry Terminal Concept Scoping Report*](https://seconference.org/program/south-tongass-highway-ferry-terminal-saxman-seaport/) (Southeast Conference, July 2023); [KRBD, January 2023](https://www.krbd.org/2023/01/27/public-weighs-in-on-new-lituya-terminal-at-hearings-in-saxman-metlakatla/); [City of Saxman Resolution 04.2024.04](https://mccmeetingspublic.blob.core.usgovcloudapi.net/saxmanak-meet-35d2c21a9e1f4e8693c5c4b6c90024b5/ITEM-Attachment-001-0957aed0ec884d9ebcab32ba35c83185.pdf); [Juneau Empire, August 2026](https://www.juneauempire.com/2026/08/29/410m-in-federal-funds-target-smooth-sailings-for-southeast-alaska-ferry-service/).
- Lituya service and the terminal background: [KTOO, January 2023](https://www.ktoo.org/2023/01/19/alaskas-ferry-system-is-considering-a-new-terminal-in-saxman/).
- Approval timing: [Alaska Beacon](https://www.newsfromthestates.com/node/429705), reporting on the September 2026 Senate Transportation Committee hearing.

## Words used on the page

| Term | Meaning in this draft |
| --- | --- |
| Federal fiscal year (FY) | October 1 through September 30. FY27 is October 2026 through September 2027. |
| Advance construction (AC) | The state starts a project with its own money and is reimbursed with federal funds later. |
| AC conversion (ACC) | That later reimbursement. An ACC line usually pays for work already done or already started. |
| Parent and child stages | A large project split into pieces. The “Project Lifecycle Obligations” table on a Volume 2 page is the full cost, including years outside this STIP. |
| NHPP | National Highway Performance Program, the federal fund for major highways such as Tongass. |
| State match | The state’s share of a federally funded project. For the Ketchikan projects in this draft, that share runs from about 9 to 20 percent. |
| Fiscal constraint | The rule that the plan cannot count on more money than DOT&PF can reasonably expect. The draft’s first three years are over that line. |
| STIP number | The project’s identifier inside the draft, such as 21114 for Deermount to Saxman. Comment letters should use it. |

Airports are planned in a separate process and are not in the STIP. The airport *ferry* berths are in this draft because they are marine projects, not airport projects.
