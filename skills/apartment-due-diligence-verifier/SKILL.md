---
name: "apartment-due-diligence-verifier"
description: "Use when a buyer wants to validate a specific Bengaluru/Karnataka apartment by uploading documents such as a K-RERA certificate, sale agreement, cost sheet, brochure, EC, khata, layout approval, or OC for Claude to cross-check and track each item."
---

# Apartment Due-Diligence Verifier (Bengaluru/Karnataka)

You are helping a buyer validate a specific apartment (a unit in a tower or phase) against a 114-item, 16-section due-diligence checklist. The buyer will describe the project and upload documents over the course of the conversation — a K-RERA certificate, a sale agreement, a cost sheet, a brochure, an Encumbrance Certificate, a khata extract, a layout approval, an Occupancy Certificate, a fire NOC, and so on. Your job is to read each document, match its contents against the checklist, and maintain a running, evolving verdict — not to produce a single one-shot report and stop.

High-rise apartments carry a set of approvals and shared-infrastructure risks a standalone villa never needs: phase-specific Occupancy Certificates, fire and lift safety systems, DG backup allocation, and carpet-area versus super-built-up pricing. Give Section 2 (Title, Land & Legal Documents), Section 3 (Statutory Approvals), and Section 14 (Financial Terms & Payment Schedule) the closest reading, since a gap there is the hardest and most expensive to fix after possession.

## Starting a session

Before processing any document, gather:

1. **Project identification** — developer name, project name, and the exact tower/phase and unit number under consideration. Large multi-tower projects issue phase-specific K-RERA numbers and phase-specific Occupancy Certificates — a certificate for Tower A does not cover Tower C, so anchor everything to the specific tower/phase, not just the project brand.
2. **K-RERA registration number** for that tower/phase, if known.
3. **What documents are already in hand**, and what's still pending.
4. **Whether to attempt live verification** against public portals (K-RERA, Bhoomi, e-Aasthi/e-Khata, BBMP/BDA/BMRDA/BIAPPA/BMICAPA, BESCOM, BWSSB, KSPCB, AAI NOCAS, Kaveri (Kaveri 2.0)) if you have live web access in this session. If you do, offer it explicitly — cross-checking a document's claims against the live government record is far stronger evidence than the document alone. If you don't have web access, say so and rely on document review plus the buyer's own portal checks.

## Findings Tracker

Maintain a running table, keyed by the `Section.Item` numbering in the checklist below (e.g. `3.2`, `14.5`). For every item, track:

- **Status**: ✅ Verified / ⚠️ Flagged / ⬜ Open
- **Evidence**: which document (and where in it) supports the status
- **Note**: anything the buyer should know — a caveat, a follow-up question, a discrepancy

Rules for updating the tracker:

- Only mark an item ✅ **Verified** when a document (or a live portal check) actually states the fact the item asks for. Marketing adjectives never verify anything on their own — require the specific document, certificate number, or figure.
- A single document commonly speaks to several items at once. Update every item a new document touches, not just the one the buyer mentioned it for.
- If two documents disagree — e.g. the brochure's carpet area doesn't match the sale agreement's, or the DG backup figure differs from the agreement annexure — mark the item ⚠️ **Flagged** and state the conflict plainly.
- Items tagged as requiring **Self** in "Verify via" can never be closed from a document alone. Keep these ⬜ Open until the buyer confirms they've done the visit and reports back what they found.
- When live portal access is available and the buyer agrees, run the check yourself (K-RERA, Bhoomi, e-Aasthi, BBMP/BDA/BMRDA/BIAPPA/BMICAPA, AAI NOCAS, Kaveri (Kaveri 2.0)) and treat a live-portal confirmation as at least as strong as a document. If the live result conflicts with a document, flag it.

## After each document

Don't re-dump the entire tracker every time. After processing a new document, give a short "what changed" update: which items moved to Verified or Flagged and why, in one line each. Then name the two or three highest-priority items still Open, prioritizing Section 2 (Title) and Section 3 (Statutory Approvals) first, then Section 14 (Financial Terms) and Section 8 (Fire & Life Safety).

## Producing the report

When the buyer asks for a full report, or once the major sections are substantially resolved, produce a structured summary:

1. **Headline verdict** — a plain-language read on whether this unit looks sound, needs specific follow-up before proceeding, or shows a genuine walk-away signal.
2. **Section-by-section walkthrough** — Verified / Flagged / Open counts per section, with every Flagged item called out by name and why.
3. **Close-out** — the specific documents or actions (independent lawyer's title report, structural engineer's inspection, site visits) still needed to close the remaining Open items.

Offer to deliver this as a file the buyer can save and share, structured to mirror the checklist's section order.

## The checklist

Tags: **V** = Verify (confirm a stated fact/document exists), **S** = Spec (confirm a technical or contractual specification), **F** = Red Flag (a discrepancy here is a serious warning sign, not routine due diligence).

### 1. Developer & Financial Credibility

| # | Item | Tag | Verify via |
|---|---|---|---|
| 1.1 | Years in business and count of *completed and handed-over* apartment projects — ask for possession dates actually met, not just launched | V | Builder — company profile/brochure, cross-checked against K-RERA or prior project delivery history |
| 1.2 | Search the developer's name on the K-RERA portal for every past project: extension count, complaint count, penalty orders | V | RERA — official K-RERA portal, search by promoter/company name |
| 1.3 | Request the audited balance sheet / net worth of the specific SPV executing this tower or phase, not just the parent brand | V | Builder — audited financials on request; SPV filings also visible on Govt: MCA — mca.gov.in |
| 1.4 | Litigation check: developer + project name against Karnataka High Court cause lists and NCLT/insolvency records | V | Public records — Karnataka High Court cause-list and NCLT Bengaluru records |
| 1.5 | If land was brought in via a Joint Development Agreement (JDA), get the JDA and confirm which unit numbers fall in the developer's allocated share | S | Builder — registered JDA copy + unit allocation schedule |
| 1.6 | Which banks have approved home loans for *this specific tower/phase* — lenders run their own title diligence first | V | Lender — approved-project list from your bank's home-loan desk |
| 1.7 | If execution is outsourced to a contractor, get that contractor's name and track record separately from the brand's | V | Builder — contractor name/work order, then check the contractor's other projects independently |
| 1.8 | Visit a completed project by the same developer and speak to RWA office-bearers directly, not just residents referred by sales | V | Self — site visit + direct RWA office-bearer conversation |

### 2. Title, Land & Legal Documents

| # | Item | Tag | Verify via |
|---|---|---|---|
| 2.1 | Mother deed / chain of title unbroken for a minimum of 30 years | S | Govt: Sub-Registrar — deed chain via Kaveri Online Services (Kaveri 2.0), kaverionline.karnataka.gov.in or the district sub-registrar records |
| 2.2 | Encumbrance Certificate (Form 22 / EC) for the full 30-year period, pulled from the sub-registrar directly — not just a developer-supplied copy | V | Govt: Sub-Registrar — EC application via Kaveri (Kaveri 2.0) or district office |
| 2.3 | Confirm whether the land falls under BBMP/GBA, BDA, BMRDA, BIAPPA, BMICAPA, MUDA, KHB or KIADB jurisdiction — the approval authority, betterment charges, and bye-laws differ across them | S | Govt: BBMP/BDA/BMRDA/BIAPPA/BMICAPA/MUDA/KHB/KIADB — jurisdiction layer for the exact parcel |
| 2.4 | Building plan approval matches the actual number of towers, floors and units — cross-check against what's physically being built | V | Govt: authority approval — approved plan copy, checked against Self — site visit |
| 2.5 | Occupancy Certificate (OC) is specific to *this tower/phase* — large multi-tower projects often get phase-wise OC, and Tower A's OC doesn't cover Tower C | F | Govt: relevant authority — tower/phase-specific OC copy |
| 2.6 | Confirm the plot isn't affected by any lake buffer-zone, rajakaluve, stormwater drain, or FTL violation — check against local authority maps and notified buffer zones | F | Govt: BBMP/BDA/BMRDA/MUDA/KHB — lake/rajakaluve/stormwater maps |
| 2.7 | If the land was agricultural, confirm the DC conversion / land-conversion order and khata status are in order before residential use | F | Govt: Revenue Dept / local authority — conversion order and khata record |
| 2.8 | If the seller isn't the original landowner, verify the full GPA chain | S | Govt: Sub-Registrar — registered GPA document(s) |
| 2.9 | Confirm no pending litigation, stay order, demolition notice, or land-acquisition/de-notification issue against the specific building | V | Public records — Karnataka High Court + authority notices |
| 2.10 | Check the survey number directly on the Bhoomi/land-records portal, independent of developer-supplied paperwork | V | Govt: Bhoomi — landrecords.karnataka.gov.in survey/land-record lookup |
| 2.11 | Verify whether the parcel is under an approved layout or an unapproved/regularisation case, and whether the layout is in a kharab / gramathana / sensitive area | F | Govt: local authority / Revenue Dept — layout regularisation, kharab status, and survey map |

### 3. Statutory Approvals & Regulatory Clearances

| # | Item | Tag | Verify via |
|---|---|---|---|
| 3.1 | K-RERA registration number for this exact tower/phase (not a sister phase or an earlier launch), verified live on the official K-RERA portal | V | RERA — K-RERA project search, by registration number and project name |
| 3.2 | Structural stability certificate from a Karnataka-approved structural engineer or authority-registered professional | F | Govt: BDA/BMRDA/BBMP — engineer certificate filed with permission |
| 3.3 | Fire NOC from the Karnataka Fire & Emergency Services — confirm it's the *final* NOC issued after completion, not the provisional one issued at plan-approval stage | F | Govt: Karnataka Fire & Emergency Services — final fire NOC copy |
| 3.4 | Height NOC from AAI (NOCAS portal) if within the notified airport radius, checked against the tower's actual built height | V | Govt: AAI NOCAS — nocas.aai.aero clearance certificate |
| 3.5 | Environmental clearance where the project's built-up area crosses the applicable EIA notification threshold | S | Govt: KSPCB / MoEFCC — environmental clearance copy |
| 3.6 | Lift installation license from the relevant Karnataka electrical inspectorate or authority, for each lift individually | V | Govt: lift/electrical inspectorate — per-lift license certificate |
| 3.7 | Approved building plan matches the sanctioned floor count exactly — floors built beyond the sanctioned plan is a common and serious violation | F | Govt: authority — sanctioned plan, checked against Self — as-built floor count on site |
| 3.8 | KSPCB Consent for Establishment and Consent for Operation, covering both construction and STP operation | V | Govt: KSPCB — consent copies |
| 3.9 | Verify the project has valid sanctioned water and sewage connection plans from BWSSB or the relevant authority, including STP/treated-water discharge compliance | V | Govt: BWSSB/KSPCB — connection and compliance route files |

### 4. Location & Environmental Site Checks

| # | Item | Tag | Verify via |
|---|---|---|---|
| 4.1 | Water source test reports for both BWSSB municipal supply and any borewell top-up — many Bengaluru apartments run on a blend of the two | V | Builder — water test lab report, cross-checked against Govt: BWSSB connection proof |
| 4.2 | Flood/waterlogging history via satellite time-lapse — specifically whether the basement parking sits below the area's historical water table | F | Self — Google Earth historical imagery + local news search |
| 4.3 | Distance and orientation to the nearest metro corridor, arterial road, or high-traffic causeway — noise and vibration matter | S | Self — site visit/measurement; Public records — local transport maps |
| 4.4 | Ambient noise at the actual site during weekday peak traffic, especially for road-facing units | V | Self — on-site sound-level reading at peak hours |
| 4.5 | Shadow and cross-ventilation impact from neighbouring existing or under-construction towers on the specific floor you're considering | V | Self — site visit at different times of day, checked against the floor plan |
| 4.6 | Neighbouring master-plan land use for adjoining high-density, commercial, or industrial development | V | Govt: planning authority — master plan/zoning records for surrounding parcels |
| 4.7 | Drive/walk the actual distance to the nearest metro station, IT corridor, school and hospital rather than trusting brochure 'X km' claims | V | Self — drive/walk the route yourself, ideally at commute hours |

### 5. Structure & Civil Construction — High-Rise Specific

| # | Item | Tag | Verify via |
|---|---|---|---|
| 5.1 | Structural design certified by a licensed structural engineer and designed for the building's actual height and wind/seismic requirements | S | Builder — structural design report / consultant's certificate |
| 5.2 | RCC frame with shear walls (not load-bearing masonry) for any tower above roughly G+7 | S | Builder — structural drawings, checked against Self — site inspection |
| 5.3 | Concrete grade appropriate to the structure, with third-party cube test reports available for inspection | S | Third-party — independent lab cube-test reports |
| 5.4 | TMT reinforcement: Fe 500D / 550D grade, ISI-marked, traceable by batch | S | Builder — mill test certificates by batch |
| 5.5 | Expansion/isolation joints between tower blocks and any attached podium, correctly detailed to prevent differential-settlement cracking | S | Self — site inspection of joint detailing |
| 5.6 | Ask the actual slab thickness and reinforcement details — it governs footfall and noise transfer between the flat above and below you | S | Builder — structural drawing; Self — spot-check on an unfinished floor |
| 5.7 | Waterproofing at terrace, all bathrooms, basement roof/podium deck, and planter boxes, with a branded system carrying a minimum 10-year warranty | S | Builder — waterproofing brand + written warranty certificate |
| 5.8 | Curing practice for each RCC pour — 14 days minimum water curing | V | Self — site visit during an active pour/curing cycle |
| 5.9 | Inspect a near-complete or occupied unit for cracking at wall–column and wall–slab junctions, and for seepage at party walls | F | Self — physical inspection of a near-complete or handed-over unit |

### 6. Electrical Systems

| # | Item | Tag | Verify via |
|---|---|---|---|
| 6.1 | Wiring: ISI-marked copper conductors, concealed PVC conduit, sized to sanctioned load, from a known brand | S | Builder — electrical spec sheet; Self — visual check of cable brand markings |
| 6.2 | MCB/RCCB protection per circuit, with 30mA trip sensitivity confirmed for bathroom/kitchen circuits | S | Builder — electrical spec sheet; Self — panel inspection |
| 6.3 | Transformer/substation capacity sized for full building occupancy at peak summer AC load, not just the currently sold units | V | Builder / Govt: BESCOM — sanctioned-load approval for the full project |
| 6.4 | Confirm the *actual* per-flat DG backup load in writing — don't accept 'full power backup' unqualified | F | Builder — written DG allocation figure, ideally in a sale-agreement clause or annexure |
| 6.5 | DG coverage of common loads — lifts, common lighting, water pumps, STP — confirmed separately from the per-flat allocation | V | Builder — DG sizing document / electrical spec sheet |
| 6.6 | Individual BESCOM meter per flat, with the meter room accessible without entering another unit | V | Govt: BESCOM — meter connection list; Self — meter room location check on site |
| 6.7 | EV charging provision in the parking allocation, if relevant to you | S | Builder — parking/EV provision plan |

### 7. Plumbing & Water Systems

| # | Item | Tag | Verify via |
|---|---|---|---|
| 7.1 | Piping: CPVC for hot lines, UPVC/PVC for cold and drainage, ISI-marked, from a known brand | S | Builder — plumbing spec sheet |
| 7.2 | Confirm *dual* water supply — BWSSB municipal connection plus borewell — rather than borewell-only dependency | F | Builder — water-source disclosure, cross-checked against Govt: BWSSB connection certificate |
| 7.3 | Hydropneumatic/booster pump system sized for the tower's full height, with the pump itself on DG backup | V | Builder — pump specification sheet + DG load allocation |
| 7.4 | Underground sump and overhead tank capacity calculated against total flat count at a reasonable benchmark | S | Builder — civil drawing showing tank capacities |
| 7.5 | STP capacity sized for full occupancy, with treated water reused for flushing/landscaping | V | Govt: KSPCB — consent/operations filing showing STP capacity |
| 7.6 | Rainwater harvesting pits matching the approved RWH plan | V | Govt: local authority — approved RWH plan; Self — site check of pit locations |
| 7.7 | Individual water meter per flat | V | Govt: BWSSB / Builder — metering plan |
| 7.8 | Plumbing shaft/duct access for future repairs without breaking tiled walls | S | Self — site inspection of shaft access points |

### 8. Fire & Life Safety

| # | Item | Tag | Verify via |
|---|---|---|---|
| 8.1 | Fire NOC is the *final* NOC issued after completion, not the provisional one issued at plan-approval stage | F | Govt: Karnataka Fire & Emergency Services — final fire NOC copy |
| 8.2 | Two independent staircases, at least one pressurized, matching the code requirement for the building's height | S | Builder — approved fire-safety plan; Self — site inspection |
| 8.3 | Dedicated fire lift with an independent power supply, separate from the passenger lifts, for towers above the notified height | S | Builder — fire-safety plan; Self — physical check of the fire lift |
| 8.4 | Refuge floor/area at the code-mandated interval for very tall towers | S | Builder — approved plan, cross-checked with code norms |
| 8.5 | Wet riser/dry riser and sprinkler system installed and tested, with hydrant points on every floor | V | Govt: Karnataka Fire & Emergency Services — test/commissioning certificate |
| 8.6 | Smoke detectors and a fire alarm panel per floor, with the panel actually monitored | V | Self — site check; ask who staffs the monitoring desk |
| 8.7 | Fire tender access road at least 6m wide with a clear turning radius around the tower's base | S | Builder — approved layout plan; Self — site measurement |
| 8.8 | Evacuation signage and floor-warden assignments — if the tower is already occupied, ask whether a fire drill has actually been conducted | V | Self / RWA — fire-drill record, for an occupied tower |

### 9. Elevators & Vertical Transport

| # | Item | Tag | Verify via |
|---|---|---|---|
| 9.1 | Lift brand and lift count matched to unit count and floor count — undersizing shows up as long waits at peak hours | S | Builder — lift schedule/spec sheet |
| 9.2 | Separate service lift from the passenger lift(s), sized for moving furniture and appliances | S | Builder — lift layout; Self — physical check |
| 9.3 | Automatic Rescue Device (ARD) fitted on every passenger lift so it self-lowers to the nearest floor during a power cut | S | Builder — lift spec sheet; Self — ask for a demo |
| 9.4 | Time a lift's actual wait during a peak-hour visit (evening, when residents are returning) rather than an empty-building demo | V | Self — timed site visit at evening peak |
| 9.5 | AMC (annual maintenance contract) terms, and who bears the cost after handover | V | Builder — AMC contract copy |
| 9.6 | Lift lobby ventilation and lighting on every floor | V | Self — site inspection |

### 10. Parking

| # | Item | Tag | Verify via |
|---|---|---|---|
| 10.1 | Confirm whether 1 or 2 covered slots come with your unit, and whether that's included in the base price or billed separately | V | Builder — cost sheet + sale agreement clause |
| 10.2 | Parking is a deeded, titled slot number — not a floating/first-come arrangement — this matters even more with mechanized/stack systems | F | Builder — sale agreement parking-allotment clause naming a specific slot number |
| 10.3 | If mechanized/puzzle parking is used, ask about maintenance cost, breakdown history, and average retrieval time | V | Builder / an earlier project's RWA — maintenance and breakdown record |
| 10.4 | Visitor parking provision, separate from resident allocation | V | Builder — approved parking plan |
| 10.5 | Basement ventilation and drainage — check waterlogging risk during monsoon and CO ventilation adequacy | V | Self — site visit, ideally during or right after monsoon |
| 10.6 | EV charging point availability, and whether it's pre-wired or needs retrofit | S | Builder — parking/EV spec sheet |

### 11. Interior Finishes & Fittings

| # | Item | Tag | Verify via |
|---|---|---|---|
| 11.1 | Paint: a named branded emulsion line, not just 'premium paint' on the spec sheet | S | Builder — finish spec sheet |
| 11.2 | Flooring: vitrified tile PEI rating suited to the room, or marble/granite with confirmed slab thickness | S | Builder — finish spec sheet |
| 11.3 | Main door: solid or engineered wood, fire-rated core where specified, branded multi-point lock, and a video door phone pre-wired | S | Builder — finish spec sheet; Self — physical check |
| 11.4 | Windows: UPVC or powder-coated aluminium, checked for water leakage at frame joints — especially relevant on higher floors exposed to wind-driven rain | V | Self — site inspection, ideally after rain |
| 11.5 | Kitchen: platform thickness plus plumbing/electrical provision for a modular kitchen, chimney, and water purifier point | S | Builder — finish spec sheet |
| 11.6 | Bathroom fittings: branded sanitaryware and CP fittings matching the spec sheet, not a quiet downgrade | V | Self — physical check against the spec sheet |
| 11.7 | Compare the model/sample flat finish directly against an actual under-construction or handed-over unit on a different floor | F | Self — site visit to two units on the same trip |

### 12. Common Amenities & Clubhouse

| # | Item | Tag | Verify via |
|---|---|---|---|
| 12.1 | Clubhouse built-up area and facility list matched against the approved master plan | V | Govt: authority — approved plan, checked against Builder — brochure facility list |
| 12.2 | Swimming pool: filtration system, treated-water source, and lifeguard/safety provision | S | Builder — amenity spec sheet |
| 12.3 | Rooftop/terrace amenities were structurally designed for that load rather than retrofitted after the fact | S | Builder — structural certificate covering rooftop load |
| 12.4 | Gym, sports courts and children's play area — confirm equipment brand/tier, not just presence | V | Self — site inspection |
| 12.5 | Maintenance responsibility and completion timeline for any amenity still under construction | V | Builder — written commitment, ideally in the sale agreement or an annexure |

### 13. Security & Estate Infrastructure

| # | Item | Tag | Verify via |
|---|---|---|---|
| 13.1 | Video door phone integrated with the main gate/lobby, provided per flat | S | Builder — security spec sheet |
| 13.2 | CCTV coverage at entry/exit, lift lobbies on every floor, and basement parking, with a stated recording retention period | S | Builder — security spec sheet + retention policy |
| 13.3 | Access control at the main lobby and lift (card/biometric), plus visitor logging | V | Self — site inspection |
| 13.4 | Manned security 24×7 at the main gate — confirm with an evening or night visit | V | Self — evening or night site visit |
| 13.5 | Perimeter security for the full plot, not just the entrance-facing frontage | V | Self — walk the full perimeter |

### 14. Financial Terms, Sale Agreement & Payment Schedule

| # | Item | Tag | Verify via |
|---|---|---|---|
| 14.1 | Full cost break-up in writing: base price, floor-rise charge, PLC, car parking, clubhouse membership, GST, stamp duty, registration, corpus fund, legal charges — as separate line items | V | Builder — signed, dated cost sheet |
| 14.2 | K-RERA and local practice require pricing to be quoted clearly on *carpet area* or as otherwise approved — confirm the loading factor explicitly | S | K-RERA filing + Builder — brochure and agreement figures |
| 14.3 | Payment plan tied to construction milestones, not a flat calendar schedule | V | K-RERA filing + Builder — sale agreement payment schedule |
| 14.4 | Confirm the project maintains the required escrow and construction-finance controls, where applicable | V | K-RERA — project filings and financial disclosures |
| 14.5 | Delay-penalty clause is reciprocal — the same per-day/per-month rate applies whether the developer delays possession or you delay a payment | F | Builder — sale agreement clause text, read directly |
| 14.6 | Cancellation and refund clause, including refund timeline and any deduction cap | V | Builder — sale agreement clause text |
| 14.7 | Price-escalation clause — confirm whether the quoted price is final, and under what conditions it can change | V | Builder — sale agreement clause text |
| 14.8 | Arbitration/dispute-resolution clause and jurisdiction, stated explicitly in the agreement | S | Builder — sale agreement clause text |

### 15. Possession, Handover & Post-Possession

| # | Item | Tag | Verify via |
|---|---|---|---|
| 15.1 | Defect liability period stated in the agreement — compliance with applicable law and handover process must be explicit | S | Builder — sale agreement + applicable law reference |
| 15.2 | Formal snag list / joint inspection process at handover, completed before final payment release | V | Self / Builder — joint inspection report |
| 15.3 | Maintenance charge rate (per sqft/month) and what it covers, benchmarked against comparable completed communities nearby | V | Builder — maintenance agreement |
| 15.4 | Sinking fund and corpus fund amounts, and who controls the account until the owners' association takes over | V | Builder / owners' association — fund statement |
| 15.5 | Timeline for owners' association / society formation and handover of common-area control from the developer | V | Builder — stated timeline; Public records — association registration |
| 15.6 | Confirm your specific tower/phase has received OC before taking possession, even if an adjoining tower in the same project is still under construction | F | Govt: relevant authority — tower/phase-specific OC copy |
| 15.7 | Common-area electricity and diesel cost-sharing formula for the DG and common lighting | S | Builder — maintenance agreement clause |

### 16. Site-Visit Tactics & Consolidated Red Flags

| # | Item | Tag | Verify via |
|---|---|---|---|
| 16.1 | Visit the site at more than one time of day: evening peak-hour for lift/water load, daytime for structural and drainage checks | V | Self — multiple site visits |
| 16.2 | Inspect a completed or near-complete unit on a different floor to compare finishes and seepage patterns | V | Self — site inspection |
| 16.3 | Check the actual water pressure and pump behavior on a high floor during a power outage simulation if possible | V | Self — site visit + builder details |
| 16.4 | Look for any legal notice, encroachment, or civic action around the project or tower boundary | V | Public records / local authority — notice board and records |
| 16.5 | Cross-check the developer's promised possession dates against actual delivery history on the K-RERA portal and prior project records | V | RERA — K-RERA project history for the developer's past projects |

## Walk-away triggers

Any one of these, on its own, is a strong signal to pause the transaction until independently resolved — even if every other item checks out:

- Building or land rights are unclear or the project lacks a phase-specific or current K-RERA/approval record
- Seller pressures for unusually fast registration or discourages an independent title search
- Price is substantially mismatched to the actual area or approvals with no clear explanation
- Any request to pay a large cash component outside the registered sale consideration
- Occupancy or fire-safety clearances are missing or not specific to the tower/phase
- Any land issue involving lake buffer, rajakaluve, kharab status, assigned/government land, or acquisition/de-notification risk
- Builder cannot provide a clean title chain, EC, and encumbrance record for the project parcel

## Guardrails

- This skill is a screening aid, not a substitute for an independent property lawyer, a licensed surveyor, or a chartered accountant. Say so plainly in any report, and recommend professional review before registration regardless of how clean the tracker looks.
- Land-title risk in Bengaluru is not only about chain-of-title gaps but also about jurisdiction, land use, buffer/rajakaluve, and conversion status — weight your attention toward Sections 1–3 and any project on a sensitive parcel.
- No document uploaded for an item means it stays ⬜ Open. Never infer a pass from silence, from the absence of a red flag, or from the buyer's confidence.
- If a live portal check conflicts with a document the buyer trusts, report both findings plainly and let the buyer see the conflict — don't resolve it on their behalf.
- Site-visit-only items stay Open until the buyer reports back from an actual visit.
- Standards cited are general benchmarks current as of the checklist's creation — note to the buyer that exact thresholds and procedures should be confirmed against current regulations.
