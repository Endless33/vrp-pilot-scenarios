# When Not To Use VRP

## Purpose

Not every system requires continuity-oriented execution.

Not every workload benefits from additional correctness controls.

This document identifies situations where a VRP evaluation may provide little or no practical value.

---

## Overview

VRP focuses on execution correctness under instability.

Examples include:

- transport mutation
- replay containment
- authority transitions
- blackout recovery
- deterministic execution
- canonical history preservation

If these concerns are not important, VRP may not be necessary.

---

## Scenario 1

### Simple Stateless APIs

Example:

```text
request
↓
response
↓
complete
```

No meaningful execution state exists.

No recovery complexity exists.

Traditional networking approaches are often sufficient.

---

## Scenario 2

### Static Content Delivery

Examples:

- images
- videos
- downloads
- documentation

The workload primarily concerns delivery.

Execution correctness is not the primary challenge.

---

## Scenario 3

### Short-Lived Sessions

Examples:

```text
open session
perform action
close session
```

Session continuity is not important.

Transport loss simply ends the interaction.

---

## Scenario 4

### Environments With No Recovery Requirements

If infrastructure failures are acceptable and recovery correctness is not important:

```text
restart
reconnect
continue
```

Additional continuity controls may provide limited value.

---

## Scenario 5

### Systems Without Authority Concerns

If no canonical authority exists:

```text
single process
single node
single owner
```

Authority preservation may not be relevant.

---

## Scenario 6

### Workloads That Tolerate Duplicate Execution

If duplicate execution is harmless:

```text
duplicate event
↓
no consequence
```

Replay containment may not justify additional complexity.

---

## Questions To Ask

Would duplicate execution matter?

Would stale authority matter?

Would incorrect recovery matter?

Would canonical history matter?

Would transport instability create operational risk?

If most answers are NO:

```text
VRP may not be necessary.
```

---

## Examples Where VRP May Not Add Significant Value

- static websites
- file downloads
- content delivery
- simple request/response services
- short-lived interactive sessions
- low-risk internal tools

---

## Examples Where Evaluation May Be Worthwhile

- financial systems
- industrial control
- edge infrastructure
- distributed runtimes
- continuity-sensitive systems
- recovery-sensitive environments

---

## Core Observation

A technology does not need to solve every problem.

The goal is identifying where it provides measurable value.

Sometimes the correct answer is:

```text
Do not use VRP.
```

That answer is perfectly acceptable.