# Pilot Success Criteria

## Purpose

This document defines objective criteria for evaluating a VRP pilot.

The goal is not proving that networks never fail.

The goal is evaluating whether execution correctness remains preserved when networks do fail.

---

## Evaluation Philosophy

A successful pilot is not measured by uptime alone.

A successful pilot is measured by observable correctness behavior under instability.

Questions include:

```text
Did execution remain canonical?

Did replay attempts mutate state?

Did authority remain valid?

Did recovery preserve correctness?

Did independent runtimes converge?
```

---

## Minimum Success Requirements

### Replay Containment

Replay attempts must not produce duplicate execution.

Expected:

```text
first mutation accepted
duplicate mutation rejected
state changes once
```

---

### Canonical Execution

One logical mutation must produce at most one canonical commit.

Expected:

```text
single commit
deterministic result
consistent history
```

---

### Recovery Correctness

Recovery should preserve correctness.

Expected:

```text
authority validated
history validated
recovery admitted
execution preserved
```

---

### Authority Preservation

Stale authority must not become canonical.

Expected:

```text
authority rollback rejected
canonical authority preserved
```

---

### Deterministic Convergence

Independent runtimes should reach equivalent outcomes.

Expected:

```text
same input
same verdict
same committed result
```

---

## Advanced Success Requirements

### Transport Migration

Expected:

```text
transport replaced
execution preserved
session identity preserved
```

---

### Regional Isolation

Expected:

```text
isolation tolerated
reintegration validated
canonical history preserved
```

---

### Blackout Recovery

Expected:

```text
multiple recovery candidates
single canonical winner
deterministic recovery
```

---

## Evidence Requirements

Recommended artifacts:

- runtime logs
- recovery logs
- authority reports
- replay reports
- continuity reports
- validation reports

Evidence should be reproducible.

---

## Pilot Failure Indicators

Examples:

```text
duplicate execution observed

replay accepted

authority rollback admitted

history divergence unresolved

recovery corruption detected

non-deterministic outcomes observed
```

Any of these require investigation.

---

## Recommended Evaluation Window

Suggested duration:

```text
1 day
3 days
7 days
14 days
```

Depending on infrastructure complexity.

---

## Pilot Completion Verdict

### Successful

```text
EXECUTION_CORRECTNESS_PRESERVED
AUTHORITY_PRESERVED
RECOVERY_VALIDATED
CANONICAL_HISTORY_PRESERVED
```

---

### Unsuccessful

```text
CORRECTNESS_NOT_DEMONSTRATED
ADDITIONAL_VALIDATION_REQUIRED
```

---

## Core Observation

The purpose of a pilot is not proving that failures never occur.

The purpose of a pilot is understanding what remains correct when they do.

A successful pilot demonstrates correctness under instability.