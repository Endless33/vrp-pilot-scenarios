# Pilot Admission Criteria

## Purpose

VRP pilot evaluations are conducted on a selective basis.

The objective is not maximizing the number of pilots.

The objective is identifying environments where continuity-oriented execution can be meaningfully evaluated.

Not every workload requires VRP.

Not every infrastructure problem is a continuity problem.

---

## Admission Philosophy

A pilot should answer a real technical question.

Examples:

```text
Can execution survive transport instability?

Can recovery remain deterministic?

Can authority remain canonical?

Can replay be contained?

Can continuity be validated?
```

If these questions are not relevant, a pilot may not provide meaningful value.

---

## Candidate Environments

Examples of environments that may be suitable:

- distributed systems
- industrial infrastructure
- edge computing
- critical communication systems
- recovery-sensitive systems
- authority-sensitive systems
- continuity-sensitive workloads

---

## Technical Requirements

At least one of the following should be important:

### Recovery Correctness

```text
YES / NO
```

---

### Replay Containment

```text
YES / NO
```

---

### Authority Preservation

```text
YES / NO
```

---

### Canonical Execution

```text
YES / NO
```

---

### Deterministic Recovery

```text
YES / NO
```

---

### Transport Migration

```text
YES / NO
```

---

### Regional Isolation

```text
YES / NO
```

---

### Blackout Recovery

```text
YES / NO
```

---

## Environments Less Likely To Benefit

Examples:

- static websites
- file hosting
- content delivery
- simple request/response applications
- low-risk internal tools
- systems with no continuity requirements

A pilot may still be possible, but expected value may be limited.

---

## Evidence Expectations

Organizations participating in a pilot should be willing to evaluate:

- runtime evidence
- validation reports
- recovery behavior
- authority behavior
- replay behavior
- continuity outcomes

The objective is observation and validation.

Not marketing.

---

## Pilot Outcomes

A pilot may result in:

```text
TECHNICAL_FIT_CONFIRMED
```

or

```text
NO_MEANINGFUL_ADVANTAGE_IDENTIFIED
```

Both outcomes are acceptable.

---

## Admission Factors

Potential factors include:

- technical relevance
- evaluation goals
- infrastructure characteristics
- continuity requirements
- recovery requirements
- operational constraints

Admission is determined on a case-by-case basis.

---

## Core Observation

The purpose of a pilot is not proving that VRP should be used everywhere.

The purpose is determining whether continuity-oriented execution provides measurable value for a specific environment.

Not every environment is a fit.

That is expected.

---

## Final Principle

Pilot participation is not determined by company size.

Pilot participation is determined by technical relevance.

The best pilot candidate is not necessarily the largest organization.

The best pilot candidate is the one asking the right questions.