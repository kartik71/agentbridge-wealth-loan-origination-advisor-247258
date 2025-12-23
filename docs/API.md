# API Documentation

## Endpoints
### Case Intake
- **Description**: Collect, validate and normalize exposure limits from Case Management; attach a runId and timestamp for traceability.
- **Type**: Processing

### Draft
- **Description**: Execute draft phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Self-Critique
- **Description**: Execute self-critique phase for the Reflection pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Limit Control
- **Description**: Limit Control across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Portfolio Check
- **Description**: Portfolio Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Case Management
- **Description**: Case Management across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Sanctions Screening
- **Description**: Sanctions Screening across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Underwriting
- **Description**: Underwriting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Break Resolution
- **Description**: Break Resolution across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Booking
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to CRM; return response JSON for the client.
- **Type**: Processing
