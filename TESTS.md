# Bengaluru / Karnataka Due-Diligence Regression Tests

This suite covers the four Bangalore/Karnataka skill files in this repo and is meant to catch future regressions in the title, approval, and red-flag logic.

## Skill index

- Apartment due diligence: [skills/apartment-due-diligence-verifier/tests/TEST_CASES.md](skills/apartment-due-diligence-verifier/tests/TEST_CASES.md)
- Villa due diligence: [skills/villa-due-diligence-verifier/tests/TEST_CASES.md](skills/villa-due-diligence-verifier/tests/TEST_CASES.md)
- Land / plot due diligence: [skills/land-plot-due-diligence-verifier/tests/TEST_CASES.md](skills/land-plot-due-diligence-verifier/tests/TEST_CASES.md)
- Apartment project comparator: [skills/apartment-project-comparator/tests/TEST_CASES.md](skills/apartment-project-comparator/tests/TEST_CASES.md)

## How to run a case

1. Open the skill file you want to test.
2. Paste the scenario's Inputs into the skill as though the buyer is providing the documents.
3. Compare Claude's tracker to the Expected tracker outcome in the test.
4. Check the final verdict and confirm the Must NOT happen guardrail stays true.
5. If a result is weaker than expected, the case has surfaced a regression in the rule set.

Each scenario below is intentionally synthetic and uses fictional names, survey numbers, plot numbers, RERA numbers, and developer names only.
