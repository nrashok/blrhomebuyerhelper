# Apartment Due-Diligence Test Cases

### 1) Clean A-Khata apartment — sound
- Scenario name & intent: "Clean A-Khata apartment — valid e-Khata, tower-specific OC, live K-RERA number, final Fire NOC -> verdict sound, no over-flagging."
- Inputs: "property type: apartment; locality: Whitefield; developer: Azure Vale Homes; tower: B; unit: 1202; docs: e-Khata, tower B OC, K-RERA cert, final fire NOC, cost sheet, sale agreement; brochure says 'ready to move' only after approval checks."
- Expected tracker outcome: "2.7 ✅ for khata/conversion status; 2.5 ✅ for Tower B OC; 3.1 ✅ for K-RERA registration; 3.3 ✅ for final Fire NOC; 14.1 ✅ for cost breakdown; 16.1 ⬜ Open only until buyer does the site visit; no item should be ⚠️."
- Expected verdict: "sound; no Walk-away trigger; no over-flagging."
- Must NOT happen: "must not mark the project as ready to move from the brochure alone; must not infer a clean file from a sister tower's OC or a provisional fire NOC."

### 2) B-Khata site sold as 'loan-ready' — red flag
- Scenario name & intent: "B-Khata site sold as 'loan-ready' — Khata item is the trap and should be Flagged with a Walk-away trigger."
- Inputs: "property type: apartment; locality: Yelahanka; developer: Nallur Crest; tower: C; docs: B-Khata, sale agreement, builder letter claiming 'loan-ready'; no e-Khata or conversion record; cost sheet shows nil legal objections."
- Expected tracker outcome: "2.7 ⚠️ Flagged for khata/conversion; 2.3 ⚠️ Flagged if the parcel is on a B-Khata / non-converted site; 14.1 ⚠️ Flagged if pricing or loan-readiness is unsupported; 3.1 may remain ✅ if K-RERA is valid, but land title status is still broken."
- Expected verdict: "needs-follow-up or walk-away; Walk-away trigger fires because the land status is not valid for clean residential use."
- Must NOT happen: "must not treat 'loan-ready' as a legal substitute for e-Khata or conversion status; must not ignore the same-site title problem because the builder says lenders are okay."

### 3) Document conflict — brochure area differs from sale agreement
- Scenario name & intent: "Brochure carpet area differs from the sale agreement annexure — conflict should be surfaced without auto-resolving it."
- Inputs: "property type: apartment; locality: Sarjapur; developer: Garuda Heights; tower: A; docs: brochure says carpet area 1,180 sqft; sale agreement annexure says 1,050 sqft; cost sheet uses 1,180 sqft; no final measurement sheet yet."
- Expected tracker outcome: "14.2 ⚠️ Flagged because the area basis is inconsistent; 2.4 and 14.1 may stay ⬜ Open until the approved plan and exact annexure are reconciled; 16.1 remains ⬜ Open since the site visit has not happened."
- Expected verdict: "needs-follow-up; no Walk-away trigger by itself unless the discrepancy is unexplained or tied to title/approval risk."
- Must NOT happen: "must not auto-resolve by preferring the newer document or the brochure; must not mark the area as Verified from marketing language alone."

### 4) Provisional Fire NOC passed off as final
- Scenario name & intent: "A provisional fire approval is passed off as final — the skill should Flag it and trigger the fire-safety walk-away rule."
- Inputs: "property type: apartment; locality: Hoskote; developer: Blue River Towers; tower: D; docs: builder email says 'final NOC obtained'; attached file is a provisional approval dated at plan stage; K-RERA and OC are otherwise clean."
- Expected tracker outcome: "3.3 ⚠️ Flagged because the NOC is provisional, not final; 8.1 ⚠️ Flagged for the same issue; 15.6 remains ⬜ Open if tower-specific OC status is not separately proved."
- Expected verdict: "walk-away or at minimum needs-follow-up; Walk-away trigger fires on fire-safety clearance gap."
- Must NOT happen: "must not accept an approval label from a builder email as proof; must not treat the provisional NOC as a valid final clearance."

### 5) Tower / phase OC mismatch
- Scenario name & intent: "OC is for Tower A, unit is in Tower C — phase mismatch should be a hard red flag."
- Inputs: "property type: apartment; locality: Hebbal; developer: Jade Court Living; tower: C; unit: 706; docs: tower A OC from the authority, sale agreement for tower C, K-RERA cert shows phase-specific towers."
- Expected tracker outcome: "2.5 ⚠️ Flagged because the OC is not specific to Tower C; 15.6 ⚠️ Flagged because possession cannot rely on a different tower's OC; 3.1 may still be ✅ if the tower-specific K-RERA is valid."
- Expected verdict: "walk-away or needs-follow-up; Walk-away trigger fires because possession/approval is not tower-specific."
- Must NOT happen: "must not let the project-level OC cover the unit-level risk; must not assume a sibling tower's approval is enough."

### 6) Site-visit-only item stays Open
- Scenario name & intent: "All documents are uploaded, but the buyer has not visited — lift/water-pressure/crack-inspection/security items remain Open and never get Verified by inference."
- Inputs: "property type: apartment; locality: Marathahalli; developer: Greenfield Vista; tower: E; docs: K-RERA, fire NOC, sale agreement, structural certificates, maintenance agreement; no site visit supplied yet."
- Expected tracker outcome: "16.1 ⬜ Open; 16.2 ⬜ Open; 16.3 ⬜ Open; 13.4 ⬜ Open; 5.9 ⬜ Open until the buyer inspects cracks; 7.3 ⬜ Open until water pressure is tested."
- Expected verdict: "needs-follow-up; no Walk-away trigger unless the buyer is ignoring explicit red flags."
- Must NOT happen: "must not infer that a good set of documents proves lift performance, pump pressure, or security quality; must not close any Self-tagged item from paperwork alone."
