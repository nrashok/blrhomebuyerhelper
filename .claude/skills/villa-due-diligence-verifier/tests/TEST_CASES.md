# Villa Due-Diligence Test Cases

### 1) Clean villa with valid layout and title
- Scenario name & intent: "Clean villa with valid layout approval and K-RERA project record — sound outcome with no over-flagging."
- Inputs: "property type: villa; locality: Devanahalli; developer: Veda Vista Homes; villa: 14; docs: sale agreement, RC copy, layout sanction, khata extract, K-RERA certificate, final fire NOC, water and drainage plan; no discrepancy between records."
- Expected tracker outcome: "2.5 ✅ for approved layout; 2.7 ✅ for OC where claimed; 3.1 ✅ for K-RERA; 3.3 ✅ for Fire NOC; 13.1 ✅ for cost sheet; 15.1 ⬜ Open until the buyer actually visits the site."
- Expected verdict: "sound; no Walk-away trigger."
- Must NOT happen: "must not mark the villa as sound based on the brochure alone; must not ignore the site-visit requirement for 15.1–15.5."

### 2) Unconverted agricultural land sold as a villa site
- Scenario name & intent: "Agricultural land sold as a villa/plot without conversion — land status should be Flagged and the verdict should stop the deal."
- Inputs: "property type: villa; locality: Kanakapura; developer: Palaru Meadows; villa: 7; docs: sale agreement, RTC still agricultural, no DC conversion order, khata still reflects agricultural status, brochure calls it 'premium villa community'."
- Expected tracker outcome: "2.3 ⚠️ Flagged; 2.4 ⚠️ Flagged because RTC and sale deed do not align with residential use; 2.11 ⚠️ Flagged for kharab/gramathana risk; 5.1 remains ⬜ Open until a geotechnical and structural review is provided."
- Expected verdict: "walk-away; Walk-away trigger fires due to unconverted agricultural land and title risk."
- Must NOT happen: "must not allow the community brochure to override the conversion record; must not ignore the agricultural status because the builder says it is 'already approved'."

### 3) Revenue / unapproved layout risk
- Scenario name & intent: "No BDA/BMRDA/MUDA sanction for the villa cluster — failure to approve the layout should be treated as a serious risk."
- Inputs: "property type: villa; locality: Kengeri; developer: Lakshmi Peak Villas; docs: sale agreement, brochure as 'exclusive township', no approved layout copy, RTC and khata show an unapproved layout record, no authority plan number supplied."
- Expected tracker outcome: "2.5 ⚠️ Flagged; 2.11 ⚠️ Flagged because the layout status is unresolved; 3.1 may be ⬜ Open or ⚠️ Flagged if the project isn't registered; 13.1 may show the financials but the legal status is not clean."
- Expected verdict: "walk-away; a layout without local authority sanction is a strong stop."
- Must NOT happen: "must not confuse a brochure's 'gated community' claim with legal approval; must not accept a layout as valid because the developer has sold several units already."

### 4) Gramathana site that's actually agricultural
- Scenario name & intent: "Form 9/11 is claimed but survey extract shows the parcel is outside the abadi and remains agricultural — land class must be Flagged."
- Inputs: "property type: villa; locality: Nelamangala; developer: Ganga Lila Homes; docs: Form 9/11 claim, survey extract showing outside abadi, sale agreement for a villa plot, no conversion order, local authority says the parcel falls under agricultural record."
- Expected tracker outcome: "2.3 ⚠️ Flagged; 2.4 ⚠️ Flagged; 2.11 ⚠️ Flagged; 3.5 ⚠️ Flagged if the site is mapped as a sensitive or non-residential parcel; 15.1 remains ⬜ Open because the site visit has not happened."
- Expected verdict: "walk-away; land classification issue is too material."
- Must NOT happen: "must not accept Form 9/11 or a builder's certificate as proof of residential status; must not silently prefer the newer document over the survey extract."

### 5) Site-visit-only items stay Open
- Scenario name & intent: "The paperwork is nicely organized, but the buyer has not visited — drainage, water pressure, and security items must remain Open."
- Inputs: "property type: villa; locality: East Bengaluru; developer: Saanvya Villas; docs: layout approval, khata, sale agreement, builder maintenance agreement, brochure; no on-site observations or walk-through yet."
- Expected tracker outcome: "15.1 ⬜ Open; 15.2 ⬜ Open; 7.6 ⬜ Open; 12.3 ⬜ Open; 4.2 ⬜ Open until the buyer checks monsoon waterlogging; 6.5 ⬜ Open until BESCOM sanction is reviewed."
- Expected verdict: "needs-follow-up; not sound until a direct visit confirms quality and access."
- Must NOT happen: "must not infer full site adequacy from approved plans, khata, or sale agreement alone; must not mark a site-visit item as Verified without a site report."
