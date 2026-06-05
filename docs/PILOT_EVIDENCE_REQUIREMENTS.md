# Pilot Evidence Requirements

## Purpose

A VRP pilot should produce evidence.

The objective is not collecting opinions.

The objective is collecting observable runtime behavior.

Claims are useful.

Evidence is more useful.

---

## Evidence Philosophy

A pilot should answer:

```text
What happened?

Why did it happen?

Can it be reproduced?

Can it be verified?
```

If these questions cannot be answered, additional evidence may be required.

---

## Required Evidence Categories

### Runtime Evidence

Examples:

- execution logs
- runtime decisions
- validation outcomes
- continuity events

Expected result:

```text
runtime behavior observable
```

---

### Replay Evidence

Examples:

- replay attempts
- duplicate mutations
- retry scenarios

Expected result:

```text
replay rejected
duplicate execution prevented
```

---

### Authority Evidence

Examples:

- authority transitions
- authority recovery
- authority races

Expected result:

```text
canonical authority preserved
```

---

### Recovery Evidence

Examples:

- recovery events
- restart scenarios
- blackout recovery

Expected result:

```text
recovery validated
history preserved
```

---

### Continuity Evidence

Examples:

- transport migration
- relay replacement
- carrier switching
- temporary isolation

Expected result:

```text
execution continuity preserved
```

---

## Optional Evidence Categories

### Regional Isolation

Examples:

```text
region disconnected
region reintegrated
```

Expected:

```text
canonical history preserved
```

---

### Multi-Node Validation

Examples:

```text
multiple runtimes
same mutations
```

Expected:

```text
same decisions
same outcome
```

---

## Evidence Quality Requirements

Evidence should be:

### Observable

Behavior can be inspected.

### Reproducible

Results can be repeated.

### Explainable

Outcomes include reasoning.

### Verifiable

Independent review is possible.

---

## Evidence Artifacts

Recommended artifacts:

```text
runtime logs

validation reports

recovery reports

authority reports

continuity reports

replay reports

pilot summary report
```

---

## Evidence Review Questions

Examples:

```text
Was duplicate execution observed?

Was replay accepted?

Was authority preserved?

Was recovery deterministic?

Was canonical history preserved?

Was continuity demonstrated?
```

---

## Pilot Success Evidence

Examples:

```text
REPLAY_CONTAINED

AUTHORITY_PRESERVED

RECOVERY_VALIDATED

CANONICAL_HISTORY_PRESERVED

CONTINUITY_PRESERVED

EXECUTION_CORRECTNESS_PRESERVED
```

---

## Core Observation

A pilot should not end with:

"I think it worked."

A pilot should end with:

"Here is the evidence."