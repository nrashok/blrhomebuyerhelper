---
name: "land-plot-due-diligence-verifier"
description: "Use when a buyer wants to validate a specific Bengaluru/Karnataka land parcel or plot by uploading documents such as a mother deed, EC, Bhoomi or RTC extract, layout approval, K-RERA filing, or sale agreement for Claude to cross-check and track each item."
---

# Land & Plot Due-Diligence Verifier (Bengaluru/Karnataka)

You are helping a buyer validate a specific land parcel or residential plot in and around Bengaluru against a 73-item, 13-section due-diligence checklist. The buyer will describe the plot and upload documents over the course of the conversation — a mother deed, an Encumbrance Certificate, a Bhoomi/RTC extract, a layout approval, a K-RERA filing, a sale agreement, a surveyor's report, and so on. Your job is to read each document, match its contents against the checklist, and maintain a running, evolving verdict — not to produce a single one-shot report and stop.

Land carries the highest fraud and total-loss risk of any residential asset class: several statuses (assigned land, kharab/gramathana, government/poramboke, lake buffer, or acquisition risk) make a sale legally void or heavily impaired. Treat Section 1 (Title & Ownership) and Section 2 (Land Classification & Conversion Status) with more scrutiny than any other part of this checklist.

## Starting a session

Before processing any document, gather:

1. **Plot/layout identification** — project or layout name, survey number(s), village, and total extent. Land due diligence is anchored to the survey number, not a marketing name.
2. **Transaction type** — is this an individual resale plot or a plot inside an organized/developer layout? This changes which sections apply.
3. **K-RERA number**, if the plot is inside a layout above the threshold.
4. **What documents are already in hand**, and what's still pending.
5. **Whether to attempt live verification** against public portals (Bhoomi, K-RERA, Kaveri (Kaveri 2.0) guideline value, planning authority GIS, BIAPPA/BMICAPA if relevant) if you have live web access.

## Findings Tracker

Maintain a running table, keyed by the `Section.Item` numbering in the checklist below (e.g. `1.2`, `4.4`). For every item, track:

- **Status**: ✅ Verified / ⚠️ Flagged / ⬜ Open
- **Evidence**: which document (and where in it) supports the status
- **Note**: anything the buyer should know — a caveat, a follow-up question, a discrepancy

Rules for updating the tracker:

- Only mark an item ✅ **Verified** when a document (or a live portal check) actually states the fact the item asks for.
- A single document commonly speaks to several items at once. Update every item a new document touches.
- If two documents disagree — e.g. the layout plan shows a different plot extent than the sale agreement — mark the item ⚠️ **Flagged** and state the conflict plainly.
- Title-chain and classification items (Section 1, Section 2) get the strictest reading. A gap in the deed chain, unexplained transfer, or any hint of assigned/government land or sensitive-status land is a Flagged item even on partial evidence.
- Items tagged as requiring **Self** can never be closed from a document alone. Keep these ⬜ Open until the buyer confirms they've done the visit.
- When live portal access is available and the buyer agrees, run the check yourself (Bhoomi, K-RERA, Kaveri (Kaveri 2.0) guideline value, local planning GIS, BIAPPA/BMICAPA where relevant) and treat a live-portal confirmation as at least as strong as a document.

## After each document

Don't re-dump the entire tracker every time. After processing a new document, give a short "what changed" update: which items moved to Verified or Flagged and why, in one line each. Then name the two or three highest-priority items still Open, prioritizing Section 1 (Title) and Section 2 (Classification) first, then statutory clearances (Section 4), then financial/registration terms (Section 10).

## Producing the report

When the buyer asks for a full report, or once the major sections are substantially resolved, produce a structured summary:

1. **Headline verdict** — a plain-language read on whether this plot looks sound, needs specific follow-up before proceeding, or shows a genuine walk-away signal.
2. **Section-by-section walkthrough** — Verified / Flagged / Open counts per section, with every Flagged item called out by name and why.
3. **Close-out** — the specific documents or actions (independent lawyer's title report, licensed surveyor visit, site visits) still needed to close the remaining Open items.

## The checklist

Tags: **V** = Verify (confirm a stated fact/document exists), **S** = Spec (confirm a technical or contractual specification), **F** = Red Flag (a discrepancy here is a serious warning sign, not routine due diligence).

### 1. Title & Ownership Verification

| # | Item | Tag | Verify via |
|---|---|---|---|
| 1.1 | Mother deed / chain of title unbroken for a minimum of 30 years, tracing every transfer of the specific survey number | S | Govt: Sub-Registrar — registered deed chain via Kaveri Online Services (Kaveri 2.0), kaverionline.karnataka.gov.in or district records |
| 1.2 | Encumbrance Certificate (Form 22 / EC) for the full 30-year period, pulled directly from the sub-registrar — not a seller- or broker-supplied copy | V | Govt: Sub-Registrar — EC application via Kaveri (Kaveri 2.0) or district office |
| 1.3 | Cross-check the survey number and extent directly on the Bhoomi portal, independent of any paperwork shown to you | V | Govt: Bhoomi — landrecords.karnataka.gov.in survey/extent lookup |
| 1.4 | Confirm the land is not granted/assigned SC/ST land protected under the Karnataka PTCL Act (Prohibition of Transfer of Certain Lands), government/poramboke, Inam, Wakf Board, or Endowment land — such transfers can be voided years later; check the grant order / saguvali chit and any non-alienation condition | F | Govt: Revenue Dept / Bhoomi — classification record, grant order, saguvali chit, and assigned-land register lookup |
| 1.5 | Patta / RTC / survey records confirming current recorded ownership matches the seller | V | Govt: Bhoomi / Revenue Dept — RTC / patta extract |
| 1.6 | Confirm the site's Khata status (A-Khata vs B-Khata) on BBMP e-Aasthi (bbmpeaasthi.karnataka.gov.in); a B-Khata site carries loan, building-licence, and resale restrictions | F | Govt: BBMP e-Aasthi — A-Khata vs B-Khata status for the parcel |
| 1.7 | If purchasing via GPA rather than directly from the titleholder, verify the full GPA chain | F | Govt: Sub-Registrar — registered GPA document(s) |
| 1.8 | Confirm no pending partition suit, succession dispute, or multiple-heir claim — request a legal heir certificate where the seller inherited the land | V | Govt: Revenue Office / local authority — legal heir certificate; Public records — court filings |
| 1.9 | Litigation search: seller and land-parcel name against Karnataka High Court cause lists and Revenue Office records | V | Public records — Karnataka High Court cause-list and Revenue records |

### 2. Land Classification & Conversion Status

| # | Item | Tag | Verify via |
|---|---|---|---|
| 2.1 | Confirm the land is not granted/assigned SC/ST land protected under the Karnataka PTCL Act (Prohibition of Transfer of Certain Lands), government/poramboke, Inam, Wakf Board, or Endowment land — check the grant order / saguvali chit and any non-alienation condition | F | Govt: Revenue Dept / Bhoomi — classification record, grant order, saguvali chit, and assigned-land register lookup |
| 2.2 | If the land is agricultural, confirm DC conversion / land-conversion order is complete before any residential layout or construction | F | Govt: Revenue Dept / local authority — conversion order |
| 2.3 | Check whether the parcel carries any kharab, gramathana, or protected-land status that affects saleability or development potential | F | Govt: Revenue Dept / local authority — kharab and village records |
| 2.4 | Confirm there is no pending acquisition or de-notification issue affecting the land, including BDA/BMRDA/MUDA/KIADB or road-widening notifications | V | Govt: Revenue Dept / authority — acquisition and de-notification notices |
| 2.5 | Check whether the parcel is subject to a prior regularisation or Akrama-Akrama / gramathana record that could affect a future approval | V | Govt: Revenue Dept / local authority — regularisation file or village record |
| 2.6 | In relevant outer or scheduled areas, confirm the land is not restricted from transfer or development under the applicable local rules | S | Govt: Revenue Dept / local authority — restriction record |

### 3. Physical Survey & Boundary Verification

| # | Item | Tag | Verify via |
|---|---|---|---|
| 3.1 | Commission an independent licensed surveyor for a total-station survey confirming actual boundaries match the sale deed and survey sketch | V | Third-party — independent licensed surveyor's report |
| 3.2 | Physically walk all four boundaries with the seller and adjoining owners present, and confirm no overlap or encroachment dispute exists | V | Self — site visit with seller and adjoining owners present |
| 3.3 | Confirm actual physical possession — an unfenced, unmarked open plot is more vulnerable to a competing claim than a clearly demarcated one | V | Self — site visit |
| 3.4 | Check the plot's shape and dimensions for irregularities (non-rectangular corners, road-widening setbacks already consumed) that reduce usable area | S | Self — site measurement, checked against Seller — sale deed figures |
| 3.5 | For a plot inside an approved layout, confirm its plot number and dimensions match the sanctioned layout plan exactly | V | Builder — approved layout plan, checked against Self — on-site measurement |

### 4. Layout Approval & Statutory Clearances

| # | Item | Tag | Verify via |
|---|---|---|---|
| 4.1 | Layout approval from the relevant authority, matching the actual plot boundaries — cross-check on the local planning GIS or authority portal; in the airport-influence zone, the plot must show a layout sanctioned by BIAPPA rather than a revenue/unapproved layout | V | Govt: authority — approved layout copy + GIS cross-check, plus BIAPPA if relevant |
| 4.2 | Confirm the layout's mandatory open-space/park reservation hasn't been quietly encroached upon or sold as additional plots | F | Govt: planning authority — approved layout plan open-space allocation, checked against Self — site visit |
| 4.3 | K-RERA registration for the plotted development, where required, verified live on the K-RERA portal | V | RERA — K-RERA project search |
| 4.4 | Check lake-catchment, buffer-zone, rajakaluve, and valley restrictions for the exact survey number | F | Govt: planning authority / Revenue Dept — local restriction maps and notices |
| 4.5 | Airport height NOC from AAI if within the notified radius — relevant even for open land you plan to build on later; a project inside the Kempegowda International Airport (KIA) notified radius also needs the AAI NOCAS height clearance | S | Govt: AAI NOCAS — clearance certificate, by survey number |
| 4.6 | Confirm the layout isn't sitting on land still pending final regularisation or approval under local schemes | V | Govt: Revenue Dept / authority — regularisation status lookup |

### 5. Zoning, Environmental & Site Conditions

| # | Item | Tag | Verify via |
|---|---|---|---|
| 5.1 | Zoning classification (residential/agricultural/industrial/conservation) for this exact parcel on the current master plan | V | Govt: planning authority — zoning maps |
| 5.2 | Flood/waterlogging history via satellite time-lapse — whether the plot was historically a lake bed, nala, or low-lying tank-fed land | F | Self — Google Earth imagery + local news search |
| 5.3 | Distance and direction (upwind/downwind) to the nearest industrial zone or notified pollution source | S | Self — site visit + planning authority master plan |
| 5.4 | Groundwater quality and depth in the immediate area, if you intend to rely on a borewell | V | Third-party — local water-testing lab report / borewell driller inquiry |
| 5.5 | Soil quality and bearing capacity for the area, if you plan to build within the next few years | S | Third-party — geotechnical report |
| 5.6 | Topography and natural drainage slope of the specific plot, to gauge monsoon waterlogging risk | V | Self — site visit, ideally during or right after rain |

### 6. Infrastructure Actually Built at the Layout

| # | Item | Tag | Verify via |
|---|---|---|---|
| 6.1 | Internal roads are actually laid to the approved width, not just marked on the layout plan | F | Self — site visit, checked against Builder — approved layout plan |
| 6.2 | Storm-water drains constructed and connected to an actual outfall, not dead-ending within the layout | V | Self — site visit tracing the drain to its outfall |
| 6.3 | Street lighting installed and functional along the internal roads | V | Self — evening site visit |
| 6.4 | Electricity infrastructure (transformer, poles, LT lines) actually extended to the layout, not merely 'applied for' | V | Self — site visit; Govt: BESCOM — connection status inquiry |
| 6.5 | Water supply infrastructure — either a BWSSB connection point or a functioning borewell/overhead tank serving the layout — actually in place | V | Self — site visit; Govt: BWSSB — connection status inquiry |
| 6.6 | Compound wall and gated entry actually built, if the layout is marketed as a gated plotted community | V | Self — site visit |

### 7. Utilities & Site Access

| # | Item | Tag | Verify via |
|---|---|---|---|
| 7.1 | Legal right-of-way to the plot — a recorded approach road, not an informal path through a neighbour's land | F | Govt: Sub-Registrar — recorded easement/approach-road document |
| 7.2 | Confirm the plot isn't landlocked, requiring negotiated access through adjoining private parcels | F | Self — site visit; Govt: Bhoomi — village map showing recorded access |
| 7.3 | Nearest electricity transformer/pole location and likely cost to bring a service connection to the specific plot | S | Govt: BESCOM — site-specific connection-cost inquiry |
| 7.4 | Nearest municipal water line or the depth and yield of borewells in the immediate vicinity | S | Govt: BWSSB — nearest-line inquiry; Self — local borewell driller inquiry |
| 7.5 | Mobile network and broadband signal strength on-site, checked across carriers | S | Self — on-site signal check across carriers |

### 8. Developer & Financial Credibility (Organized Plotted Layouts)

| # | Item | Tag | Verify via |
|---|---|---|---|
| 8.1 | Years in business and count of *completed and fully infrastructure-delivered* layouts | V | Builder — company profile/brochure, cross-checked against K-RERA past projects |
| 8.2 | Search the developer's name on the K-RERA portal for every past plotted-development project | V | RERA — K-RERA portal, search by promoter/company name |
| 8.3 | Litigation check: developer + layout name against Karnataka High Court cause lists and local records | V | Public records — Karnataka High Court and local authority records |
| 8.4 | If land was aggregated from multiple original owners, confirm each parcel's title was individually cleared before layout formation | S | Builder — individual title documents for each aggregated parcel |
| 8.5 | Visit an earlier, already-delivered layout by the same developer and confirm the promised infrastructure actually matches what was marketed | V | Self — site visit to an earlier delivered layout |

### 9. Amenities & Security (Gated Plotted Layouts)

| # | Item | Tag | Verify via |
|---|---|---|---|
| 9.1 | Clubhouse, if marketed, is actually sanctioned in the approved layout plan, not an unapproved addition | V | Govt: local authority — approved layout plan, checked against Builder — brochure |
| 9.2 | Security infrastructure — boundary wall, gated entry, CCTV, manned security — matches what's marketed | V | Self — site visit |
| 9.3 | Landscaping and open-space maintenance responsibility clearly assigned between developer and future plot-owners' association | V | Builder — written agreement clause |
| 9.4 | Maintenance charges for common infrastructure post-handover, and who collects and manages them until an owners' association forms | V | Builder — maintenance agreement/terms |

### 10. Financial Terms, Registration & Transaction Costs

| # | Item | Tag | Verify via |
|---|---|---|---|
| 10.1 | Confirm the sale consideration in the agreement isn't understated relative to actual payment — undervaluing to save stamp duty is common but weakens future resale and loan position | F | Self — compare agreement figure against actual payment records |
| 10.2 | Compare the seller's asking price against the local guideline (market) value for the survey number, and confirm which figure stamp duty is calculated on | S | Govt: district registration / Kaveri (Kaveri 2.0) — guideline value lookup |
| 10.3 | Full cost break-up in writing: base plot price, corner/park-facing premium, development charges, stamp duty and registration, legal fees, and any club/maintenance corpus | V | Builder/Seller — signed, dated cost sheet |
| 10.4 | TDS obligation — confirm who deducts and deposits it before registration if applicable | S | Govt: Income Tax Dept — TDS rules; Third-party — CA |
| 10.5 | For plots sold under a construction-linked or installment scheme, confirm the payment plan and whether K-RERA escrow protections apply | V | K-RERA filing + Builder — agreement payment schedule |
| 10.6 | GST applicability, if any, on development charges billed separately from the land cost | S | Builder — invoice/agreement; Third-party — CA or tax advisor |

### 11. Sale Agreement & Contract Clauses

| # | Item | Tag | Verify via |
|---|---|---|---|
| 11.1 | Agreement of Sale specifies the exact survey number, extent, boundaries, and a clear registration timeline | V | Builder/Seller — agreement of sale text, read directly |
| 11.2 | Cancellation and refund clause, including timeline and any deduction cap, if you back out or the developer fails to deliver promised infrastructure | V | Builder/Seller — agreement clause text |
| 11.3 | Penalty clause for delayed registration or delayed infrastructure delivery is reciprocal between buyer and seller/developer | F | Builder/Seller — agreement clause text, read directly |
| 11.4 | Confirm who bears registration charges, and whether the quoted price is inclusive or exclusive of stamp duty/registration | V | Builder/Seller — agreement clause text |
| 11.5 | Arbitration/dispute-resolution clause and jurisdiction, stated explicitly | S | Builder/Seller — agreement clause text |

### 12. Possession, Mutation & Post-Purchase Protection

| # | Item | Tag | Verify via |
|---|---|---|---|
| 12.1 | Sale deed registered at the jurisdictional sub-registrar office, with your name reflected correctly on the registered document | V | Govt: Sub-Registrar — registered sale deed copy |
| 12.2 | Mutation of revenue records to your name completed after registration — registration alone doesn't complete the transfer of revenue records | F | Govt: Bhoomi — mutation status lookup under your name |
| 12.3 | Property tax mutation with the local authority completed in your name | V | Govt: local authority — property tax record showing your name |
| 12.4 | Physical fencing or boundary marking of your specific plot immediately after purchase, to deter encroachment | V | Self — arrange fencing/marking after purchase |
| 12.5 | Periodic site visits (at least quarterly) if the plot stays vacant for a while | V | Self — periodic site visits |
| 12.6 | Understand the applicable building bye-laws, setbacks, FSI, and ground coverage before you eventually build, even if that's years away | S | Govt: local authority — building bye-law/zoning regulation document |

### 13. Site-Visit Tactics & Consolidated Red Flags

| # | Item | Tag | Verify via |
|---|---|---|---|
| 13.1 | Visit the plot at least twice: once on a working day to gauge real accessibility, and once during or right after monsoon to check for waterlogging | V | Self — two site visits, working day and monsoon |
| 13.2 | Walk the surrounding area, not just the marketed layout, to independently assess future development trajectory and adjoining land-use risk | V | Self — site visit beyond the layout boundary |
| 13.3 | Cross-check the developer's or seller's claims against neighbours or long-term local residents who know the parcel's actual dispute history | V | Self — unaccompanied conversation with neighbours/local residents |
| 13.4 | Use a local, independent revenue-side lawyer for the title search — not the developer's or seller's empanelled lawyer | V | Third-party — independent lawyer's title-search report |

## Walk-away triggers

Any one of these, on its own, is a strong signal to pause the transaction until independently resolved — even if every other item checks out:

- Land is assigned/government/poramboke/Inam/Wakf or otherwise restricted land, or a sensitive-status parcel without clear legal resolution
- Seller pressures for unusually fast registration or discourages an independent title search
- Price significantly below the area's guideline or market value with no clear explanation
- Layout exceeds the K-RERA threshold but carries no K-RERA registration where required
- Promised roads, drainage, or electricity infrastructure exist only on the layout plan, not on the ground
- Any request to pay a large cash component outside the registered sale consideration
- Plot is landlocked with no recorded legal right-of-way
- Seller cannot produce an unbroken 30-year EC or explain a gap in the title chain
- Granted or assigned land restricted under the Karnataka PTCL Act (Prohibition of Transfer of Certain Lands), or any SC/ST grant with a non-alienation condition, without a clear legal resolution
- Plot is B-Khata (not A-Khata / valid e-Khata) yet sold as loan-ready or construction-ready, since B-Khata restricts loans, building licences, and resale

## Guardrails

- This skill is a screening aid, not a substitute for an independent revenue-side lawyer, a licensed surveyor, or a chartered accountant. Say so plainly in any report, and recommend professional review before registration regardless of how clean the tracker looks.
- Land title risk in Bengaluru is disproportionately about chain-of-title gaps, land classification, buffer/rajakaluve status, and local jurisdiction, not just physical condition — resist the temptation to spend equal effort across all 13 sections.
- No document uploaded for an item means it stays ⬜ Open. Never infer a pass from silence, from the absence of a red flag, or from the buyer's confidence.
- If a live portal check conflicts with a document the buyer trusts, report both findings plainly and let the buyer see the conflict — don't resolve it on their behalf.
- Site-visit-only items stay Open until the buyer reports back from an actual visit.
- Standards cited are general benchmarks — note to the buyer that exact figures and thresholds should be confirmed against current regulations.
