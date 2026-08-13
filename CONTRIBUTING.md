# Contributing to Java Zenith

> **Java Zenith is a deliberate learning system first, an engineering laboratory second, and a collaborative repository third.**
>
> Contributions are welcome when they strengthen the repository without replacing the learning process that the repository exists to produce.

**Status:** Active  
**Primary Language:** Java 21  
**Primary Framework:** Spring Boot  
**Build System:** Maven  
**Development Environment:** Linux / WSL2  
**Repository Type:** Personal engineering curriculum, laboratory, reference system, and portfolio of implementation work

---

## Table of Contents

- [1. Welcome](#1-welcome)
- [2. What Java Zenith Is](#2-what-java-zenith-is)
- [3. The Core Contribution Principle](#3-the-core-contribution-principle)
- [4. Learning Integrity](#4-learning-integrity)
- [5. Contributor Roles](#5-contributor-roles)
- [6. What Contributions Are Welcome](#6-what-contributions-are-welcome)
- [7. What Contributions Are Restricted](#7-what-contributions-are-restricted)
- [8. The Contribution Hierarchy](#8-the-contribution-hierarchy)
- [9. Before You Contribute](#9-before-you-contribute)
- [10. Issues and Proposals](#10-issues-and-proposals)
- [11. Curriculum Contributions](#11-curriculum-contributions)
- [12. Exercise and Kata Contributions](#12-exercise-and-kata-contributions)
- [13. Laboratory Contributions](#13-laboratory-contributions)
- [14. Project Contributions](#14-project-contributions)
- [15. Documentation Contributions](#15-documentation-contributions)
- [16. Reference Material Contributions](#16-reference-material-contributions)
- [17. Code Standards](#17-code-standards)
- [18. Testing Standards](#18-testing-standards)
- [19. Benchmarking and Performance Work](#19-benchmarking-and-performance-work)
- [20. Dependency Policy](#20-dependency-policy)
- [21. AI-Assisted Contributions](#21-ai-assisted-contributions)
- [22. Git Workflow](#22-git-workflow)
- [23. Commit Standards](#23-commit-standards)
- [24. Pull Requests](#24-pull-requests)
- [25. Review Standards](#25-review-standards)
- [26. Maintainer Authority](#26-maintainer-authority)
- [27. Rejection Criteria](#27-rejection-criteria)
- [28. Conflict Resolution](#28-conflict-resolution)
- [29. Attribution](#29-attribution)
- [30. Security and Sensitive Information](#30-security-and-sensitive-information)
- [31. Contribution Checklist](#31-contribution-checklist)
- [32. Definition of an Accepted Contribution](#32-definition-of-an-accepted-contribution)
- [33. Long-Term Collaboration](#33-long-term-collaboration)
- [34. Final Principle](#34-final-principle)

---

# 1. Welcome

Thank you for taking an interest in **Java Zenith**.

Java Zenith is intentionally different from a conventional open-source software project.

It is not merely an application that happens to contain Java code.

It is a structured record of an engineer learning, experimenting with, and progressively mastering:

```text
Java
 ↓
Object-Oriented Design
 ↓
Collections & Generics
 ↓
Modern Java
 ↓
Testing
 ↓
JVM Internals
 ↓
Concurrency
 ↓
Spring
 ↓
Spring Boot
 ↓
Persistence
 ↓
Security
 ↓
Production Engineering
 ↓
Distributed Systems
```

Because of that, the most important resource in this repository is not its source code.

It is the **learning process behind the source code**.

This document explains how other people can participate in Java Zenith while preserving that process.

---

# 2. What Java Zenith Is

Java Zenith is a:

- personal learning curriculum;
- Java and Spring reference system;
- software engineering laboratory;
- collection of implementation exercises;
- repository of experiments;
- collection of progressively larger projects;
- record of engineering decisions;
- debugging journal;
- performance laboratory;
- and portfolio of practical work.

The repository is organized around several distinct areas:

```text
curriculum/    What is being learned
reference/     What is being consulted
katas/         Focused practice
labs/          Experiments
projects/      Integrated construction
benchmarks/    Measurement
notes/         Understanding and reflection
docs/          Engineering documentation
scripts/       Automation
```

These areas do not have identical contribution rules.

A typo correction in documentation is fundamentally different from contributing a complete solution to a Java exercise.

A benchmark is different from a curriculum change.

A security fix is different from a stylistic refactor.

Contributions must therefore be evaluated according to **purpose**, not merely according to whether the submitted code works.

---

# 3. The Core Contribution Principle

The governing principle of Java Zenith is:

> **Contributions must strengthen the learning system without replacing the learning that the system exists to produce.**

This means a contribution can be technically excellent and still be inappropriate for the repository.

For example, a contributor may submit a sophisticated implementation of an exercise that has not yet been studied.

The implementation may be:

- correct;
- elegant;
- efficient;
- well tested;
- idiomatic;
- and production quality.

It may still be rejected.

Why?

Because the purpose of the exercise is to create an opportunity for the maintainer to solve the problem independently.

In Java Zenith:

```text
Technical correctness
        +
Educational suitability
        +
Architectural consistency
        +
Curriculum alignment
        =
Good contribution
```

Not every technically correct change belongs in the repository.

---

# 4. Learning Integrity

## 4.1 The repository must preserve genuine learning

Java Zenith exists to develop independent engineering ability.

Contributors should therefore avoid doing work that removes the intellectual challenge intentionally built into the curriculum.

The maintainer should be allowed to:

- get stuck;
- make mistakes;
- write inefficient code;
- misunderstand APIs;
- encounter compiler errors;
- encounter runtime failures;
- debug incorrect assumptions;
- redesign solutions;
- benchmark competing approaches;
- and eventually discover the correct solution.

These experiences are not defects in the repository.

They are part of the curriculum.

## 4.2 Do not solve an intentionally unsolved problem

If a topic is currently being learned, do not submit its completed solution unless explicitly requested.

For example:

### Appropriate

> "Your use of `HashMap` here has an interesting consequence. Have you checked how `equals()` and `hashCode()` interact?"

### Also appropriate

> "The official documentation describes this method's contract in a slightly different way. You may want to inspect it."

### Generally inappropriate

> "I implemented the entire exercise for you and opened a PR."

The distinction is simple:

> **Help the learner think. Do not remove the need for the learner to think.**

## 4.3 Hints are different from solutions

Hints can be extremely valuable.

A useful hierarchy is:

```text
Question
 ↓
Hint
 ↓
Documentation reference
 ↓
Conceptual explanation
 ↓
Pseudocode
 ↓
Partial implementation
 ↓
Complete implementation
```

When the learning objective is still active, contributors should prefer the **least revealing intervention that meaningfully helps**.

## 4.4 Completed topics are different

Once a curriculum topic has been completed and the maintainer has demonstrated sufficient understanding, alternative implementations become more appropriate.

At that point, contributions may include:

- alternative algorithms;
- idiomatic Java approaches;
- performance comparisons;
- additional tests;
- alternative API designs;
- refactorings;
- additional exercises.

The important distinction is:

```text
Before mastery:
Protect the challenge.

After mastery:
Expand the understanding.
```

---

# 5. Contributor Roles

Java Zenith does not require everyone who participates to have repository write access.

## 5.1 Observer

An observer:

- reads the repository;
- follows the curriculum;
- provides informal feedback;
- reports obvious issues.

No repository permissions are required.

## 5.2 Peer Collaborator

A peer collaborator may:

- discuss concepts;
- compare implementations;
- review code;
- suggest experiments;
- recommend documentation;
- challenge assumptions;
- propose alternative approaches.

This is the preferred collaboration model during active learning.

A peer collaborator does not need write access.

## 5.3 Contributor

A contributor may submit:

- documentation fixes;
- tests;
- exercises;
- laboratory experiments;
- benchmarks;
- supporting scripts;
- reference corrections;
- approved code changes.

Contributors should follow this document and obtain appropriate approval before making substantial curriculum changes.

## 5.4 Trusted Collaborator

A trusted collaborator is someone who has demonstrated:

- sound technical judgment;
- respect for learning boundaries;
- consistency;
- good communication;
- understanding of repository conventions;
- and responsible Git practices.

Trusted collaborators may eventually receive broader permissions.

Access is earned through demonstrated judgment, not assumed from friendship or technical ability.

## 5.5 Maintainer

The maintainer owns the final direction of Java Zenith.

The maintainer decides:

- curriculum order;
- educational objectives;
- repository architecture;
- accepted dependencies;
- project direction;
- contribution boundaries;
- and whether a contribution belongs in the repository.

---

# 6. What Contributions Are Welcome

The following categories are generally welcome.

## Documentation

- fixing factual errors;
- improving explanations;
- correcting terminology;
- fixing broken links;
- improving examples;
- clarifying confusing instructions;
- improving grammar and spelling.

## Learning resources

- recommending authoritative references;
- identifying useful documentation;
- suggesting books;
- proposing relevant specifications;
- identifying useful technical papers.

## Exercises

- proposing additional exercises;
- adding exercises to completed topics;
- improving exercise descriptions;
- adding edge cases;
- creating independent challenge problems.

## Testing

- additional test cases;
- regression tests;
- edge-case coverage;
- integration tests;
- concurrency tests.

## Experiments

- JVM experiments;
- concurrency experiments;
- collection behavior experiments;
- Spring experiments;
- database experiments;
- performance experiments.

## Benchmarks

- reproducible benchmarks;
- profiling experiments;
- performance comparisons;
- allocation measurements.

## Tooling

- development scripts;
- validation scripts;
- build improvements;
- repository automation.

## Bug reports

Any technically accurate report that helps identify:

- incorrect code;
- broken instructions;
- incorrect documentation;
- unexpected behavior;
- build failures;
- dependency problems;
- or reproducibility problems.

---

# 7. What Contributions Are Restricted

The following require additional consideration.

## 7.1 Unsolicited curriculum rewrites

Do not reorganize the curriculum simply because you prefer another learning order.

The curriculum is intentionally ordered according to conceptual dependencies.

## 7.2 Complete solutions to active exercises

Do not submit completed solutions to exercises that are intentionally unsolved.

## 7.3 Unnecessary abstractions

Do not introduce:

- interfaces without a meaningful reason;
- factories without a meaningful construction problem;
- design patterns merely to demonstrate patterns;
- additional layers merely because production applications sometimes have them.

Java Zenith values:

> **appropriate complexity over impressive complexity.**

## 7.4 Unnecessary dependencies

Do not introduce a library simply because it makes a small task easier.

A dependency should solve a meaningful problem and have an understood cost.

## 7.5 Large changes without discussion

Substantial changes should be proposed before implementation.

This includes:

- curriculum changes;
- architecture changes;
- major project rewrites;
- dependency migrations;
- framework changes;
- repository restructuring.

---

# 8. The Contribution Hierarchy

When proposing a contribution, prefer the smallest intervention that achieves the intended result.

```text
Documentation correction
        ↓
Suggestion
        ↓
Issue
        ↓
Small patch
        ↓
Focused contribution
        ↓
Larger contribution
        ↓
Architectural change
```

The larger the change, the stronger the expectation for prior discussion.

A one-line typo fix does not require a design meeting.

A change to the curriculum architecture probably does.

---

# 9. Before You Contribute

Before making a contribution:

1. Read `README.md`.
2. Read this document.
3. Inspect the relevant directory.
4. Understand the purpose of the existing code.
5. Determine whether the topic is currently active.
6. Check whether an issue or proposal already exists.
7. Avoid duplicating existing work.
8. Consider whether the contribution preserves the learning objective.
9. Ask before making a substantial change.

When in doubt:

> **Ask first.**

---

# 10. Issues and Proposals

Issues are useful for discussing:

- bugs;
- curriculum questions;
- proposed exercises;
- architectural ideas;
- documentation problems;
- resources;
- experiments;
- feature proposals.

A useful issue should explain:

```text
Problem
Context
Observed behavior
Expected behavior
Proposed direction
Open questions
```

For curriculum proposals, additionally explain:

```text
What should be learned?
Why does it belong here?
What prerequisite knowledge does it require?
What practical exercise demonstrates it?
How does it fit the existing progression?
```

---

# 11. Curriculum Contributions

Curriculum changes are among the most sensitive contributions.

The curriculum is not simply a list of technologies.

It represents a deliberate progression of concepts.

A proposed curriculum change should answer:

### What is being added?

Example:

```text
Structured concurrency
```

### Why is it needed?

What engineering capability does it develop?

### Where should it appear?

Which phase and section?

### What are the prerequisites?

What concepts should already be understood?

### How should it be learned?

What combination of:

- theory;
- documentation;
- implementation;
- experimentation;
- testing;
- and project work

will establish understanding?

### How will mastery be demonstrated?

A curriculum change without a mastery mechanism is incomplete.

---

# 12. Exercise and Kata Contributions

Exercises should have a clear educational objective.

A good exercise should answer:

> **What does solving this teach?**

A proposed exercise should ideally include:

```text
Title
Objective
Prerequisites
Problem statement
Constraints
Expected behavior
Suggested test cases
Extension challenges
Learning outcome
```

Avoid exercises that are difficult merely because they are complicated.

Difficulty should arise from the concept being learned.

## Solutions

Solutions may be stored separately when appropriate.

Possible structures include:

```text
exercise/
├── README.md
├── starter/
└── solution/
```

However, solutions should not be exposed prematurely when doing so would undermine an active learning objective.

---

# 13. Laboratory Contributions

Labs exist to investigate questions.

A strong laboratory contribution follows:

```text
Question
 ↓
Hypothesis
 ↓
Setup
 ↓
Experiment
 ↓
Observation
 ↓
Analysis
 ↓
Conclusion
```

For example:

```text
Question:
How does synchronization affect throughput?

Hypothesis:
Increasing contention will reduce throughput.

Experiment:
Run equivalent workloads under multiple synchronization strategies.

Observation:
Measure throughput, latency, CPU usage, and contention.

Conclusion:
Explain what the measurements demonstrate.
```

A lab should not merely be:

> "Here is some code I ran."

It should explain **what the experiment teaches**.

---

# 14. Project Contributions

Projects integrate multiple concepts.

Contributions to projects should respect the project's current educational stage.

Before contributing to a project, determine:

- what phase the project belongs to;
- what concepts it is intended to reinforce;
- what architecture is currently being explored;
- whether the maintainer has already implemented the relevant concepts.

Do not prematurely transform an educational project into an enterprise architecture demonstration.

For example, a beginner banking CLI does not necessarily need:

```text
microservices
Kafka
Redis
Kubernetes
event sourcing
distributed tracing
```

The objective of the project may simply be:

> Learn object-oriented Java.

---

# 15. Documentation Contributions

Documentation is one of the safest and most valuable ways to contribute.

Documentation should be:

- accurate;
- concise where possible;
- explicit where necessary;
- technically grounded;
- consistent with Java 21 unless otherwise stated;
- clear about assumptions;
- and linked to authoritative sources where appropriate.

Avoid explanations that merely restate syntax.

Good documentation explains:

```text
What is it?
Why does it exist?
How does it work?
When should it be used?
When should it not be used?
What are the trade-offs?
```

---

# 16. Reference Material Contributions

Recommended resources should be evaluated for:

- authority;
- relevance;
- technical accuracy;
- version compatibility;
- longevity;
- educational value.

Prefer:

1. official documentation;
2. specifications;
3. authoritative books;
4. recognized technical references;
5. reputable educational material.

Avoid making a random blog post the canonical explanation of a Java language feature when official documentation or specifications are available.

---

# 17. Code Standards

Java Zenith targets **Java 21** unless a section explicitly specifies another version for comparison or compatibility work.

Code should prioritize:

- readability;
- correctness;
- explicit intent;
- appropriate abstraction;
- maintainability;
- testability.

## 17.1 Naming

Use descriptive names.

Prefer:

```java
calculateTransactionTotal()
```

over:

```java
calc()
```

Prefer:

```java
transactionCount
```

over:

```java
n
```

unless the shorter form has a clear local mathematical meaning.

## 17.2 Methods

Methods should have coherent responsibilities.

Avoid methods that simultaneously:

- parse input;
- validate business rules;
- access a database;
- perform networking;
- format output;
- and manage application state.

The exact structure should follow the problem rather than a rigid template.

## 17.3 Comments

Comments should explain **why**, not merely restate **what** the code already says.

Prefer:

```java
// Retry only idempotent operations because repeating the request
// can otherwise create duplicate financial transactions.
```

over:

```java
// Retry the operation.
```

## 17.4 Abstraction

Do not abstract prematurely.

Use abstraction when it provides meaningful value such as:

- substitution;
- isolation;
- testability;
- reuse;
- domain clarity;
- or architectural separation.

Do not introduce patterns merely because they exist.

---

# 18. Testing Standards

Contributions that change behavior should include appropriate tests where practical.

Tests should communicate behavior.

Consider:

```text
Happy path
Boundary conditions
Invalid input
Failure modes
State transitions
Concurrency behavior
Integration behavior
```

depending on the feature.

A test suite should not exist solely to increase coverage.

## Test quality

A useful test should make it clear:

- what is being tested;
- what behavior is expected;
- what condition matters;
- and why the failure would matter.

---

# 19. Benchmarking and Performance Work

Performance claims should be measured.

Do not submit:

> "This is faster."

without evidence.

A benchmark should document:

- workload;
- environment;
- Java version;
- JVM configuration where relevant;
- number of iterations;
- warm-up considerations;
- measurement method;
- results;
- interpretation;
- limitations.

For serious JVM benchmarking, prefer appropriate tooling such as JMH rather than naïve timing with `System.nanoTime()`.

The principle is:

> **Measure before concluding.**

---

# 20. Dependency Policy

Every dependency introduces:

- maintenance cost;
- security considerations;
- versioning concerns;
- transitive dependencies;
- learning implications.

Before adding a dependency, ask:

1. Is it necessary?
2. Is the functionality reasonably implementable for the educational objective?
3. Does the dependency hide the concept currently being studied?
4. Is the project mature and maintained?
5. Is the license appropriate?
6. Does the dependency introduce unnecessary complexity?

A dependency may be rejected even if it is convenient.

Educational value matters.

---

# 21. AI-Assisted Contributions

AI-assisted development may be used as a tool, but generated code must not replace understanding.

Contributors are responsible for:

- understanding submitted code;
- verifying its correctness;
- checking dependencies;
- testing behavior;
- reviewing security implications;
- and explaining significant design decisions.

Do not submit generated code merely because it compiles.

For learning-focused material, contributors should be especially careful not to use AI to bypass the intended intellectual work.

A useful standard is:

> **If you cannot explain the code you are contributing, you should not contribute it.**

The same principle applies to the maintainer.

---

# 22. Git Workflow

A contribution should generally follow:

```text
Issue / discussion
        ↓
Branch
        ↓
Implementation
        ↓
Tests
        ↓
Documentation
        ↓
Review
        ↓
Revision
        ↓
Merge
```

Avoid making unrelated changes in the same branch.

A branch should have a coherent purpose.

Examples:

```text
docs/improve-generics-notes
test/add-transaction-edge-cases
lab/virtual-thread-experiment
feat/add-collection-kata
fix/broken-maven-instructions
```

---

# 23. Commit Standards

Commits should describe meaningful changes.

Preferred prefixes include:

```text
feat:
fix:
docs:
test:
refactor:
perf:
chore:
lab:
```

Examples:

```text
docs: clarify HashMap equality contract
test: add boundary cases for transaction service
feat: add collection kata
lab: compare synchronized counters
perf: benchmark virtual thread workload
refactor: simplify validation logic
fix: correct Maven setup instructions
chore: update repository tooling
```

Avoid:

```text
update
changes
stuff
work
final
final-final
test
asdf
```

A good commit should help someone understand the repository's history months later.

---

# 24. Pull Requests

A pull request should clearly communicate:

## What changed?

Describe the actual change.

## Why?

Explain the problem or educational objective.

## How?

Describe the implementation approach.

## How was it tested?

List relevant tests or experiments.

## What did you learn?

For educational contributions, explain the relevant lesson.

## Does it affect the curriculum?

State whether the contribution changes:

- learning order;
- difficulty;
- prerequisites;
- or mastery requirements.

A useful PR description may follow:

```markdown
## Summary

Describe the change.

## Motivation

Why is this change useful?

## Learning Objective

What concept does this reinforce?

## Implementation

Explain the approach.

## Testing

Describe tests performed.

## Documentation

Describe documentation changes.

## Curriculum Impact

Does this alter the learning progression?

## Learning Integrity

Does this contribution expose or replace an active solution?

## Additional Notes

Anything else reviewers should know.
```

---

# 25. Review Standards

Reviews should be technical, constructive, and educational.

Reviewers should consider:

### Correctness

Does it work?

### Clarity

Can another engineer understand it?

### Testing

Is important behavior verified?

### Design

Are abstractions justified?

### Performance

Are there meaningful performance implications?

### Security

Does it introduce vulnerabilities or unsafe assumptions?

### Maintainability

Will the code remain understandable?

### Educational value

Does the contribution reinforce the intended learning objective?

### Scope

Does the contribution solve the stated problem without unnecessary expansion?

---

# 26. Maintainer Authority

The maintainer retains final authority over Java Zenith.

This includes decisions regarding:

- repository structure;
- curriculum;
- learning objectives;
- implementation direction;
- accepted contributions;
- dependencies;
- project scope;
- documentation;
- release strategy;
- contributor permissions.

This is not intended to discourage collaboration.

It exists because Java Zenith has a specific purpose.

The repository is not governed solely by the question:

> "Is this technically better?"

It must also answer:

> **"Is this better for the learning system?"**

---

# 27. Rejection Criteria

A contribution may be rejected if it:

- undermines an active learning objective;
- solves an exercise prematurely;
- introduces unnecessary complexity;
- introduces an unnecessary dependency;
- lacks sufficient testing;
- contains unexplained generated code;
- conflicts with the curriculum;
- duplicates existing functionality;
- changes unrelated parts of the repository;
- introduces security concerns;
- cannot be reproduced;
- is insufficiently documented;
- or does not provide enough educational or engineering value.

Rejection does not necessarily mean the contribution is bad.

It may simply mean:

> **It does not belong in Java Zenith at this time.**

---

# 28. Conflict Resolution

Technical disagreements should be resolved through evidence.

When two approaches differ, prefer:

```text
Clarify assumptions
        ↓
Identify requirements
        ↓
Build minimal examples
        ↓
Test
        ↓
Measure where appropriate
        ↓
Consult documentation
        ↓
Compare trade-offs
        ↓
Choose deliberately
```

Avoid arguments based purely on:

- personal preference;
- popularity;
- authority;
- "everyone does it this way";
- or cargo-cult architecture.

When evidence remains inconclusive, document the trade-off.

---

# 29. Attribution

Contributors should receive appropriate credit for accepted work.

Attribution may occur through:

- commit history;
- pull requests;
- contributor listings;
- documentation;
- project acknowledgements.

Contributions should not be misrepresented as work performed by someone else.

Likewise, contributors should not claim ownership of the overall Java Zenith curriculum merely because they contributed to a component.

---

# 30. Security and Sensitive Information

Never commit:

- passwords;
- API keys;
- access tokens;
- private keys;
- credentials;
- database secrets;
- personal information;
- production configuration containing secrets.

Use environment variables or appropriate secret-management mechanisms.

Before contributing code involving:

- authentication;
- authorization;
- cryptography;
- payments;
- financial data;
- networking;
- file access;
- deserialization;
- or external services,

consider the security implications carefully.

If a vulnerability is discovered, avoid publicly exposing sensitive exploit details before appropriate remediation.

---

# 31. Contribution Checklist

Before submitting a contribution, ask:

### Purpose

- [ ] Does this solve a real problem?
- [ ] Is the purpose clear?
- [ ] Does it fit Java Zenith?

### Learning integrity

- [ ] Does this preserve the intended learning process?
- [ ] Am I accidentally solving an active exercise?
- [ ] Does this contribution expose more than necessary?

### Code

- [ ] Is the code understandable?
- [ ] Are names meaningful?
- [ ] Are abstractions justified?
- [ ] Is the implementation appropriate for the current phase?

### Testing

- [ ] Have relevant tests been added?
- [ ] Have edge cases been considered?
- [ ] Have failure modes been considered?

### Documentation

- [ ] Is the behavior documented where necessary?
- [ ] Are technical claims accurate?
- [ ] Are relevant references included?

### Performance

- [ ] Are performance claims measured?
- [ ] Are benchmarks reproducible?

### Dependencies

- [ ] Is every new dependency justified?

### Git

- [ ] Is the branch focused?
- [ ] Are commits meaningful?
- [ ] Are unrelated changes excluded?

### Review

- [ ] Is the pull request easy to understand?
- [ ] Have the relevant questions been answered?
- [ ] Is the contribution ready for review?

---

# 32. Definition of an Accepted Contribution

A contribution is considered ready for acceptance when:

- its purpose is understood;
- it fits the repository;
- it preserves learning integrity;
- the implementation is technically sound;
- relevant tests exist;
- documentation is sufficient;
- dependencies are justified;
- security implications have been considered;
- the scope is appropriate;
- and the maintainer approves the change.

For larger contributions, acceptance may additionally require:

- architectural review;
- curriculum review;
- benchmarking;
- design documentation;
- or a dedicated experiment.

---

# 33. Long-Term Collaboration

Java Zenith may evolve from a primarily personal repository into a broader collaborative learning environment.

If that happens, collaboration should expand deliberately.

A possible progression is:

```text
Personal learning
        ↓
Peer discussion
        ↓
Peer review
        ↓
Small contributions
        ↓
Trusted contributors
        ↓
Collaborative experiments
        ↓
Shared projects
        ↓
Open educational ecosystem
```

The repository should not skip directly from:

```text
"This is my learning repository."
```

to:

```text
"Everyone has write access."
```

Trust, responsibility, and repository authority should grow with demonstrated collaboration.

---

# 34. Final Principle

Java Zenith is built around a simple idea:

> **The repository exists to produce an engineer, not merely to contain code.**

Every contribution should therefore be evaluated against that purpose.

A contribution is valuable when it helps the repository become:

- clearer;
- more accurate;
- more rigorous;
- more useful;
- more reproducible;
- more technically sound;
- or more educational.

But there is one principle above all others:

```text
Do not optimize the repository
at the expense of the learner.
```

The ideal collaborator does not simply provide answers.

They help create better questions.

They do not merely write code.

They help develop better reasoning.

They do not remove every failure.

They help make failures understandable.

They do not replace the struggle.

They make the struggle more productive.

The desired relationship is:

```text
                    ┌───────────────┐
                    │    QUESTION   │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   STRUGGLE    │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │  EXPERIMENT   │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   DISCUSS     │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   UNDERSTAND  │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │    BUILD      │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │    TEST       │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   DOCUMENT    │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │    SHARE      │
                    └───────┬───────┘
                            │
                            └──────────→ Repeat
```

**Java Zenith welcomes collaboration.**

**Java Zenith protects learning.**

**The two are not contradictory.**

---

## Zenith Contribution Principle

```text
Help me understand.
Don't simply help me finish.

Challenge my assumptions.
Don't replace my reasoning.

Share knowledge.
Don't remove the opportunity to discover.

Improve the repository.
Don't compromise the learner.

Build together.
Learn deliberately.
```

**That is how we contribute to Java Zenith.**
