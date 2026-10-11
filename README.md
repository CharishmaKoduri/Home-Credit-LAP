# Home Credit LAP Eligibility Voice Agent

A Bolna AI Agent Studio project for preliminary Loan Against Property (LAP) eligibility screening, disqualification handling, and routing eligible or existing-loan customers to the appropriate specialist.

> This is a demonstration project. It is not an official Home Credit product description and does not provide credit decisions, rates, or loan approval.

## What the agent is designed to do
- Verify the intended customer and ask whether it is a suitable time to speak.
- Explain the LAP offer as up to ₹75 lakh, subject to eligibility.
- Collect the seven preliminary screening items: property type, ownership, original property documents, requested loan amount, occupation/income mode, estimated property market value, and requested tenure.
- Stop screening for disqualifying conditions such as agricultural property, unavailable original documents, or cash-only income.
- For an existing property loan or EMI-reduction request, route to a loan-transfer specialist and end the current screening flow.
- Ask only for missing or unclear details, use the latest clear correction, and avoid inventing rates, fees, or approval outcomes.
- After a positive preliminary screen, state that a senior loan expert will follow up; this is not final approval.

## Repository contents
- `prompts/system_prompt.md` — agent instructions and guardrails.
- `docs/architecture.md` — conversation workflow and decision logic.
- `docs/test-results-summary.md` — notes on available call records and evaluation limitations.
- `tests/test_cases.csv` — 50 planned test scenarios.
- `tests/test_results.csv` — 50 call-record metadata rows from the updated export. These are marked **Review required** until each is checked against the original transcript/recording.

## Test evidence and limitations
The latest supplied call-record export contains 50 rows. The public results file omits phone numbers, raw transcripts, and recording URLs. Scenario labels are heuristic hints only, not verified pass/fail outcomes. Please do not interpret `Review required` as a pass. Review each call in the authorized Bolna workspace and update the result only after checking the evidence.

A screen recording and the live agent link are provided separately in the assignment submission, as requested. They are intentionally not duplicated in this repository.

## Privacy
Do not commit raw call exports, customer phone numbers, unrestricted recording URLs, credentials, API keys, or unredacted transcripts. Only share recordings/transcripts through an approved access-controlled channel and where you have authorization.

## Suggested review order
1. Read the system prompt.
2. Review the architecture.
3. Inspect the 50 planned cases.
4. Review the 50 call-reference rows and verify outcomes in Bolna.
5. Open the separately submitted agent link and screen recording.
