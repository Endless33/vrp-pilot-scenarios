# Pilot Evaluation Checklist

## Purpose

This document helps organizations determine whether a VRP pilot evaluation is appropriate.

Not every workload requires continuity-oriented execution.

The objective is to identify environments where execution correctness may be more important than simple connectivity.

---

## Technical Fit

Evaluate the following questions.

### Transport Instability

Does the environment experience:

- network interruptions
- transport migration
- route changes
- relay replacement
- regional isolation

```text
YES / NO
```

---

### Duplicate Execution Risk

Would duplicate execution create operational problems?

Examples:

- payments
- commands
- state mutations
- workflow transitions

```text
YES / NO
```

---

### Recovery Complexity

Does recovery currently depend on:

- reconnect logic
- state reconstruction
- retry loops
- manual reconciliation

```text
YES / NO
```

---

### Authority Sensitivity

Does the system require:

- authority transitions
- leadership changes
- canonical decision selection

```text
YES / NO
```

---

### Deterministic Behavior

Is deterministic execution important?

Examples:

- finance
- industrial systems
- distributed runtimes
- critical infrastructure

```text
YES / NO
```

---

## Evaluation Goals

Select desired outcomes.

```text
[ ] Replay containment

[ ] Authority validation

[ ] Recovery correctness

[ ] Canonical execution

[ ] Transport migration validation

[ ] Blackout recovery validation

[ ] Regional isolation validation

[ ] Continuity validation
```

---

## Success Indicators

Potential indicators include:

```text
duplicate execution prevented

replay attempts rejected

authority rollback rejected

canonical history preserved

deterministic recovery achieved

execution correctness preserved
```

---

## Evidence Collection

Recommended evidence:

- runtime logs
- validation reports
- recovery reports
- replay reports
- authority transition reports
- continuity reports

---

## Pilot Recommendation

If most answers are YES:

```text
VRP pilot may be worth evaluating.
```

If most answers are NO:

```text
Traditional networking approaches may already be sufficient.
```

---

## Core Observation

The goal is not deploying VRP everywhere.

The goal is identifying environments where execution correctness under instability has measurable value.