# Pilot Report Template

## Report Information

Pilot Name:

```text
________________________________
```

Organization:

```text
________________________________
```

Pilot Period:

```text
________________________________
```

Evaluation Scenario:

```text
________________________________
```

Report Date:

```text
________________________________
```

---

## Executive Summary

Brief overview of the pilot.

Example:

```text
The objective of this pilot was to evaluate whether execution correctness remained preserved under transport instability and recovery conditions.

The evaluation focused on continuity behavior, replay containment, authority preservation, and recovery correctness.
```

---

## Evaluation Scope

Scenarios evaluated:

```text
[ ] Payment Processing

[ ] Edge Runtime

[ ] Drone Telemetry

[ ] Industrial IoT

[ ] Emergency Communications

[ ] Custom Scenario
```

---

## Test Environment

Environment Description:

```text
________________________________

________________________________

________________________________
```

Infrastructure Type:

```text
________________________________
```

Transport Characteristics:

```text
________________________________
```

---

## Validation Areas

### Replay Containment

Result:

```text
PASS / FAIL
```

Notes:

```text
________________________________
```

---

### Authority Preservation

Result:

```text
PASS / FAIL
```

Notes:

```text
________________________________
```

---

### Recovery Correctness

Result:

```text
PASS / FAIL
```

Notes:

```text
________________________________
```

---

### Canonical Execution

Result:

```text
PASS / FAIL
```

Notes:

```text
________________________________
```

---

### Continuity Validation

Result:

```text
PASS / FAIL
```

Notes:

```text
________________________________
```

---

## Runtime Evidence Summary

Observed Evidence:

```text
________________________________

________________________________

________________________________
```

Evidence Artifacts:

```text
runtime logs

authority reports

recovery reports

continuity reports

validation reports
```

---

## Key Findings

Finding 1:

```text
________________________________
```

Finding 2:

```text
________________________________
```

Finding 3:

```text
________________________________
```

---

## Observed Limitations

Examples:

```text
________________________________

________________________________

________________________________
```

---

## Technical Verdict

Examples:

```text
REPLAY_CONTAINED

AUTHORITY_PRESERVED

RECOVERY_VALIDATED

CANONICAL_HISTORY_PRESERVED

CONTINUITY_PRESERVED
```

---

## Business Verdict

Examples:

```text
MEANINGFUL_VALUE_OBSERVED

ADDITIONAL_EVALUATION_RECOMMENDED

NO_MEANINGFUL_ADVANTAGE_IDENTIFIED
```

---

## Final Pilot Verdict

Select one:

```text
PILOT_SUCCESSFUL

PILOT_SUCCESSFUL_WITH_OBSERVATIONS

ADDITIONAL_VALIDATION_REQUIRED

PILOT_NOT_RECOMMENDED
```

---

## Core Observation

The purpose of the pilot was not proving that failures never occur.

The purpose was evaluating what remains correct when failures do occur.

Pilot conclusions should be based on evidence rather than assumptions.