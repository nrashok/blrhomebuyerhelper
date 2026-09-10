# Bengaluru / Karnataka Due-Diligence Usage Examples

## Apartment example

Setup line: "Load the apartment skill from skills/apartment-due-diligence-verifier/SKILL.md, then paste this opening prompt: 'I am evaluating Tower B, Unit 1202 in Cedar Crest Residences, Whitefield. Developer: Azure Vale Homes. The project has K-RERA no. KR-1234567890-2025, and I have the K-RERA certificate, sale agreement, cost sheet, and a brochure.'"

User: I am evaluating Tower B, Unit 1202 in Cedar Crest Residences, Whitefield. Developer: Azure Vale Homes. K-RERA no. KR-1234567890-2025. I have the K-RERA certificate, sale agreement, cost sheet, and brochure.
Assistant: I’ll anchor this on Tower B, Unit 1202, not the project as a whole. I can verify the K-RERA and authority records live if web access is available; otherwise I’ll use document review and ask you for the missing items.
User: Here is the K-RERA certificate and cost sheet. The unit is 1,240 sqft carpet; the cost sheet shows a DG backup of 3 kVA per flat.
Assistant: What changed: 3.1 ✅ Verified by the tower-specific K-RERA certificate; 14.1 ✅ Verified, cost sheet itemized the charges; 6.4 ⚠️ Flagged because the DG note is not enough to confirm the actual per-flat backup without the written allocation clause. Highest priority Open: 2.5 tower-specific OC and 3.3 final Fire NOC.
User: I also uploaded the sale agreement and a brochure. The brochure says 'ready to move', but the tower is still under completion.
Assistant: What changed: 14.2 ⚠️ Flagged because the brochure's area claim does not match the sale agreement's annexure; 15.6 ⚠️ Flagged because the project can’t claim ready-to-move status without a tower-specific OC. Highest priority Open: 2.5 OC status and 3.3 final Fire NOC.
User: Can you give me the headline verdict and the close-out list?
Assistant: Headline verdict: needs-follow-up before proceeding. Section counts: 2 critical items are Flagged; 4 items remain Open; the tower-specific OC and final Fire NOC are the highest-risk gaps. Close-out: obtain tower B OC, final Fire NOC, written DG allocation figure, and an independent title/khata check. The remaining site-visit items stay Open until you report back from the site.

> Guardrails: This is a screening aid, not legal advice. Site-visit-only items stay Open until you confirm them. Recommend an independent Karnataka property advocate, a licensed surveyor, and a CA before registration.

## Villa example

Setup line: "Load the villa skill from skills/villa-due-diligence-verifier/SKILL.md, then paste this opening prompt: 'I am buying Villa 14 in Greenstone Courtyard, off Yelahanka Road. Developer: Veda Vista Homes. Plot is in a gated villa community; I have the sale agreement, layout sanction, khata extract, and brochure.'"

User: I am buying Villa 14 in Greenstone Courtyard, off Yelahanka Road. Developer: Veda Vista Homes. I have the sale agreement, layout sanction, khata extract, and brochure.
Assistant: I’ll anchor the review to Villa 14 and the exact layout, and I can live-check Bhoomi, K-RERA, and local authority records if web access is enabled.
User: The brochure says 'approved layout' and 'ready to occupy'. The unit is a villa in a gated community.
Assistant: What changed: 2.5 ✅ Verified for the layout approval; 2.7 ⚠️ Flagged because 'ready to occupy' is not enough without the actual OC; 3.1 ✅ Verified if the project K-RERA certificate is for the exact phase. Highest priority Open: 2.3 conversion status and 2.11 kharab/gramathana checks.
User: I uploaded the khata extract and RTC. There is a DC conversion order in the file, but the RTC still says agricultural use for the parent parcel.
Assistant: What changed: 2.3 ⚠️ Flagged and 2.4 ⚠️ Flagged as a direct conflict between the DC conversion and the RTC; 2.11 ⚠️ Flagged because the same parcel must be checked for kharab/gramathana or lake-buffer exposure. Highest priority Open: a local authority confirmation on conversion and the actual layout sanction for this villa cluster.
User: Please give me the final report.
Assistant: Headline verdict: needs-follow-up before proceeding. Section counts: the title and conversion items are the biggest issue; the approval record is partly clean but the land-use status is not yet resolved. Close-out: obtain the conversion order from the Revenue Department, confirm the exact survey number against the approved layout, and ask the builder for the building-plan approval and OC before final payment.

> Guardrails: This is a screening aid, not legal advice. The land-use record is what matters here, not marketing claims. Recommend an independent Karnataka property advocate, a licensed surveyor, and a CA before taking any final step.

## Land / plot example

Setup line: "Load the land skill from skills/land-plot-due-diligence-verifier/SKILL.md, then paste this opening prompt: 'I am evaluating Plot 42, Survey No. 91/2A, in Kanakapura Road fringe area. Seller says it is a residential plot in a gated layout. I have the mother deed, EC, RTC, and a brochure from the layout.'"

User: I am evaluating Plot 42, Survey No. 91/2A, in Kanakapura Road fringe area. Seller says it is a residential plot in a gated layout. I have the mother deed, EC, RTC, and a brochure from the layout.
Assistant: I’ll anchor everything to survey number 91/2A and verify the title, conversion, and layout status before covering the financial terms. I can check Bhoomi, Kaveri (Kaveri 2.0), and local planning records live if web access is enabled.
User: Here is the mother deed and EC. The seller says 'approved layout'.
Assistant: What changed: 1.1 ✅ Verified for the deed chain; 1.2 ✅ Verified for the 30-year EC; 4.1 ⚠️ Flagged because a brochure's 'approved layout' label is not enough without the exact layout sanction and survey-number match. Highest priority Open: 2.2 DC conversion, 2.3 kharab/gramathana classification, and 4.4 lake/buffer checks.
User: I also uploaded the RTC and the layout sanction. The RTC still shows agricultural status, and there is no DC conversion order.
Assistant: What changed: 2.2 ⚠️ Flagged; 2.3 ⚠️ Flagged; 4.1 ✅ Verified only once the survey number and sanctioned layout match exactly; 4.4 ⚠️ Flagged because the parcel is in a sensitive zone. Highest priority Open: a full revenue-side title review and a surveyor boundary cert.
User: Can you tell me whether this is a walk-away?
Assistant: Headline verdict: walk-away. The plot is still agricultural in the RTC, has no conversion order, and the layout sanction cannot cure a land-classification defect. Close-out: stop the transaction; obtain a local revenue-office clarification, a legal opinion on the PTCL/assigned-land risk, and an independent surveyor report before any further payment or registration.

> Guardrails: This is a screening aid, not legal advice. Land-use and title status are the real risk here, not marketing language. Recommend an independent Karnataka property advocate, a licensed surveyor, and a CA before proceeding.

## Comparator example

Setup line: "Load the apartment comparator from skills/apartment-project-comparator/SKILL.md, then paste this opening prompt: 'I am comparing two 2BHK projects in North Bengaluru: Aster Park in Yelahanka and Magnolia Crest in Hebbal. I only have brochures and price lists so far.'"

User: I am comparing two 2BHK projects in North Bengaluru: Aster Park in Yelahanka and Magnolia Crest in Hebbal. I only have brochures and price lists so far.
Assistant: I’ll use the four-state model for each project: Confirmed, Estimated, Unknown, or Flagged. Right now, all price and area numbers are estimated from marketing material unless you upload a document or a live portal check.
User: The brochures show Aster Park at 1,060 sqft carpet, Rs. 8,250/sqft, and Magnolia at 1,180 sqft carpet, Rs. 7,800/sqft.
Assistant: What changed: Aster Park and Magnolia Crest both moved to Estimated on price/sqft and configuration; no project is Confirmed on finished area because a brochure is not a legal measurement. Highest priority Unknown: K-RERA registration, tower-specific OC, and any delay-penalty clause.
User: I uploaded the K-RERA cert and cost sheet for Aster Park, and only a brochure for Magnolia.
Assistant: What changed: Aster Park moved from Estimated to Confirmed on builder identity and K-RERA registration number; 14.1 on Aster Park is Confirmed due to the cost sheet; Magnolia remains Estimated on price and area because the brochure alone cannot verify those values. Highest priority Open for Magnolia: K-RERA registration, tower-specific OC, and the actual layout/approval status.
User: Which project should I deepen first?
Assistant: Deepen Aster Park first because its K-RERA and price documents are in hand; Magnolia is still too marketing-heavy to rank it as the safer choice. If you upload the Aster Park cost sheet and sale agreement, I can check the exact pricing load and payment terms; if Magnolia uploads its K-RERA and tower-specific approvals, the comparison becomes more decisive.

> Guardrails: This is a screening aid, not legal advice. Marketing language is never proof; it stays Estimated until supported by a document or live portal check. Recommend an independent Karnataka property advocate, a licensed surveyor, and a CA before any final choice.

## Tips

- Anchor every review to the exact tower, unit, survey number, or plot number — not the project brand alone.
- Treat marketing claims as Estimated, never Verified, until a document or live portal check confirms them.
- Get every red-flag item in writing before progressing, especially title, conversion, and approval issues.
- Confirm live portal facts where possible; when a live check conflicts with a document, report both clearly.
