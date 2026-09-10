# Apartment Project Comparator Test Cases

### 1) Early-state comparison — brochures only
- Scenario name & intent: "Two projects, only brochures — the comparator should use Estimated/Unknown correctly and never label a brochure as Confirmed."
- Inputs: "property type: apartment comparison; locality: North Bengaluru; projects: Aster Park (Yelahanka) and Magnolia Crest (Hebbal); docs: brochures and web price lists only; no K-RERA, no cost sheets, no approvals, no site visit."
- Expected tracker outcome: "Aster Park: price, area, amenities, possession -> Estimated; Magnolia Crest: price, area, amenities, possession -> Estimated; K-RERA registration and builder history -> Unknown; no project should be marked Confirmed on price, area, or possession."
- Expected verdict: "needs-follow-up; no Walk-away trigger yet because no valid red flags are confirmed."
- Must NOT happen: "must not mark price, area or claims as Confirmed from a brochure alone; must not treat a project as sound because one brochure looks more polished."

### 2) Clean A-Khata apartment — comparator deepens to sound
- Scenario name & intent: "One project is later deepened with proper documents and should become sound while the other remains marketing-heavy."
- Inputs: "property type: apartment comparison; locality: Whitefield; projects: Aster Park and Azure Vale Homes; docs: Aster Park has e-Khata, K-RERA, final fire NOC, tower-specific OC, cost sheet; Magnolia is still brochure-only."
- Expected tracker outcome: "Aster Park: 2.7 ✅, 2.5 ✅, 3.1 ✅, 3.3 ✅, 14.1 ✅; Magnolia: price and builder claims remain Estimated; no Flagged items for Aster Park."
- Expected verdict: "sound for Aster Park; Magnolia remains needs-follow-up; no Walk-away trigger for Aster Park."
- Must NOT happen: "must not keep Aster Park at Estimated just because a sister project is still weak; must not call Magnolia sound based on a brochure."

### 3) Builder complaint-history trap
- Scenario name & intent: "One project appears cheaper, but the comparator should surface past K-RERA complaint and extension history before ranking it."
- Inputs: "property type: apartment comparison; locality: East Bengaluru; projects: Grove Heights and Riverline Residency; docs: brochure and price list show Grove Heights cheaper; K-RERA search shows repeated extension orders and complaints for Grove Heights; Riverline has negligible complaint history."
- Expected tracker outcome: "Grove Heights developer credibility -> ⚠️ Flagged on 1.2 and 1.6 if delays or complaint history are confirmed; Riverline remains Estimated until documents are uploaded; price alone should not override the risk profile."
- Expected verdict: "needs-follow-up; the cheaper project may still be riskier and should not rank above the safer project without more review."
- Must NOT happen: "must not treat lower price as automatically better; must not ignore the complaint history simply because the developer's brochure is glossy."

### 4) Provisional fire NOC passed off as final in the comparison
- Scenario name & intent: "One project's promised fire safety is weaker than the brochure suggests — comparator should surface it as Flagged."
- Inputs: "property type: apartment comparison; locality: Sarjapur; projects: Solace Park and Ashok Residency; docs: Solace Park has a builder email claiming 'fire NOC done'; attached file is a provisional approval; Ashok Residency has a claimed final NOC but not yet uploaded."
- Expected tracker outcome: "Solace Park: 3.3 ⚠️ Flagged; 8.1 ⚠️ Flagged; 15.6 may remain ⬜ Open if the OC is not yet audited; Ashok Residency remains Estimated or Unknown until documents arrive."
- Expected verdict: "needs-follow-up; Solace Park should fall behind unless the final NOC is produced."
- Must NOT happen: "must not accept a builder email or a provisional printout as a final fire NOC; must not conclude that the cheaper project is safer without verifying the fire clearance."

### 5) Tower-specific OC mismatch in comparison
- Scenario name & intent: "A project claims a ready-to-move premium but the OC file covers a different tower — comparator should surface the mismatch."
- Inputs: "property type: apartment comparison; locality: Hebbal; projects: Jade Court Living and Crown Crest; docs: Jade Court has Tower A OC but the buyer is comparing Tower C; cost sheet says 'ready to move' as if Tower C were complete; Crown Crest is still under approval."
- Expected tracker outcome: "Jade Court Living Tower C: 2.5 ⚠️ Flagged; 15.6 ⚠️ Flagged; tower-level readiness is not confirmed; Crown Crest remains Estimated or Unknown."
- Expected verdict: "walk-away or needs-follow-up; the project is not safe to rank as ready to move based on a sister tower's OC."
- Must NOT happen: "must not treat a different tower's OC as covering the buyer's unit or the comparison scope; must not call the project ready because the marketing deck says so."
