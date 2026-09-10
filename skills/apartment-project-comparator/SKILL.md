---
name: "apartment-project-comparator"
description: "Use when a buyer wants to compare two or more Bengaluru/Karnataka apartment projects side by side on price, value, builder credibility, location, amenities, and due-diligence risk. Start from the buyer's existing project data and deepen each project as documents are shared."
---

# Apartment Project Comparator (Bengaluru/Karnataka)

You are helping a buyer choose between two or more specific apartment projects in Bengaluru/Karnataka. Unlike a single-project due-diligence run, this starts immediately from whatever the buyer already knows (a brochure, a price list, a sales pitch, a friend's opinion) and gets more rigorous only as actual documents are shared for a given project. The goal is a clear-eyed side-by-side comparison, not a verdict — the buyer weighs the trade-offs, you make sure they're seeing them accurately.

This skill embeds the same 16-section, 114-item due-diligence checklist as `apartment-due-diligence-verifier`, so it works standalone. If that skill is also loaded and the buyer wants to run a full deep-dive on whichever project they've narrowed down to, defer to it or keep using the embedded checklist below directly.

## Starting a session

Gather, for each project:

1. **Identity** — developer, project, locality, and the specific configuration being compared.
2. **A reference point, if proximity matters to the buyer** — commute to a workplace, school, family, or IT corridor.
3. **Whatever they already know** about each project — price, size, floor, possession timeline, amenities, brochure claims.
4. **What matters most to them**, if they're willing to say — price, resale/rental potential, builder pedigree, ready-to-move vs under-construction, specific amenities, and so on.
5. **Whether to attempt live verification** (K-RERA project/promoter search, MCA company search) if you have live web access in this session.

## Per-project Findings Tracker

Maintain one independent tracker per project. Use a four-state model:

- ✅ **Confirmed** — from an actual document, a live portal check, or a source the buyer explicitly trusts
- 🟡 **Estimated** — from a brochure, a sales pitch, a web listing, or something the buyer heard
- ⬜ **Unknown** — nothing said about it yet
- ⚠️ **Flagged** — a red flag, contradiction, or something that doesn't add up

Be explicit about status, especially price and area. Track each project against these comparison dimensions:

1. **Identity & Configuration** — developer, project, tower/phase, BHK, carpet area, super built-up area, loading factor
2. **Price & Payment Terms** — total price, price per sqft on carpet area, payment plan, and all extra charges
3. **Location & Connectivity** — locality, distance/time to the buyer's reference point(s), nearest metro/arterial road, IT corridor, schools, and hospitals as relevant
4. **Builder Credibility** — years in business, K-RERA complaint/extension history, litigation, and delivery track record
5. **Construction & Specs** — structure type, material/finish specs, and inspection notes
6. **Amenities & Community** — clubhouse and key amenities, density, maintenance charge rate
7. **Possession & Risk** — possession status, timeline, K-RERA registration status and number, defect liability terms
8. **Due-diligence red flags** — anything Flagged, cross-referenced against the walk-away triggers below

## Deepening a project

When the buyer uploads an actual document for one project, process it as a single-project due-diligence run: match it against the full checklist below for that project specifically, upgrade the relevant comparison rows from Estimated/Unknown to Confirmed, and surface anything Flagged immediately.

## After each update

After new information arrives for one project, give a short "what changed" note — which rows moved from Estimated/Unknown to Confirmed, or what got Flagged — and note if it shifts the overall picture.

## Producing the comparison

1. **Quick-look table** — one row per project: price/sqft on carpet area, BHK & carpet area, possession status, builder K-RERA-complaint history, and any active red flags.
2. **Dimension-by-dimension walkthrough** — Price & Value, Location & Connectivity, Builder Credibility, Construction & Amenities, Risk — noting which project leads on each and why.
3. **Trade-off summary** — if the buyer named what matters most, lead with that read.
4. **Open items** — what's still Estimated or Unknown for each project, prioritized by what would most change the comparison if confirmed.

Offer to deliver this as a file the buyer can save and share.

## The embedded checklist

Used for deepening any individual project to full due-diligence rigor. Tags: **V** = Verify, **S** = Spec, **F** = Red Flag.

### 1. Developer & Financial Credibility

| # | Item | Tag | Verify via |
|---|---|---|---|
| 1.1 | Years in business and count of *completed and handed-over* apartment projects | V | Builder — company profile/brochure, cross-checked against K-RERA project history |
| 1.2 | Search the developer's name on the K-RERA portal for every past project: extension count, complaint count, penalty orders | V | RERA — official K-RERA portal |
| 1.3 | Request the audited balance sheet / net worth of the specific SPV executing this tower or phase | V | Builder — audited financials on request; SPV filings visible on MCA |
| 1.4 | Litigation check: developer + project name against Karnataka High Court cause lists and NCLT/insolvency records | V | Public records — Karnataka High Court and NCLT Bengaluru records |
| 1.5 | If land was brought in via a JDA, get the JDA and confirm which unit numbers fall in the developer's allocated share | S | Builder — registered JDA copy + schedule |
| 1.6 | Which banks have approved home loans for *this specific tower/phase* | V | Lender — approved-project list from your bank |
| 1.7 | If execution is outsourced to a contractor, get that contractor's name and track record separately | V | Builder — contractor name/work order |
| 1.8 | Visit a completed project by the same developer and speak to RWA office-bearers directly | V | Self — site visit + direct RWA conversation |

### 2. Title, Land & Legal Documents

| # | Item | Tag | Verify via |
|---|---|---|---|
| 2.1 | Mother deed / chain of title unbroken for a minimum of 30 years | S | Govt: Sub-Registrar — deed chain through Kaveri Online Services (Kaveri 2.0), kaverionline.karnataka.gov.in or the district registry |
| 2.2 | Encumbrance Certificate (Form 22 / EC) for the full 30-year period | V | Govt: Sub-Registrar — EC application via Kaveri (Kaveri 2.0) |
| 2.3 | Confirm whether the land falls under BBMP/GBA, BDA, BMRDA, BIAPPA, BMICAPA, MUDA, KHB or KIADB jurisdiction — the sanctioning authority, betterment charges, and bye-laws differ across them | S | Govt: planning authority — jurisdiction layer on the parcel |
| 2.4 | Building plan approval matches the actual number of towers, floors and units | V | Govt: authority — approved plan copy |
| 2.5 | Occupancy Certificate (OC) is specific to *this tower/phase* | F | Govt: relevant authority — tower/phase-specific OC copy |
| 2.6 | Confirm the plot isn't affected by lake buffer, rajakaluve, or FTL/drainage violation | F | Govt: local authority — lake/buffer maps |
| 2.7 | If the land was agricultural, confirm the DC conversion / land-conversion order and khata status are in order | F | Govt: Revenue Dept / authority — conversion order and khata record |
| 2.8 | If the seller isn't the original landowner, verify the full GPA chain | S | Govt: Sub-Registrar — registered GPA document(s) |
| 2.9 | Confirm no pending litigation, stay order, demolition notice, or acquisition/de-notification issue | V | Public records — Karnataka High Court + authority notices |
| 2.10 | Check survey number on Bhoomi, independent of developer paperwork | V | Govt: Bhoomi — landrecords.karnataka.gov.in |
| 2.11 | Verify whether the parcel is under an approved layout or an unapproved/regularisation case | F | Govt: local authority / Revenue Dept — layout regularisation and survey map |

### 3. Statutory Approvals & Regulatory Clearances

| # | Item | Tag | Verify via |
|---|---|---|---|
| 3.1 | K-RERA registration number for this exact tower/phase, verified live on the K-RERA portal | V | RERA — K-RERA project search |
| 3.2 | Structural stability certificate from a Karnataka-approved structural engineer | F | Govt: authority — engineer certificate |
| 3.3 | Fire NOC from the Karnataka Fire & Emergency Services | F | Govt: Karnataka Fire & Emergency Services — final fire NOC |
| 3.4 | Height NOC from AAI if within the notified airport radius | V | Govt: AAI NOCAS — clearance certificate |
| 3.5 | Environmental clearance where the project's built-up area crosses the threshold | S | Govt: KSPCB / MoEFCC — clearance copy |
| 3.6 | Lift installation license from the relevant authority, per lift | V | Govt: electrical/inspectorate — per-lift license |
| 3.7 | Approved building plan matches the sanctioned floor count exactly | F | Govt: authority — sanctioned plan, checked against Self |
| 3.8 | KSPCB Consent for Establishment and Consent for Operation | V | Govt: KSPCB — consent copies |
| 3.9 | Valid sanctioned water and sewage connection plans from BWSSB / relevant authority | V | Govt: BWSSB/KSPCB — connection files |

### 4. Location & Environmental Site Checks

| # | Item | Tag | Verify via |
|---|---|---|---|
| 4.1 | Water source test reports for both BWSSB and any borewell top-up | V | Builder — water test lab report |
| 4.2 | Flood/waterlogging history via satellite time-lapse | F | Self — Google Earth imagery + local news search |
| 4.3 | Distance and orientation to the nearest metro corridor or arterial road | S | Self — site visit/measurement |
| 4.4 | Ambient noise at the site during weekday peak traffic | V | Self — on-site sound-level reading |
| 4.5 | Shadow and cross-ventilation impact from neighbouring towers | V | Self — site visit at different times of day |
| 4.6 | Neighbouring master-plan land use for adjoining high-density or industrial development | V | Govt: authority — master plan/zoning portal |
| 4.7 | Drive/walk actual distance to the nearest metro station, IT corridor, school and hospital | V | Self — drive/walk the route |

### 5. Structure & Civil Construction — High-Rise Specific

| # | Item | Tag | Verify via |
|---|---|---|---|
| 5.1 | Structural design certified for the actual height and wind/seismic requirements | S | Builder — design report / consultant's certificate |
| 5.2 | RCC frame with shear walls for any tower above roughly G+7 | S | Builder — structural drawings; Self — site inspection |
| 5.3 | Concrete grade appropriate to the structure, with third-party cube tests | S | Third-party — lab cube-test reports |
| 5.4 | TMT reinforcement: Fe 500D / 550D grade, ISI-marked and batch-traceable | S | Builder — mill test certificates |
| 5.5 | Expansion/isolation joints between tower blocks and podium | S | Self — inspection of joint detailing |
| 5.6 | Actual slab thickness and reinforcement details | S | Builder — structural drawings |
| 5.7 | Waterproofing and warranty coverage for terrace, bathrooms and podium deck | S | Builder — waterproofing certificate |
| 5.8 | Curing practice for each RCC pour | V | Self — site visit during curing |
| 5.9 | Cracking and seepage inspection in a near-complete or occupied unit | F | Self — physical inspection |

### 6. Electrical Systems

| # | Item | Tag | Verify via |
|---|---|---|---|
| 6.1 | Wiring and cable brand quality, concealed conduits, sized to sanctioned load | S | Builder — electrical spec sheet |
| 6.2 | MCB/RCCB protection per circuit | S | Builder — electrical spec sheet; Self — panel inspection |
| 6.3 | Transformer/substation capacity sized for full building occupancy | V | Builder / Govt: BESCOM — sanctioned-load approval |
| 6.4 | Actual per-flat DG backup load in writing | F | Builder — DG allocation figure |
| 6.5 | DG coverage of common loads | V | Builder — DG sizing document |
| 6.6 | Individual BESCOM meter per flat | V | Govt: BESCOM — meter connection list |
| 6.7 | EV charging provision in the parking allocation | S | Builder — parking/EV spec sheet |

### 7. Plumbing & Water Systems

| # | Item | Tag | Verify via |
|---|---|---|---|
| 7.1 | Piping material and quality standards | S | Builder — plumbing spec sheet |
| 7.2 | Dual water supply — BWSSB plus borewell | F | Builder — water-source disclosure |
| 7.3 | Booster pump system sized for tower height | V | Builder — pump specification sheet |
| 7.4 | Underground sump and overhead tank capacity calculation | S | Builder — civil drawing |
| 7.5 | STP capacity and treated-water reuse | V | Govt: KSPCB — consent / operations filing |
| 7.6 | Rainwater harvesting pits matching the approved RWH plan | V | Govt: local authority — approved RWH plan |
| 7.7 | Individual water meter per flat | V | Govt: BWSSB / Builder — metering plan |
| 7.8 | Plumbing shaft/duct access without breaking tiled walls | S | Self — site inspection |

### 8. Fire & Life Safety

| # | Item | Tag | Verify via |
|---|---|---|---|
| 8.1 | Fire NOC is the final NOC after completion | F | Govt: Karnataka Fire & Emergency Services |
| 8.2 | Two independent staircases; at least one pressurized | S | Builder — fire-safety plan; Self — site inspection |
| 8.3 | Dedicated fire lift with independent power supply | S | Builder — fire-safety plan |
| 8.4 | Refuge floor/area for very tall towers | S | Builder — approved plan |
| 8.5 | Wet riser/dry riser and sprinkler system installation/testing | V | Govt: Karnataka Fire & Emergency Services — test certificate |
| 8.6 | Smoke detectors and fire alarm panel per floor | V | Self — site check |
| 8.7 | Fire tender access road and turning radius | S | Builder — approved layout plan; Self — measurement |
| 8.8 | Evacuation signage and fire drill record | V | Self / RWA — fire-drill record |

### 9. Elevators & Vertical Transport

| # | Item | Tag | Verify via |
|---|---|---|---|
| 9.1 | Lift brand and lift count matched to traffic | S | Builder — lift spec sheet |
| 9.2 | Separate service lift | S | Builder — lift layout |
| 9.3 | ARD fitted on each passenger lift | S | Builder — lift spec sheet |
| 9.4 | Peak-hour lift wait times | V | Self — timed site visit |
| 9.5 | AMC terms after handover | V | Builder — AMC contract |
| 9.6 | Lift lobby ventilation and lighting | V | Self — site inspection |

### 10. Parking

| # | Item | Tag | Verify via |
|---|---|---|---|
| 10.1 | Covered slots and price treatment | V | Builder — cost sheet + agreement clause |
| 10.2 | Deeded, titled slot number | F | Builder — parking-allotment clause |
| 10.3 | Mechanized parking maintenance and retrieval time | V | Builder / RWA — maintenance record |
| 10.4 | Visitor parking | V | Builder — approved parking plan |
| 10.5 | Basement ventilation and drainage | V | Self — site visit |
| 10.6 | EV charging point provision | S | Builder — parking/EV spec sheet |

### 11. Interior Finishes & Fittings

| # | Item | Tag | Verify via |
|---|---|---|---|
| 11.1 | Paint specification | S | Builder — finish spec sheet |
| 11.2 | Flooring and tile quality | S | Builder — finish spec sheet |
| 11.3 | Main door and lock specification | S | Builder — finish spec sheet |
| 11.4 | Window quality and water leakage checks | V | Self — site inspection |
| 11.5 | Kitchen platform and modular provisions | S | Builder — finish spec sheet |
| 11.6 | Bathroom fittings match spec sheet | V | Self — physical check |
| 11.7 | Compare sample flat to actual unit | F | Self — site visit |

### 12. Common Amenities & Clubhouse

| # | Item | Tag | Verify via |
|---|---|---|---|
| 12.1 | Clubhouse built-up area and facility list against approved plan | V | Govt: authority — approved plan |
| 12.2 | Swimming pool | S | Builder — amenity spec sheet |
| 12.3 | Rooftop amenities structurally designed for load | S | Builder — structural certificate |
| 12.4 | Gym, sports courts and children's play area | V | Self — site inspection |
| 12.5 | Maintenance responsibility and completion timeline | V | Builder — written commitment |

### 13. Security & Estate Infrastructure

| # | Item | Tag | Verify via |
|---|---|---|---|
| 13.1 | Video door phone integrated with lobby | S | Builder — security spec sheet |
| 13.2 | CCTV coverage and retention period | S | Builder — security spec sheet |
| 13.3 | Access control and visitor logging | V | Self — site inspection |
| 13.4 | Manned security 24×7 | V | Self — evening or night site visit |
| 13.5 | Perimeter security for the full plot | V | Self — full perimeter walk |

### 14. Financial Terms, Sale Agreement & Payment Schedule

| # | Item | Tag | Verify via |
|---|---|---|---|
| 14.1 | Full cost break-up and separate charges | V | Builder — signed, dated cost sheet |
| 14.2 | Pricing on carpet area or clearly disclosed, loading factor explicit | S | K-RERA filing + Builder — brochure and agreement figures |
| 14.3 | Payment plan tied to construction milestones | V | K-RERA filing + Builder — sale agreement scheduling |
| 14.4 | Escrow and construction-finance controls | V | K-RERA — project filings |
| 14.5 | Delay-penalty clause reciprocal | F | Builder — sale agreement clause text |
| 14.6 | Cancellation and refund clause | V | Builder — sale agreement clause text |
| 14.7 | Price-escalation clause | V | Builder — sale agreement clause text |
| 14.8 | Arbitration/dispute-resolution clause and jurisdiction | S | Builder — sale agreement clause text |

### 15. Possession, Handover & Post-Possession

| # | Item | Tag | Verify via |
|---|---|---|---|
| 15.1 | Defect liability period and handover process | S | Builder — sale agreement |
| 15.2 | Formal snag list / joint inspection | V | Self / Builder — joint inspection report |
| 15.3 | Maintenance charge rate and what it covers | V | Builder — maintenance agreement |
| 15.4 | Sinking fund and corpus fund amounts | V | Builder / owners' association — fund statement |
| 15.5 | Timeline for association formation | V | Builder — stated timeline |
| 15.6 | Tower/phase-specific OC before taking possession | F | Govt: relevant authority — OC copy |
| 15.7 | Common-area electricity and diesel cost-sharing formula | S | Builder — maintenance agreement clause |

### 16. Site-Visit Tactics & Consolidated Red Flags

| # | Item | Tag | Verify via |
|---|---|---|---|
| 16.1 | Visit at more than one time of day | V | Self — multiple site visits |
| 16.2 | Inspect completed or near-complete unit on another floor | V | Self — site inspection |
| 16.3 | Check water pressure and pump behavior on a high floor | V | Self — site visit |
| 16.4 | Look for any legal notice or civic action around the project | V | Public records / authority notice board |
| 16.5 | Cross-check promised possession dates against actual delivery history on K-RERA | V | RERA — K-RERA project history |

## Walk-away triggers

- Project or parcel lacks valid K-RERA/approval record where required
- Land status is unclear or is in a sensitive buffer / kharab / acquisition risk area
- Seller discourages independent title search or requests unusual cash structure
- Missing or non-phase-specific OC or fire-safety clearance
- Any request to make large cash payments outside the registered sale consideration
- Builder cannot explain a poor title, EC or land-use mismatch

## Guardrails

- This skill is a screening aid, not a substitute for an independent property lawyer, surveyor, or chartered accountant.
- Land-title risk in Bengaluru is heavily shaped by conversion status, land use, buffer restrictions, and jurisdiction, not just building quality.
- If a live portal check conflicts with a document, report both findings plainly.
- Site-visit-only items stay Open until the buyer reports back from an actual visit.
