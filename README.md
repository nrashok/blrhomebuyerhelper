# Bengaluru / Karnataka Property Due-Diligence & Home-Buying Skills

Public skill pack for Bengaluru/Karnataka home-buying due diligence, covering apartments, villas, land/plot checks, and project comparison for residential property buyers in Karnataka.

Claude Skills that turn a Bengaluru/Karnataka property due-diligence checklist into an interactive verification session: describe the property, upload documents as you collect them (K-RERA certificate, sale agreement, cost sheet, encumbrance certificate, khata, layout approval, brochure, and so on), and Claude cross-checks each one against the full checklist — tracking every item as **Verified**, **Flagged**, or **Open**, and refining that tracker as more documents arrive.

Due diligence for Bengaluru/Karnataka real estate is scattered across many portals — K-RERA, Bhoomi, e-Aasthi/e-Khata, BBMP, BDA/BMRDA, BIAPPA, BMICAPA, MUDA, KHB, KIADB, BESCOM, BWSSB, KSPCB, Karnataka Fire, AAI NOCAS, Kaveri (Kaveri 2.0), and sub-registrar records — with no single list of what to check and where to check it. These checklists and skills exist to close that gap.


> **⚠️ Disclaimer:** This is a weekend hobby project, not a professional or commercial product. It's provided for informational/educational purposes only, with **no warranty of any kind**, and it is **not** legal, financial, engineering, surveying, or investment advice. It does not replace an independent lawyer, structural engineer/surveyor, or chartered accountant, and nothing it outputs is a legal or professional clearance of any property or document. Use entirely at your own risk — see [Disclaimer](#disclaimer) below for the full terms.

## What's included

| Skill | Covers | Sections | Items |
|---|---|---|---|
| [`apartment-due-diligence-verifier`](skills/apartment-due-diligence-verifier/SKILL.md) | Apartments / flats in a tower or phase | 16 | 114 |
| [`villa-due-diligence-verifier`](skills/villa-due-diligence-verifier/SKILL.md) | Villas / independent houses in a gated community or plotted layout | 15 | 108 |
| [`land-plot-due-diligence-verifier`](skills/land-plot-due-diligence-verifier/SKILL.md) | Land parcels and residential plots (individual resale or organized plotted layouts) | 13 | 73 |
| [`apartment-project-comparator`](skills/apartment-project-comparator/SKILL.md) | Side-by-side comparison of two or more specific apartment projects | 16 (embedded) | 114 (embedded) |

Each checklist item carries a **Verify via** annotation naming exactly where to get supporting proof: the builder/seller, K-RERA, a named Karnataka government portal or office (Bhoomi, e-Aasthi/e-Khata, BBMP, BDA/BMRDA, BIAPPA, BMICAPA, MUDA, KHB, KIADB, BESCOM, BWSSB, KSPCB, Karnataka Fire & Emergency Services, AAI NOCAS, Kaveri (Kaveri 2.0), and others), your lender, public court/company records, an independent third-party professional (lawyer, structural engineer, surveyor, CA), or a personal site visit.

## Karnataka / Bengaluru portals used in these checklists

The skill set references the most common public-facing portals used in Bengaluru/Karnataka due diligence. Always cross-check the exact official portal and current procedure, because authorities can change URLs and workflows.

- K-RERA: https://k-rera.karnataka.gov.in or official K-RERA portal for the current year
- Karnataka Bhoomi / RTC / land records: https://landrecords.karnataka.gov.in
- e-Aasthi / e-Khata / BBMP property records: https://bbmpeaasthi.karnataka.gov.in
- BBMP / GBA / property tax / online services: https://bbmp.gov.in and official BBMP/GBA services
- BDA / BMRDA / layout approvals: relevant authority portals for the parcel or project
- MUDA / KHB / KIADB / other development authorities: official authority portals by district/locality
- BESCOM: https://bescom.karnataka.gov.in or the official BESCOM service-area portal
- BWSSB: https://bwssb.karnataka.gov.in
- KSPCB: https://kspcb.karnataka.gov.in
- Karnataka Fire & Emergency Services: https://fire.karnataka.gov.in
- AAI NOCAS: https://nocas.aai.aero
- Kaveri Online Services (Kaveri 2.0): https://kaverionline.karnataka.gov.in
- BIAPPA / BMICAPA: relevant planning-authority portals for the parcel or project in the airport corridor / north-Bengaluru influence area
- MCA: https://www.mca.gov.in/

> Verification date for the portal list above: 2026-09-10. Some portal names and URLs shift over time; treat this list as a current working reference, not a legal directory.

## How the skills work

The three single-project due-diligence skills follow the same model:

1. **Starting a session** — Claude gathers the property's identifying details (project/survey number, phase or transaction type, K-RERA number) and asks what documents you already have.
2. **Findings Tracker** — a running, per-item table keyed to the checklist's section/item numbering (e.g. `3.2`, `14.5`), with a Status, supporting Evidence, and a Note. Nothing is marked Verified from marketing language alone — only from an actual document or a live portal check.
3. **Iterative refinement** — as you upload more documents, Claude updates the tracker incrementally, calls out any conflicts between documents instead of silently picking one, and flags items that can only ever be closed by a physical site visit.
4. **A final report** — on request, Claude produces a structured due-diligence report: a headline verdict, a section-by-section walkthrough, and a close-out list of what's still needed.

`apartment-project-comparator` works differently: it starts from whatever you already know about each project (a brochure, a price list, a sales pitch) and uses a four-state tracker per project — Confirmed / Estimated / Unknown / Flagged — so it can produce a useful comparison early and get more rigorous only as real documents arrive for a given project. It embeds the same apartment checklist for deepening any one project to full due-diligence rigor.

## Using these skills

These are [Claude Skills](https://docs.claude.com/en/docs/claude-code/skills) — portable instruction sets that a Claude client loads to guide how it handles a task. To use one:

- **Claude Code / Claude Agent SDK**: copy the skill's folder (e.g. `skills/apartment-due-diligence-verifier/`) into your project's or user-level skills directory, or point your skills configuration at this repository.
- **claude.ai (Skills feature, where available)**: create a new skill and paste in the contents of the relevant `SKILL.md`.

Once loaded, start a conversation naming the property you're evaluating and begin sharing documents — the skill takes it from there.

## Publish to skills.sh

To publish this repository as a public skill pack on skills.sh:

1. Make sure the repo is public on GitHub.
2. Keep the skill files in a `skills/` directory, with each skill containing a valid `SKILL.md` file and YAML front matter such as:

```yaml
---
name: apartment-due-diligence-verifier
description: Use when a buyer wants to validate a specific Bengaluru/Karnataka apartment against a due-diligence checklist.
---
```

3. Push the repository to GitHub.
4. Install it with:

```bash
npx skills add nrashok/blrhomebuyerhelper
```

If the command fails on Windows PowerShell because scripts are blocked, first run:

```powershell
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

Then retry the install command above.

This repository is already structured for the expected public skill-pack pattern: a GitHub repo, a root `README.md`, a `LICENSE`, and skill folders under `skills/` with valid `SKILL.md` files.

## Disclaimer

This project was built over a weekend as a personal, hobby exercise — a byproduct of Bengaluru property search — and is shared publicly in case it helps other buyers. It is **not**:

- A commercial product or service. No professional relationship of any kind is created by using it, forking it, or contacting me about it.
- Legal, financial, tax, engineering, surveying, or investment advice.
- A substitute for independent professional review — a licensed property lawyer, a structural engineer or surveyor, and a chartered accountant, as applicable to your situation.
- A guarantee, certification, or legal clearance of any property, document, or transaction. A "Verified" status from these skills means a document was found that matches a checklist item's wording — nothing more, and nothing that should be relied on in place of professional due diligence.

Several checklist items (site visits, physical inspections, live negotiations) can only ever be closed by you, in person — the skills are designed to keep those honestly marked "Open" rather than infer a pass from a document alone.

Regulatory references (K-RERA, Bhoomi, e-Aasthi/e-Khata, BBMP, BDA/BMRDA, BIAPPA, BMICAPA, MUDA, KHB, KIADB, BESCOM, BWSSB, KSPCB, Karnataka Fire, AAI NOCAS, Kaveri (Kaveri 2.0), and other Karnataka/Bengaluru government portals, procedures, and thresholds) reflect my own understanding at the time of writing and may be incomplete, outdated, or inaccurate. Regulations, portal names, and procedures change — verify everything independently against current, authoritative government sources before relying on it for any decision.

This repository and its content are provided **"as is," with no warranty of any kind, express or implied** (see the [LICENSE](LICENSE) for the full legal terms). To the fullest extent permitted by law, I accept no liability for any loss, damage, missed defect, or legal or financial consequence arising from the use of this repository. By using it, you agree you're doing so entirely at your own risk and discretion, and that you will seek qualified professional advice before making any property decision.

If you spot an error, a stale regulation, or an outdated portal reference, please open an issue or a pull request rather than relying on the content as-is.

## Companion checklists

The full checklists these skills are built from also exist as standalone, print-ready reference documents (apartment, villa, and land/plot), covering the same ground in a format suited to printing and manual use rather than conversational, document-by-document verification.

## License

MIT — see [LICENSE](LICENSE). Use, adapt, and share freely.

## Contributing

Issues and pull requests that correct a stale regulation, portal name, or add a missing verification path are welcome.
