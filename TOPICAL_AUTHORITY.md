# Topical Authority — saung.id

## Role and boundary

`saung.id` should become an Indonesian reference for planning, designing, procuring, building, using, inspecting, and repairing saung or gazebo as small outdoor structures. Its audience includes homeowners, hospitality and restaurant operators, landscape designers, architects, contractors, facility managers, community or worship administrators, and buyers comparing a vendor's proposal.

The editorial boundary is the structure and its immediate site interface. Full houses, generic landscape design, standalone furniture, and material industries belong only where they change a saung decision. Commercial landing pages may sell design, fabrication, installation, or repair, but the knowledge articles remain neutral and evidence-led.

This is a planning document, not structural design, a bill of quantities, a permit opinion, or permission for DIY work. Span tables, member sizes, anchorage, foundations, fire performance, chemical treatment, electrical work, and work-at-height procedures must be project-specific and reviewed by competent professionals. Applicable national standards, local rules, product registrations, and manufacturer instructions must be rechecked at publication and project time.

## Evidence audited

Repository audit performed on 2026-07-23 against the clean `main` branch:

| Evidence source | Observed count or finding | Editorial implication |
|---|---:|---|
| `sitemap_index.xml` | 17 child sitemaps | The index combines core posts/pages with five mass-generated commercial families. |
| All indexed child sitemaps | 2,961 unique URLs | URL volume is not evidence of topical depth. |
| `post-sitemap.xml` | 21 URLs | Includes four gazebo material pages, material/design/application pages, several timber-house pages, and `/hello-world.html`. |
| `page-sitemap.xml` | 6 URLs | Home, about, contact, projects, services, and a sample page. |
| Material/location families | 2,934 URLs | Bamboo 489, steel 489, concrete 489, timber 978, and timber-house 489. |
| Timber location family | 978 URLs | It contains 489 normal routes and 489 `-copy` variants, an explicit duplicate-risk group. |
| On-disk HTML export | 7,532 files | Includes site pages plus WordPress administrative/API export artifacts, not 7,532 useful editorial pages. |
| On-disk `/wp-json/` artifacts | 2,964 HTML files | Technical export residue should not be indexed as content. |
| Unsitemapped steel folders | 391 additional location directories | Canonical and deployment behavior need crawl-level verification before removal. |
| Feed/archive residue | author, category, comments, and feed routes | Thin archives and feeds need an indexability policy. |
| Core design coverage | modern, classic Javanese, stilt, European, traditional, application, and material pages | Useful visual evidence exists, but house and saung intents are mixed and technical boundaries are weak. |

Primary source gates identified for later article research:

- [PP 16/2021 on implementation of building regulations](https://peraturan.bpk.go.id/Details/161846/pp-no-16-tahun-) is recorded as in force by the BPK regulation database; project applicability and local PBG/SLF requirements still need location-specific checking.
- [Permen PUPR 10/2021 on construction safety management](https://jdih.pu.go.id/detail-dokumen/PermenPUPR-nomor-10-tahun-2021-Pedoman-Sistem-Manajemen-Keselamatan-Konstruksi) is an official construction-safety source.
- BSN's official catalog records [SNI 7973:2013 for timber construction](https://pesta.bsn.go.id/produk/index/354), [SNI 1726:2019 for seismic design](https://pesta.bsn.go.id/produk/index?key=1726), and [SNI 1727:2020 for minimum design loads](https://pesta.bsn.go.id/produk/detail/12927-sni17272020). The licensed standard text, status, scope, and applicable edition must be checked before technical publication.
- The BPK regulation database records [Permen PU 26/PRT/M/2008 on fire protection for buildings and environments](https://peraturan.bpk.go.id/Details/104475/permen-pupr-no-) as in force. Occupancy and local fire-authority requirements still control project application.
- Pest-control or termiticide guidance must verify current registration and label directions. [PP 7/2026](https://jdih.pertanian.go.id/peraturan/pp-7-2026) covers pesticide registration, quality, labeling, and use; the current product registry and implementing rules must be checked at publication.

## Existing coverage and risks

| Existing URL/pattern | Observed role/problem | Decision | Destination/owner | Verification needed |
|---|---|---|---|---|
| `/` | Broad sales home page | keep | Commercial home route | Confirm current offer, service area, contact tracking, and canonical. |
| `/saung.html` | Broad saung overview mixed with sales | expand | Central saung hub, linked to `TOPIC:SAU-01` and `TOPIC:SAU-02` | Check Search Console history before changing title or URL. |
| `/saung-gazebo-bambu.html` | Material/service hybrid | expand | Bamboo decision hub, `TOPIC:SAU-09` | Separate neutral material education from vendor claims. |
| `/saung-gazebo-kayu.html` | Material/service hybrid | expand | Timber decision hub, `TOPIC:SAU-10` | Preserve useful photos and validate species claims. |
| `/saung-gazebo-besi.html` | Material/service hybrid | expand | Metal/hybrid decision hub, `TOPIC:SAU-11` | Replace unverified durability claims with coating/system evidence. |
| `/saung-gazebo-beton.html` | Material/service hybrid | expand | Concrete/hybrid decision hub, `TOPIC:SAU-11` | Clarify precast versus cast-in-place and structural-review boundary. |
| `/material.html` | Broad material summary overlapping four routes | merge | Material chooser, `SAU-09-A01`, `SAU-10-A01`, and `SAU-11-A01` | Choose one informational canonical after query/history review. |
| `/material-bambu.html` | Bamboo page overlapping `/saung-gazebo-bambu.html` | merge | Preserve stronger route; support `TOPIC:SAU-09` | Compare links, impressions, content, and canonical tags. |
| `/material-kayu-jati.html` and `/material-kayu-glugu.html` | Species-specific sales content | expand | `SAU-10-A02` and `SAU-10-A03` | Verify species identification, grade, moisture, legality, and availability claims. |
| `/desain.html` plus `/desain-*.html` | Visual style family, mostly timber-house oriented | manual review | `TOPIC:SAU-01`; move full-house intent to the relevant house property if appropriate | Determine which assets depict saung versus full houses and retain image rights/provenance. |
| `/penerapan.html`, `/rumah.html`, `/restaurant.html`, `/musholla.html` | Use-case pages with overlapping generic copy | merge | Application hub and `TOPIC:SAU-02` | Retain a separate page only when program, safety, accessibility, or operations materially differ. |
| `/rumah-kayu.html` and `/rumah-kayu/jasa-pembuatan-rumah-kayu-*` | Full-house intent outside the saung core | manual review | Separate timber-house hub/property; do not fold into saung articles | Review traffic, leads, ownership strategy, and redirect feasibility. |
| `/bambu/jasa-pembuatan-saung-gazebo-bambu-*` | 489 city/regency swaps | manual review | One bamboo service scope plus substantiated local case pages only | Export indexation, impressions, leads, unique text/images, and backlinks first. |
| `/besi/jasa-pembuatan-saung-gazebo-besi-*` | 489 sitemap routes plus 391 unsitemapped folders | manual review | One metal service scope plus substantiated cases | Reconcile sitemap, disk, deployment, canonical, and HTTP status. |
| `/beton/jasa-pembuatan-saung-gazebo-beton-*` | 489 city/regency swaps | manual review | One concrete service scope plus substantiated cases | Verify local evidence before keep/noindex/redirect decisions. |
| `/kayu/jasa-pembuatan-saung-gazebo-kayu-*` | 489 base plus 489 `-copy` sitemap routes | canonicalize | One canonical per real service/case; no `-copy` canonical | Crawl exact pairs, inspect response/canonical, then redirect or remove copies with history preserved. |
| `/hello-world.html` and `/sample-page` | Default WordPress placeholders | remove | None | Confirm no links, impressions, or intentional content. |
| `/author/`, `/category/`, feeds, comments, `/wp-json/`, `/wp-admin/` export routes | Thin archives and technical residue | noindex | None or controlled technical endpoint | Confirm what Cloudflare serves and ensure no useful API dependency is broken. |

Main risks:

- Location-template volume can consume crawling and confuse service-page relevance without proving local expertise.
- Material, service, and application pages currently overlap; titles alone do not define which page owns informational versus transactional intent.
- Timber-house coverage dilutes the saung entity and may create internal ambiguity.
- Existing pages make broad technical or durability claims without visible calculation, standard, test, treatment, or maintenance evidence.
- Unsafe DIY content is especially risky for structure, anchors, roof work, electricity, open flame, coatings, preservatives, and termiticides.

## Coverage matrix

| Completeness lens | Topic owner(s) | Coverage note |
|---|---|---|
| Definition, vocabulary, history, taxonomy | SAU-01, SAU-02 | Saung, gazebo, pendopo, pavilion, pergola, shelter, regional forms, and style choices are distinguished by form, use, and cultural context rather than synonym pages. |
| Anatomy, measurement, capacity | SAU-05, SAU-07, SAU-12, SAU-13, SAU-14 | Covers space, load path, ground interface, connections, roof, floor, rail, and enclosure. |
| Materials and properties | SAU-09, SAU-10, SAU-11, SAU-15 | Bamboo, timber, metal, concrete, hybrid assemblies, finishes, moisture, pests, and corrosion. |
| Need, survey, requirements, design | SAU-02, SAU-03, SAU-05 | Converts users, activities, site, climate, landscape, access, and appearance into a brief. |
| Selection and comparison | SAU-02, SAU-09, SAU-10, SAU-11, SAU-17 | Separates neutral choice support from quote/vendor evaluation. |
| Budget and procurement | SAU-17 | Scope, quantity assumptions, alternates, bids, contracts, warranty, schedule, and red flags. |
| Preparation and construction | SAU-03, SAU-08, SAU-12, SAU-18 | Survey, ground, logistics, sequencing, hold points, temporary works, QA, and handover. |
| Commissioning and operation | SAU-16, SAU-18 | Safety checks, drainage observation, documents, user limits, and emergency readiness. |
| Inspection and maintenance | SAU-15, SAU-19 | Material-specific inspection, cleaning, recoating, pest monitoring, and records. |
| Diagnosis, repair, upgrade, end of life | SAU-20 | Symptom-led triage, stabilization, repair-versus-replace, retrofit, disassembly, and reuse. |
| Stakeholders and site types | SAU-02, SAU-05, SAU-16, SAU-17 | Residential, hospitality, public, school, worship, landscape, contractor, operator, and neighbor needs. |
| Climate, geography, disaster context | SAU-03, SAU-07, SAU-08, SAU-13, SAU-15 | Rain, humidity, heat, coast, flood, soil, wind, landscape drainage, and seismic exposure without location-swapped pages. |
| New build, retrofit, prefab | SAU-02, SAU-07, SAU-12, SAU-18, SAU-20 | Distinct survey, connection, lifting, acceptance, and upgrade paths. |
| Safety, health, fire, K3 | SAU-07, SAU-08, SAU-12, SAU-15, SAU-16, SAU-18, SAU-20 | Strong professional/primary-source gates and clear DIY stop conditions. |
| Failure modes and myths | SAU-07, SAU-08, SAU-12, SAU-13, SAU-15, SAU-19, SAU-20 | Addresses uplift, settlement, decay, termites, corrosion, leaks, loose joints, fire, and unsafe rules of thumb. |
| Environment and circularity | SAU-03, SAU-09, SAU-10, SAU-11, SAU-15, SAU-20 | Biodiversity, drainage, sourcing evidence, material impacts, service life, disassembly, and waste. |
| Calculators, checklists, diagrams, cases | All topics | Calculators expose assumptions; diagrams do not become construction details; cases require real evidence and consent. |
| News/trends | N/A as a parent | Material changes are incorporated into maintained guides; trend-only filler is excluded. |

## Topical map

| Topic ID | Parent topic | Reader outcome | Required subtopics/questions | Evidence/formats | Boundary | Article target |
|---|---|---|---|---|---|---:|
| SAU-01 | Fundamentals, vocabulary, history, cultural context, and architectural form | Correctly identify the structure and choose a coherent form without flattening culturally specific precedents into generic “gazebo” labels. | Saung versus gazebo, pendopo, bale, pavilion, pergola, shelter; vernacular evolution; regional attribution; anatomy; open/semi-enclosed; style brief; proportion; adaptation ethics; render review. | Illustrated glossary, sourced history, form comparison, proportion diagrams, expert cultural/architect review, photo provenance. | Does not select a use program (`SAU-02`), engineer the structure (`SAU-07`), or engineer the roof (`SAU-13`). | 6 |
| SAU-02 | Use program, occupancy, and project type | Decide what the saung must do before choosing its look or material. | Residential rest/dining; hospitality/restaurant; park/school/public; worship/community; activities, occupancy and operating hours; permanent, prefab, movable, retrofit; neighbor impacts. | Brief template, stakeholder matrix, activity diagrams, operator checklist, real case only when documented. | Does not set dimensions (`SAU-05`), site placement (`SAU-03`), or quote scope (`SAU-17`). | 6 |
| SAU-03 | Site survey, climate, microclimate, and landscape integration | Record site constraints and choose a placement that works with circulation, planting, water, views, drainage, and outdoor ecology. | Boundaries, utilities/access; sun/shade; rain/wind; humidity/coast; flood/slope/soil clues; paths; views/privacy/noise; trees/root zones; planting; pond/pool interface; runoff/erosion; local rules and hazards. | Survey checklist, site-plan overlays, sun/wind/rain diagrams, measured photos, hazard map, arborist/landscape review where relevant. | Does not size foundations (`SAU-08`), design pool systems, or replace a full landscape master plan. | 6 |
| SAU-05 | Dimensions, layout, ergonomics, and accessibility | Turn occupants and activities into a usable, inclusive spatial layout. | Capacity; furniture clearances; circulation; headroom; entrances; ramps/steps; handrails and edge protection; wheelchair turning; child/elderly needs; floor level and transfer; anthropometry limits. | Dimension worksheets, plan diagrams, accessibility checklist, mock-up/field measurement. | Does not prescribe member sizes (`SAU-07`) or detailed floor/rail assemblies (`SAU-14`). | 6 |
| SAU-07 | Structural system, loads, and stability | Understand the load path and know which decisions require an engineer. | Gravity, occupancy, wind and seismic actions; uplift/overturning/racking; frames, posts, bracing and diaphragms; irregular/open structures; robustness; member design inputs; alteration risks; no universal spans. | Load-path diagrams, licensed standards, engineer review, calculation-input checklist, failure photos. | Does not provide universal member sizes, connection recipes (`SAU-12`), foundations (`SAU-08`), or roof weathering (`SAU-13`). | 6 |
| SAU-08 | Ground, foundations, drainage, and anchorage | Choose a survey and foundation pathway appropriate to soil, water, loads, and reversibility. | Soil/fill clues; settlement; footings, piers, slabs and screw/prefab concepts; frost N/A locally unless project-specific; drainage; splash zone; flood/scour; anchor interface; existing paving; excavation safety. | Site checklist, section diagrams, geotechnical/engineer gate, drainage observation, hold-point list. | Does not calculate foundation dimensions or anchor capacity; structural demand belongs to `SAU-07` and connection behavior to `SAU-12`. | 6 |
| SAU-09 | Bamboo systems | Select and specify bamboo based on species/culm condition, treatment, detailing, connections, and service environment. | Identification and grading; maturity/moisture; splitting/crushing; seasoning; preservative treatment; rain/ground separation; joint behavior; replaceable parts; sourcing; maintenance. | Expert identification, treatment records, moisture checks, detail diagrams, supplier evidence, no unverified life claims. | Does not prescribe structural spans (`SAU-07`), pesticide application (`SAU-15`), or generic timber guidance (`SAU-10`). | 6 |
| SAU-10 | Timber systems | Compare timber options and specify moisture, grade, legality, detailing, finish, and maintenance. | Species versus trade names; strength grade; moisture movement; jati/glugu and alternatives; engineered timber; sapwood/heartwood; legality/traceability; end grain; replaceability; finish compatibility. | Species/grade evidence, moisture measurements, supplier documentation, decision tables, expert review. | Does not promise performance from species name alone, size members (`SAU-07`), or own bamboo content (`SAU-09`). | 6 |
| SAU-11 | Steel, concrete, masonry, and hybrid systems | Choose non-timber or hybrid systems by structural, corrosion, thermal, construction, maintenance, and end-of-life trade-offs. | Carbon/stainless/coated steel; hollow sections; reinforced/precast concrete; masonry plinths; hybrid interfaces; coastal corrosion; galvanic risks; cracking/spalling; thermal comfort; disassembly. | System comparison, coating/manufacturer data, engineer review, defect photos, lifecycle matrix. | Does not provide welding/rebar/member designs; those require project engineering under `SAU-07`, `SAU-12`, and `SAU-18`. | 6 |
| SAU-12 | Joints, connectors, and interfaces | Understand how joints transfer force, tolerate movement, drain water, and remain inspectable. | Bamboo lashing/bolts/inserts; timber joinery and fasteners; steel bolts/welds; concrete embeds; dissimilar materials; edge/end distances as design inputs; concealed versus exposed; corrosion; tightening and replacement. | Exploded diagrams, manufacturer data, engineer review, mock-up/inspection checklist, destructive-test evidence where applicable. | Does not publish universal connector spacing, weld sizes, or anchor capacity; load demand belongs to `SAU-07`. | 6 |
| SAU-13 | Roof, ceiling, rainwater, and wind-driven rain | Select a roof assembly that manages heat, rain, drainage, uplift, maintenance, and local material realities. | Roof shapes and pitch logic; tiles, metal, shingles, thatch and membranes; underlay; ridge/eaves/flashing; gutters/downpipes; condensation; ventilation; ceiling; penetrations; wind uplift; safe access. | Roof sections, manufacturer instructions, rainfall/drainage assumptions, thermal comparison, inspection checklist. | Does not calculate roof structure (`SAU-07`) or specify electrical/lightning systems (`SAU-16`). | 6 |
| SAU-14 | Floor, edges, enclosure, comfort, and daily usability | Design safe contact surfaces and optional enclosure without turning a saung into an unhealthy room. | Floor materials and slip; gaps/drainage; steps/ramps; rails/guards; screens; shutters; seating; insects; daylight/glare; ventilation; acoustics; cleaning; child and elderly use. | Detail concepts, slip/accessibility evidence, user observation, comfort checklist, manufacturer data. | Does not set structural rail capacity or dimensions without engineering (`SAU-07`) and does not own spatial capacity (`SAU-05`). | 6 |
| SAU-15 | Moisture, termites, decay, corrosion, and protective treatments | Prevent material deterioration with design-first controls and safe, documented treatment choices. | Moisture pathways; termite inspection; fungal decay; borers; corrosion; coating compatibility; preservative/termiticide labels; ventilation and drainage; retreatment; exposure and waste; design for replacement. | Failure-mode map, SDS/label/registration, moisture readings, coating data, pest-professional review, PPE and disposal gates. | Does not teach unlicensed chemical mixing/application, diagnose structural capacity (`SAU-20`), or replace routine maintenance (`SAU-19`). | 6 |
| SAU-16 | Fire, electrical, lightning, security, and user safety | Identify hazards, define safe operating limits, and know when specialist design is mandatory. | Open flame/cooking; combustible roof/furnishings; separation and egress; extinguishers and emergency plan; outdoor electrical/IP suitability/RCD concepts; lightning risk; lighting; security; child/water edges; occupancy signage. | Current law/standard check, fire/electrical professional review, hazard register, emergency checklist, product certification. | Does not give electrical wiring, lightning-protection, or fire-rating designs; project professionals and authorities own those decisions. | 6 |
| SAU-17 | Budget, procurement, vendor selection, and contracts | Compare proposals on equal scope and control quality, exclusions, schedule, warranty, and change risk. | Cost anatomy; quantity/allowance assumptions; design-build versus separated roles; prefab versus site-built; quote normalization; samples/mock-ups; supplier verification; contract milestones; warranty; logistics; lifecycle cost. | Scope template, bid-comparison table, risk register, sample approval log, contract-review prompts. | Does not publish timeless price lists, replace legal advice, or supervise construction (`SAU-18`). | 6 |
| SAU-18 | Construction workflow, K3, quality assurance, and handover | Sequence work, define hold points, document hidden work, and accept only verifiable completion. | Mobilization; temporary works; excavation/lifting/work at height; material receipt/storage; setting out; foundations; frame/joints/roof/finish; inspections; tolerances per project; drainage test; punch list; as-builts; user briefing. | ITP/checklists, dated photos, delivery records, competent-person sign-offs, current SMKK source, handover pack. | Does not authorize DIY high-risk work or replace contractor methods, engineering inspection, or statutory approvals. | 6 |
| SAU-19 | Inspection and preventive maintenance | Establish risk-based inspection, cleaning, adjustment, coating, pest, roof, drainage, and record routines. | Baseline condition; frequent/seasonal/event-driven checks; material-specific intervals from evidence; cleaning; gutter/vegetation; fasteners; coatings; termites; floor/rail; electrical visual checks; log and escalation. | Inspection form, condition photos, trend log, manufacturer schedules, risk-based decision tree. | Does not promise one universal interval, perform invasive diagnosis (`SAU-20`), or instruct chemical application (`SAU-15`). | 6 |
| SAU-20 | Defects, repair, retrofit, replacement, and end of life | Triage symptoms safely, stop use when warranted, and choose repair, strengthening, component replacement, relocation, or dismantling. | Lean/racking; settlement; loose joints; cracks/splits; rot/termite; corrosion/spalling; leaks; unsafe rail/floor; emergency stabilization; root-cause diagnosis; repair specification; retrofit access; disassembly/reuse/waste. | Symptom matrix, stop-use triggers, engineer/pest/chemical gates, before/after records, repair acceptance checklist. | Does not diagnose from photos alone, give emergency shoring recipes, or replace routine prevention (`SAU-19`). | 6 |

## Related-domain opportunities

Cross-domain overlap is allowed because cannibalization is assessed within one domain.

| Related property | Independent viewpoint it may own | Useful relationship from `saung.id` |
|---|---|---|
| `kayu.co.id` | Timber species, grading, moisture, legality, processing, and product ecosystem | Cite deeper timber references while keeping the saung-specific selection and detailing decision complete here. |
| `taman.co.id` | Landscape design, planting, paths, drainage, and garden maintenance | Exchange contextual links around siting and landscape integration; neither domain must suppress the topic. |
| `almini.id` | Aluminium systems, finishes, corrosion, and fabrication | Supply material-specific evidence when aluminium appears in hybrid saung systems. |
| `panggung.id` | Raised platforms and stage systems | Compare temporary/event platforms without treating a saung deck as a stage by default. |
| `safety.co.id` and `firesafety.co.id` | Broader occupational and fire-safety systems | Support high-risk guidance while retaining saung-specific hazard decisions on this domain. |
| `kolam.co.id` | Pool design, operation, and water-edge safety | Coordinate when a saung is placed beside a pool; pool engineering remains independent. |

No topic is excluded merely because another owned domain can cover the same subject.

## Consolidation plan

1. Export Search Console and analytics by exact URL before touching the 2,934 location routes.
2. Crawl deployed responses, canonicals, titles, status codes, internal links, and content hashes. Reconcile the 391 unsitemapped steel folders and 489 timber `-copy` routes.
3. Preserve `/saung.html` as the likely central hub unless evidence supports a different canonical.
4. Separate neutral material selection from commercial service intent. Merge duplicate bamboo/material and timber/material routes only after choosing the stronger historical URL.
5. Keep local pages only when a real office/service boundary, local regulation, climate, supply chain, or documented project makes the page materially unique. Do not replace deleted city swaps with new city swaps.
6. Quarantine or noindex technical export residue and default WordPress pages after confirming deployment behavior.
7. Move or clearly subordinate full timber-house content so the saung entity is not diluted.
8. Redirect only after mapping each useful legacy URL to a genuinely equivalent destination; otherwise use manual review rather than forcing an irrelevant redirect.

## Internal-link architecture

- `/saung.html` is the central entity hub and links to every parent hub.
- Reader path: terminology/form (`SAU-01`) → need/program (`SAU-02`) → site/landscape (`SAU-03`) → layout (`SAU-05`) → system/material (`SAU-07`, `SAU-09`–`SAU-13`) → procurement/build (`SAU-17`, `SAU-18`) → care/repair (`SAU-19`, `SAU-20`).
- Site and landscape articles link laterally to foundation, drainage, roof, and preservation owners only where the constraint changes the decision.
- Each material hub links to structure, joints, preservation, maintenance, and repair using material-specific anchor context.
- Diagnostic pages link backward to prevention and inspection, then forward to professional repair/replacement choices.
- Neutral guidance links to commercial routes only when a reader is ready for a survey, quote, build, inspection, or repair; sales routes do not own informational definitions.
- Every child links upward to its topic hub, every hub lists all children, and no article receives a copied generic related-link block.

## Evidence and editorial standards

- Distinguish observation, hypothesis, rule, standard requirement, manufacturer instruction, and professional judgment.
- Verify the current status and project applicability of PP 16/2021, local PBG/SLF rules, licensed SNI texts, fire requirements, accessibility requirements, and construction-safety obligations at publication.
- Structural articles may explain load paths, failure modes, and design inputs but may not publish universal spans, member sizes, footing sizes, anchor capacities, fastener spacing, or copied details. A structural engineer reviews project-specific design.
- Bamboo/timber claims require verified material identity/grade, moisture/condition evidence, treatment records, exposure class, detailing, and maintenance assumptions. Species names alone do not prove strength or durability.
- Termiticide, preservative, coating, adhesive, and cleaning guidance must use the current registered label, safety data sheet, substrate/manufacturer instructions, ventilation, PPE, storage, spill, and disposal requirements. Never invent mixtures or off-label uses.
- Fire, electrical, lightning, work-at-height, lifting, welding, excavation, and temporary-support content needs a competent-person review and explicit stop conditions.
- Calculators expose inputs, units, uncertainty, exclusions, and professional sign-off thresholds; they are planning aids, not designs.
- Photos need provenance, consent, location/privacy review, and useful annotations. Case studies require real records and may not fabricate costs, defects, tests, or outcomes.
- Update-sensitive articles state an evidence review date and named source owner.

## First bounded publication cluster

Publish 12 assets in Wave 1:

1. `SAU-01-A01` — terminology and entity hub.
2. `SAU-02-A05` — activity, occupancy, and brief worksheet.
3. `SAU-03-A01` — pre-design site-survey checklist.
4. `SAU-05-A01` — capacity and layout worksheet.
5. `SAU-07-A01` — load-path and professional-review explainer.
6. `SAU-08-A01` — soil, water, and foundation pathway.
7. `SAU-09-A01` — bamboo decision guide.
8. `SAU-10-A01` — timber decision guide.
9. `SAU-11-A01` — material-system comparison.
10. `SAU-13-A01` — roof decision guide for wet tropical exposure.
11. `SAU-17-A03` — quote normalization checklist.
12. `SAU-19-A01` — baseline inspection and maintenance record.

The cluster connects definition → brief → survey/layout → structural/material/roof choices → quote comparison → care. It can upgrade existing high-value pages without publishing the full catalog at once.

Success signals:

- valid indexation and canonical selection for the central hub and child assets;
- impressions and clicks grouped by distinct intent, not only aggregate rank;
- worksheet/checklist completion, useful scroll or interaction, and return visits;
- qualified survey/quote contacts with material, site, size, and use information;
- crawl reduction or canonical clarity among legacy duplicate groups;
- no Search Console query/page pairs showing same-domain intent splitting;
- editorial review completion and correction rate for safety-critical claims.

## Definition of done

- All 18 parent topics have six distinct, validated article briefs in `ARTICLE_CATALOG.md`.
- IDs, titles, and slugs are unique; proposed slugs do not collide with current core routes.
- Every brief states one intent, audience, coverage promise, explicit exclusion with an owner, evidence format, related IDs, priority, and wave.
- The within-domain overlap register covers terminology, applications, materials, structure, preservation, maintenance, repair, and commercial pages.
- The sitemap/location/template audit is reconciled against the deployed site before redirects, removals, or canonicals are implemented.
- Structural, fire, chemical, pest, accessibility, electrical, and K3 content passes the stated evidence and competent-review gates.
- Wave 1 is published as a connected cluster, measured beyond rankings, and reviewed for cannibalization before the next wave.
