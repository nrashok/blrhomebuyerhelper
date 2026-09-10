# Land / Plot Due-Diligence Test Cases

### 1) Clean residential plot with valid documents
- Scenario name & intent: "Clean residential plot with complete title chain, BHOMI match, and approved layout — should be sound with no over-flagging."
- Inputs: "property type: plot; locality: Whitefield fringe; survey no: 14/8A; docs: mother deed, 30-year EC, RTC showing current owner, approved layout copy, local authority GIS match, sale deed, no disputes; the layout is a sanctioned residential plot."
- Expected tracker outcome: "1.1 ✅ for deed chain; 1.2 ✅ for EC; 1.5 ✅ for RTC and current ownership; 4.1 ✅ for approved layout; 3.1 ✅ Surveyor confirms actual boundaries; 12.2 ✅ after registration ideally, but pre-registration remains ⬜ Open if not yet registered."
- Expected verdict: "sound; no Walk-away trigger."
- Must NOT happen: "must not accept a marketing plan as proof of approved layout; must not close the title chain without a full deed search."

### 2) B-Khata / loan-ready trap
- Scenario name & intent: "The seller insists the plot is 'loan-ready' on a B-Khata or unconverted site — item 1.6 (Khata status) and the classification items must be Flagged."
- Inputs: "property type: plot; locality: Kengeri; survey no: 43/5B; docs: "loan-ready" claim from seller, B-Khata entry, RTC showing a non-residential status, no DC conversion, sale deed references a development area but no conversion order."
- Expected tracker outcome: "1.6 ⚠️ Flagged — B-Khata confirmed on e-Aasthi, the primary loan/resale-restriction signal; 2.2 ⚠️ Flagged for missing DC conversion; 2.3 ⚠️ Flagged for classification; 1.4 ⚠️ Flagged if assigned or non-convertible status is present; 10.1 ⚠️ Flagged if the sale consideration is understated."
- Expected verdict: "walk-away; Walk-away trigger fires because the land classification is not clean."
- Must NOT happen: "must not treat 'loan-ready' as a substitute for conversion or title status; must not ignore the risk because a lender verbally said it qualifies."

### 3) PTCL granted land — title void risk
- Scenario name & intent: "A PTCL granted plot is sold without a clear non-alienation condition review — title-risk should be Flagged and hard-stop."
- Inputs: "property type: plot; locality: Tumkur Road; survey no: 66/2; docs: grant deed mentions PTCL (SC/ST grant), non-alienation condition, mother deed on the grant, seller says 'it was sold long ago and clean now'; no legal opinion or mutation papers."
- Expected tracker outcome: "1.4 ⚠️ Flagged because land status is restricted; 1.6 ⚠️ Flagged if GPA or transfer chain is incomplete; 2.1 ⚠️ Flagged for grant/title-chain risk; 4.6 ⚠️ Flagged until the authority confirms the transfer status."
- Expected verdict: "walk-away; title-void risk is material."
- Must NOT happen: "must not treat an old sale deed as curing a PTCL grant with a non-alienation condition; must not ignore the grant classification because the seller has been paying tax for years."

### 4) Revenue / unapproved layout
- Scenario name & intent: "No BDA/BMRDA/BIAPPA sanction or layout approval — should be flagged as a layout-risk and potential land-use failure."
- Inputs: "property type: plot; locality: Yelahanka; survey no: 99/4; docs: brochure says 'approved township'; no local authority layout approval, no K-RERA registration, no open-space plan or drainage map; sale agreement cites a survey number but not the exact layout sanction."
- Expected tracker outcome: "4.1 ⚠️ Flagged; 4.2 ⚠️ Flagged because open-space or park reservation is not verifiable; 4.3 ⬜ Open if K-RERA is not required; 6.1 ⚠️ Flagged because the internal roads are clearly not laid to the stated standard."
- Expected verdict: "walk-away or needs-follow-up; serious land-use and approval risk."
- Must NOT happen: "must not accept the developer's brochure or the marketing narrative as proof of a sanctioned layout; must not assume a plot is saleable just because some units were sold already."

### 5) Gramathana site that is actually agricultural
- Scenario name & intent: "Form 9/11 is claimed but the survey extract shows the parcel outside abadi and remains agricultural — should be Flagged immediately."
- Inputs: "property type: plot; locality: Nelamangala outskirts; survey no: 88/12; docs: seller claims 'gramathana / form 9/11'; survey extract says outside abadi; no conversion order; layout brochure calls it a premium residential plot."
- Expected tracker outcome: "2.3 ⚠️ Flagged; 2.5 ⚠️ Flagged; 3.1 ✅ if the surveyor confirms the actual boundary but does not cure the classification; 4.4 ⚠️ Flagged for sensitive parcel classification and local restrictions; 5.2 ⚠️ Flagged if historical imagery shows low-lying or lake-adjacent risk."
- Expected verdict: "walk-away; the agricultural and gramathana mismatch is material."
- Must NOT happen: "must not let a seller's Form 9/11 claim override the actual survey extract; must not neglect the land-classification check because the plot is in a gated layout."

### 6) Right-of-way / landlocked parcel
- Scenario name & intent: "The plot appears saleable but lacks a legal right-of-way — a landlocked parcel should be treated as a hard stop."
- Inputs: "property type: plot; locality: Hosur Road fringe; survey no: 21/9C; docs: sale deed shows extents and boundaries, but no recorded access route; adjoining parcels are privately owned; no easement or access document; buyer has not seen a legal road access."
- Expected tracker outcome: "7.1 ⚠️ Flagged; 7.2 ⚠️ Flagged; 3.2 ⚠️ Flagged if the boundary walk shows no legal approach; 11.1 may stay ⬜ Open until the deed confirms exact frontage, but access is still the main risk."
- Expected verdict: "walk-away; without a legal access path, value and marketability collapse."
- Must NOT happen: "must not accept the seller's statement that 'access exists by a local road' as proof of a legal right-of-way; must not call it sound just because the site is near a main highway."
