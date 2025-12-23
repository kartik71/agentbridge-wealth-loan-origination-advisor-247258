# Architecture Documentation

## Overview
This Reflection implements Wealth Loan Origination Advisor for Banking & Finance use cases.

## Components
1. **Case Intake**: Collect, validate and normalize exposure limits from Case Management; attach a runId and timestamp for traceability.
2. **Draft**: Execute draft phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Self-Critique**: Execute self-critique phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Limit Control**: Limit Control across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Portfolio Check**: Portfolio Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Case Management**: Case Management across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Sanctions Screening**: Sanctions Screening across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Underwriting**: Underwriting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
9. **Break Resolution**: Break Resolution across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
10. **Booking**: Assemble final payload with status, artifacts, KPIs and audit trail; store to CRM; return response JSON for the client.

## Data Flow
- Input: Case Intake
- Processing: 10 sequential steps
- Output: Booking
