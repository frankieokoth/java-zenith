# Java Zenith

> A deliberate, documentation-driven journey from Java 21 fundamentals to production-grade Spring Boot backend engineering.

**Status:** Active  
**Primary Language:** Java 21  
**Primary Framework:** Spring Boot  
**Build System:** Maven  
**Development Environment:** Linux / WSL2  
**Editor:** Visual Studio Code / Cursor  
**Version Control:** Git  
**Repository Type:** Personal engineering curriculum, laboratory, reference system, and portfolio of implementation work

---

## Table of Contents

- [1. What Is Java Zenith?](#1-what-is-java-zenith)
- [2. Why This Repository Exists](#2-why-this-repository-exists)
- [3. The Philosophy](#3-the-philosophy)
- [4. The Zenith Standard](#4-the-zenith-standard)
- [5. Learning Model](#5-learning-model)
- [6. Core Learning Loop](#6-core-learning-loop)
- [7. Curriculum](#7-curriculum)
  - [Phase 00 - Environment & Tooling](#phase-00--environment--tooling)
  - [Phase 01 - Java Foundations](#phase-01--java-foundations)
  - [Phase 02 - Object-Oriented Programming & Design](#phase-02--object-oriented-programming--design)
  - [Phase 03 - Exceptions & Robustness](#phase-03--exceptions--robustness)
  - [Phase 04 - Collections & Generics](#phase-04--collections--generics)
  - [Phase 05 - Functional & Modern Java](#phase-05--functional--modern-java)
  - [Phase 06 - Testing & Build Engineering](#phase-06--testing--build-engineering)
  - [Phase 07 - JVM Internals](#phase-07--jvm-internals)
  - [Phase 08 - Concurrency](#phase-08--concurrency)
  - [Phase 09 - Spring Core](#phase-09--spring-core)
  - [Phase 10 - Spring Boot & Web](#phase-10--spring-boot--web)
  - [Phase 11 - Persistence](#phase-11--persistence)
  - [Phase 12 - Spring Testing](#phase-12--spring-testing)
  - [Phase 13 - Security](#phase-13--security)
  - [Phase 14 - Production Engineering](#phase-14--production-engineering)
  - [Phase 15 - Distributed Backend Systems](#phase-15--distributed-backend-systems)
  - [Phase 16 - Zenith Capstone](#phase-16--zenith-capstone)
- [8. Repository Architecture](#8-repository-architecture)
- [9. Reference Material](#9-reference-material)
- [10. Documentation Standards](#10-documentation-standards)
- [11. Experimentation](#11-experimentation)
- [12. Testing Philosophy](#12-testing-philosophy)
- [13. Concurrency Philosophy](#13-concurrency-philosophy)
- [14. Spring Philosophy](#14-spring-philosophy)
- [15. Linux & CLI Integration](#15-linux--cli-integration)
- [16. Git Discipline](#16-git-discipline)
- [17. Engineering Journal](#17-engineering-journal)
- [18. Feynman Method](#18-feynman-method)
- [19. Struggle-First Learning](#19-struggle-first-learning)
- [20. Mastery Checkpoints](#20-mastery-checkpoints)
- [21. Definition of Done](#21-definition-of-done)
- [22. Projects](#22-projects)
- [23. Capstone](#23-capstone)
- [24. Anti-Patterns](#24-anti-patterns)
- [25. Progress Tracking](#25-progress-tracking)
- [26. Long-Term Objective](#26-long-term-objective)
- [27. Final Principle](#27-final-principle)

---

# 1. What Is Java Zenith?

**Java Zenith** is a long-form, implementation-first curriculum for mastering modern Java and the Spring ecosystem.

It is not intended to be:

- a collection of copied tutorials;
- a list of completed courses;
- a repository of random coding exercises;
- a Spring Boot boilerplate generator;
- a "finish this book as quickly as possible" challenge;
- or a certificate-collection exercise.

Instead, Java Zenith is a **personal software engineering laboratory**.

The repository exists to document the progression from:

```text
Java syntax
    ↓
Java programming
    ↓
Object-oriented design
    ↓
Data structures & collections
    ↓
Modern Java
    ↓
Testing
    ↓
JVM understanding
    ↓
Concurrency
    ↓
Software construction
    ↓
Spring
    ↓
Spring Boot
    ↓
Databases
    ↓
Security
    ↓
Production engineering
    ↓
Distributed systems
    ↓
Production-grade backend engineering
```

The ultimate objective is not merely to "know Java."

The objective is to become capable of **designing, implementing, testing, debugging, profiling, documenting, deploying, and maintaining serious Java backend systems.**

---

# 2. Why This Repository Exists

Java is required for the trainee engineering path this repository is preparing for.

Spring Boot extends that requirement into the modern backend ecosystem.

Rather than learning the two technologies independently through disconnected tutorials, this repository treats them as part of one continuous engineering progression.

The intended progression is:

```text
Java
 ↓
JVM
 ↓
Software Construction
 ↓
Concurrency
 ↓
Spring
 ↓
Spring Boot
 ↓
Web Applications
 ↓
Persistence
 ↓
Security
 ↓
Production Systems
```

This matters because Spring makes much more sense when its underlying Java concepts are already understood.

For example, dependency injection becomes considerably easier to understand after learning:

- interfaces;
- classes;
- composition;
- constructors;
- polymorphism;
- abstraction;
- reflection;
- annotations;
- immutability;
- lifecycle management;
- and dependency inversion.

Likewise, backend concurrency becomes more meaningful after understanding:

- threads;
- executors;
- synchronization;
- locks;
- atomic operations;
- futures;
- asynchronous computation;
- and virtual threads.

Java Zenith therefore emphasizes **conceptual dependency order** rather than simply following the table of contents of a book.

---

# 3. The Philosophy

## 3.1 Learn the language, not just the framework

Spring Boot is not a substitute for Java knowledge.

The framework should amplify Java knowledge rather than conceal its absence.

The repository therefore prioritizes:

1. Java fundamentals
2. object-oriented programming
3. collections and generics
4. modern Java
5. testing
6. JVM fundamentals
7. concurrency
8. Spring
9. Spring Boot
10. backend engineering

---

## 3.2 Documentation is part of programming

Documentation is not something consulted only after becoming stuck.

Primary documentation is part of the learning process.

The Java platform documentation, API documentation, language specifications, framework documentation, build-tool documentation, and relevant technical references should be treated as first-class learning resources.

The goal is to develop the ability to answer:

> "Where does the platform itself say this?"

rather than relying exclusively on:

> "Someone on Stack Overflow said this."

---

## 3.3 Understand before abstracting

Framework abstractions are useful.

But abstractions should not become magic.

Whenever practical, the repository should move through:

```text
Observe
 ↓
Understand
 ↓
Implement manually
 ↓
Use the abstraction
 ↓
Understand what the abstraction provides
```

For example:

```text
Raw HTTP
 ↓
Servlet concepts
 ↓
Spring MVC
 ↓
Spring Boot
```

The goal is not to reinvent every framework.

The goal is to understand enough of the underlying system that the framework remains comprehensible.

---

## 3.4 Build things that can fail

A system that only works under perfect conditions teaches very little.

Projects should deliberately encounter:

- invalid input;
- malformed requests;
- unavailable resources;
- database failures;
- race conditions;
- incorrect assumptions;
- performance problems;
- configuration errors;
- authentication failures;
- dependency failures;
- and unexpected state.

Failure is not an interruption to the curriculum.

**Failure is part of the curriculum.**

---

## 3.5 Struggle before searching

When encountering a problem:

1. Understand the problem.
2. Attempt a solution.
3. Inspect the failure.
4. Form a hypothesis.
5. Test the hypothesis.
6. Consult documentation.
7. Search externally if necessary.
8. Compare solutions.
9. Implement the solution.
10. Explain why it works.

The objective is to prevent passive consumption.

---

# 4. The Zenith Standard

A topic is not considered mastered merely because its syntax has been encountered.

A concept reaches the **Zenith Standard** when it can be:

### 1. Explained

The concept can be described in clear language without relying on memorized definitions.

### 2. Implemented

The concept can be used without following a tutorial line by line.

### 3. Debugged

When something goes wrong, the underlying mechanism can be investigated.

### 4. Tested

Expected behavior and important failure modes can be verified.

### 5. Compared

Alternative approaches can be evaluated and their trade-offs explained.

### 6. Applied

The concept can be incorporated into a larger system.

### 7. Defended

Design decisions can be justified technically.

The progression is therefore:

```text
Recognize
   ↓
Understand
   ↓
Implement
   ↓
Debug
   ↓
Test
   ↓
Compare
   ↓
Apply
   ↓
Defend
```

---

# 5. Learning Model

Java Zenith uses several complementary resources.

## Primary textbook

The primary comprehensive Java reference is:

**Java: The Complete Reference, 13th Edition**

The book is used as a structured reference and conceptual guide.

It is **not** treated as a race to the final page.

---

## Official documentation

Official Java documentation is used to verify:

- language behavior;
- APIs;
- classes;
- interfaces;
- methods;
- exceptions;
- JVM behavior;
- version-specific functionality;
- and implementation contracts.

---

## Secondary references

Additional books and references may be introduced when they provide value that the primary text does not.

Potential areas include:

- effective Java practices;
- software construction;
- JVM internals;
- concurrency;
- system design;
- Spring;
- databases;
- distributed systems.

---

## Practical work

Every major conceptual section should produce something tangible:

- an exercise;
- a kata;
- a laboratory experiment;
- a benchmark;
- a test suite;
- a small application;
- or a larger project.

---

# 6. Core Learning Loop

Every significant topic follows this cycle:

```text
                    ┌───────────────┐
                    │    THEORY     │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │ DOCUMENTATION │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │ IMPLEMENTATION│
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │ EXPERIMENT    │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   FAILURE     │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   DEBUGGING   │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │    TESTING    │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │  EXPLANATION  │
                    └───────┬───────┘
                            ↓
                    ┌───────────────┐
                    │   INTEGRATION │
                    └───────────────┘
```

The cycle then repeats at a higher level of complexity.

---

# 7. Curriculum

# Phase 00 — Environment & Tooling

Directory:

```text
curriculum/00-environment/
```

Objective:

Become comfortable operating the development environment before serious Java development begins.

Topics:

- Linux filesystem
- absolute paths
- relative paths
- `/`
- `.`
- `..`
- `~`
- Bash
- environment variables
- command execution
- standard input
- standard output
- standard error
- pipes
- redirection
- quoting
- escaping
- globbing
- brace expansion
- command substitution
- exit codes
- permissions
- processes
- package management
- Git
- Maven
- JDK installation
- Java environment variables

Core commands include:

```text
pwd
ls
cd
mkdir
touch
cp
mv
rm
rmdir
find
grep
cat
less
head
tail
which
echo
printf
chmod
ps
kill
```

This phase also establishes the development environment used by all subsequent phases.

---

# Phase 01 — Java Foundations

Directory:

```text
curriculum/01-java-foundations/
```

Topics:

- Java source files
- classes
- `main`
- variables
- primitive types
- reference types
- literals
- operators
- expressions
- statements
- control flow
- conditionals
- loops
- arrays
- methods
- parameters
- return values
- scope
- packages
- imports
- access modifiers
- `static`
- `final`
- strings
- `StringBuilder`
- basic input/output

Core question:

> Can I write a small Java program from an empty directory without a tutorial?

---

# Phase 02 — Object-Oriented Programming & Design

Directory:

```text
curriculum/02-oop-design/
```

Topics:

- classes
- objects
- constructors
- encapsulation
- inheritance
- polymorphism
- abstraction
- interfaces
- composition
- delegation
- method overriding
- method overloading
- `Object`
- equality
- identity
- `equals`
- `hashCode`
- `toString`
- immutability
- records
- sealed classes
- nested classes
- enums

Engineering concepts:

- coupling
- cohesion
- composition over inheritance
- dependency inversion
- API design
- object ownership
- invariants

---

# Phase 03 — Exceptions & Robustness

Directory:

```text
curriculum/03-exceptions-robustness/
```

Topics:

- exceptions
- checked exceptions
- unchecked exceptions
- `try`
- `catch`
- `finally`
- try-with-resources
- custom exceptions
- exception propagation
- exception handling strategies
- validation
- defensive programming
- resource management

Questions:

- What should fail?
- Where should it fail?
- Who should handle the failure?
- What information should the exception contain?
- When should an exception be translated?
- When should it be allowed to propagate?

---

# Phase 04 — Collections & Generics

Directory:

```text
curriculum/04-collections-generics/
```

Topics:

- `List`
- `ArrayList`
- `LinkedList`
- `Set`
- `HashSet`
- `TreeSet`
- `Map`
- `HashMap`
- `TreeMap`
- queues
- deques
- iterators
- collection algorithms
- generics
- bounded type parameters
- wildcards
- covariance
- contravariance
- type erasure
- comparators
- sorting

Engineering focus:

- complexity
- memory usage
- API contracts
- mutability
- equality
- ordering
- performance trade-offs

---

# Phase 05 — Functional & Modern Java

Directory:

```text
curriculum/05-functional-modern-java/
```

Topics:

- lambda expressions
- functional interfaces
- method references
- `Predicate`
- `Function`
- `Consumer`
- `Supplier`
- streams
- collectors
- optional
- `var`
- records
- sealed classes
- pattern matching
- switch expressions
- modern language features
- text blocks

Focus:

> Understand why the feature exists, not merely how to write its syntax.

---

# Phase 06 — Testing & Build Engineering

Directory:

```text
curriculum/06-testing-build/
```

Topics:

- Maven
- project lifecycle
- dependencies
- plugins
- profiles
- packaging
- JUnit
- assertions
- unit testing
- integration testing
- parameterized tests
- test doubles
- mocking
- test fixtures
- test organization
- code coverage
- static analysis
- build automation

Engineering principle:

> Tests are executable specifications.

A test should communicate intended behavior, not merely increase a coverage percentage.

---

# Phase 07 — JVM Internals

Directory:

```text
curriculum/07-jvm-internals/
```

Topics:

- JVM architecture
- bytecode
- class files
- class loading
- class loaders
- heap
- stack
- metaspace
- garbage collection
- JIT compilation
- runtime optimization
- memory management
- object allocation
- references
- profiling
- JVM diagnostic tools
- `jcmd`
- `jstack`
- `jmap`
- `jps`
- Java Flight Recorder
- Java Mission Control

Objective:

Develop a useful mental model of what happens after Java source code is compiled.

---

# Phase 08 — Concurrency

Directory:

```text
curriculum/08-concurrency/
```

Topics:

- processes
- threads
- thread lifecycle
- race conditions
- visibility
- atomicity
- ordering
- `synchronized`
- intrinsic locks
- explicit locks
- `ReentrantLock`
- read/write locks
- atomics
- concurrent collections
- executors
- thread pools
- `Future`
- `CompletableFuture`
- asynchronous programming
- parallel streams
- structured concurrency concepts
- virtual threads
- deadlocks
- starvation
- livelocks
- contention
- thread safety

Core question:

> What guarantees does this concurrency mechanism provide?

Concurrency is not learned by memorizing APIs.

It is learned by understanding **shared state, visibility, ordering, synchronization, and failure**.

---

# Phase 09 — Spring Core

Directory:

```text
curriculum/09-spring-core/
```

Topics:

- Spring architecture
- IoC
- dependency injection
- beans
- bean lifecycle
- application context
- component scanning
- configuration
- Java configuration
- annotations
- scopes
- constructor injection
- configuration properties
- profiles
- application events
- AOP concepts

Objective:

Understand Spring as a dependency management and application framework before relying on Spring Boot's conventions.

---

# Phase 10 — Spring Boot & Web

Directory:

```text
curriculum/10-spring-boot-web/
```

Topics:

- Spring Boot
- starters
- auto-configuration
- application configuration
- embedded servers
- REST
- HTTP
- controllers
- request mapping
- request parameters
- request bodies
- response entities
- validation
- DTOs
- serialization
- deserialization
- JSON
- exception handling
- API versioning
- pagination
- filtering
- sorting
- OpenAPI concepts

Projects should progress from:

```text
CLI
 ↓
HTTP service
 ↓
REST API
 ↓
multi-layer backend
```

---

# Phase 11 — Persistence

Directory:

```text
curriculum/11-persistence/
```

Topics:

- SQL
- relational modeling
- normalization
- transactions
- ACID
- indexes
- constraints
- PostgreSQL
- JDBC
- connection pools
- JPA
- Hibernate
- repositories
- entities
- relationships
- lazy loading
- eager loading
- N+1 queries
- transactions
- optimistic locking
- pessimistic locking
- migrations

Objective:

Understand the database rather than allowing an ORM to hide it.

---

# Phase 12 — Spring Testing

Directory:

```text
curriculum/12-spring-testing/
```

Topics:

- Spring test context
- integration tests
- controller tests
- service tests
- repository tests
- test containers
- database integration
- test slices
- HTTP integration testing
- test configuration
- mocking boundaries
- contract testing concepts

Objective:

Develop confidence that a Spring application works as a system, not merely as isolated classes.

---

# Phase 13 — Security

Directory:

```text
curriculum/13-security/
```

Topics:

- authentication
- authorization
- identity
- sessions
- cookies
- CSRF
- CORS
- password hashing
- JWT
- OAuth concepts
- OpenID Connect concepts
- roles
- authorities
- security filters
- Spring Security
- secure API design
- secret management
- common web vulnerabilities

Security principle:

> Security is an architectural property, not a final feature.

---

# Phase 14 — Production Engineering

Directory:

```text
curriculum/14-production-engineering/
```

Topics:

- logging
- structured logging
- configuration management
- environment variables
- observability
- metrics
- tracing
- health checks
- graceful shutdown
- resilience
- retries
- timeouts
- circuit breakers
- caching
- rate limiting
- performance
- profiling
- containerization
- Docker
- CI/CD
- deployment
- configuration separation
- operational debugging

Objective:

Move from:

> "The application works on my machine."

to:

> "The application can be operated responsibly."

---

# Phase 15 — Distributed Backend Systems

Directory:

```text
curriculum/15-distributed-systems/
```

Topics:

- distributed systems fundamentals
- networking
- latency
- availability
- consistency
- replication
- partitioning
- service boundaries
- asynchronous messaging
- message queues
- event-driven architecture
- idempotency
- retries
- delivery semantics
- eventual consistency
- distributed transactions
- caching
- load balancing
- service discovery
- fault tolerance
- observability
- backpressure
- concurrency at scale

Objective:

Understand the difference between:

```text
A program
```

and:

```text
A system of programs communicating over unreliable networks.
```

---

# Phase 16 — Zenith Capstone

Directory:

```text
curriculum/16-capstone/
```

The capstone is the final integration point for the entire curriculum.

It should demonstrate:

- modern Java
- object-oriented design
- collections
- generics
- functional programming
- testing
- Maven
- concurrency
- Spring Boot
- REST
- PostgreSQL
- JPA/Hibernate
- security
- observability
- caching
- resilience
- asynchronous processing
- Docker
- CI/CD
- documentation
- performance analysis

The capstone should not be a tutorial clone.

It should be designed, implemented, tested, documented, and defended independently.

---

# 8. Repository Architecture

The repository follows this structure:

```text
java-zenith/
│
├── curriculum/
│   ├── 00-environment/
│   ├── 01-java-foundations/
│   ├── 02-oop-design/
│   ├── 03-exceptions-robustness/
│   ├── 04-collections-generics/
│   ├── 05-functional-modern-java/
│   ├── 06-testing-build/
│   ├── 07-jvm-internals/
│   ├── 08-concurrency/
│   ├── 09-spring-core/
│   ├── 10-spring-boot-web/
│   ├── 11-persistence/
│   ├── 12-spring-testing/
│   ├── 13-security/
│   ├── 14-production-engineering/
│   ├── 15-distributed-systems/
│   └── 16-capstone/
│
├── reference/
│   ├── book-mapping/
│   ├── java-21/
│   └── spring/
│
├── katas/
│   ├── java/
│   ├── concurrency/
│   └── spring/
│
├── labs/
│   ├── java/
│   ├── jvm/
│   ├── concurrency/
│   ├── spring/
│   └── database/
│
├── projects/
│   ├── 01-banking-cli/
│   ├── 02-transaction-analytics/
│   ├── 03-financial-rest-api/
│   ├── 04-concurrency-lab/
│   ├── 05-production-service/
│   └── 06-zenith-capstone/
│
├── benchmarks/
│
├── notes/
│   ├── feynman.md
│   ├── learning-journal.md
│   └── gotchas.md
│
├── docs/
│   ├── architecture/
│   └── checkpoints/
│
├── scripts/
│
├── .gitignore
├── CONTRIBUTING.md
├── README.md
└── ROADMAP.md
```

The structure intentionally separates:

```text
curriculum → what is being learned

reference → what is being consulted

katas → focused practice

labs → experiments

projects → integrated construction

benchmarks → measurement

notes → understanding

docs → engineering documentation

scripts → automation
```

---

# 9. Reference Material

Reference material is organized rather than scattered throughout the repository.

## Java

The primary Java reference is:

**Java: The Complete Reference, 13th Edition**

The book provides broad coverage of the language and platform.

The official Java documentation is used to verify and deepen understanding.

---

## Effective Java

A dedicated idiomatic-Java reference should be incorporated after sufficient Java fundamentals have been developed.

The purpose is to answer questions such as:

- What makes an API good?
- When should objects be immutable?
- Why prefer composition?
- How should `equals` and `hashCode` be implemented?
- How should generics be designed?
- When should streams be used?
- How should exceptions be handled?
- What makes concurrent code safe?

---

## Spring

Spring documentation is treated as a primary reference rather than relying exclusively on tutorials.

---

# 10. Documentation Standards

Every substantial project should contain documentation sufficient for another developer to understand it.

At minimum:

```text
README.md
```

For larger projects:

```text
README.md
ARCHITECTURE.md
DESIGN.md
SPEC.md
```

Important architectural decisions may be recorded separately.

Example:

```text
decisions/
├── 001-database-choice.md
├── 002-authentication-strategy.md
└── 003-message-delivery-model.md
```

---

# 11. Experimentation

Labs exist specifically to answer questions.

A laboratory should be allowed to fail.

Examples:

```text
Why does HashMap require hashCode?
Why does modifying a collection during iteration fail?
What happens when two threads update shared state?
How much does synchronization cost?
How do virtual threads behave under blocking I/O?
What happens when a transaction fails halfway through?
What does lazy loading actually do?
What does the JVM do with this object?
```

A useful laboratory follows:

```text
Question
 ↓
Hypothesis
 ↓
Experiment
 ↓
Observation
 ↓
Explanation
 ↓
Conclusion
```

---

# 12. Testing Philosophy

Testing exists to establish confidence.

The repository distinguishes between:

```text
Unit tests
Integration tests
System tests
Performance tests
Concurrency tests
```

A test suite should not merely prove that the happy path works.

Important failure modes should be represented.

For example:

```text
valid input
invalid input
boundary input
missing data
duplicate data
concurrent access
resource failure
database failure
network failure
authentication failure
authorization failure
```

---

# 13. Concurrency Philosophy

Concurrency is treated as a first-class engineering discipline.

The repository should avoid the mindset:

> "Use a thread because we need something to happen simultaneously."

Instead ask:

- What state is shared?
- Who owns that state?
- Can the state be immutable?
- What must be atomic?
- What must be visible?
- What ordering is required?
- What happens when operations overlap?
- What happens when one operation fails?
- What is the contention profile?
- What is the cost of synchronization?

Concurrency experiments should deliberately attempt to expose race conditions.

---

# 14. Spring Philosophy

Spring should never be treated as magic.

When learning a Spring feature, ask:

```text
What problem does this solve?

What did developers do before this abstraction?

What does Spring manage?

When does it happen?

What object is created?

Who owns its lifecycle?

What dependency is injected?

How is the dependency discovered?

What happens when configuration is incorrect?
```

Annotations should be understood as metadata and framework instructions, not mystical language constructs.

---

# 15. Linux & CLI Integration

Linux is part of the learning environment, not merely a place where Java happens to run.

The repository therefore intentionally uses the command line.

Important skills include:

```text
Filesystem navigation
File creation
Directory creation
Path manipulation
Permissions
Environment variables
Pipes
Redirection
Process management
Package management
Git
Maven
Java tooling
Shell scripting
```

Commands should be learned conceptually.

For example:

```text
mkdir
```

means:

> make directory

while:

```text
mkdir -p
```

means:

> make the directory and create missing parent directories as necessary.

Likewise:

```text
rm
```

means:

> remove

while:

```text
rm -r
```

means:

> remove recursively

and:

```text
rm -rf
```

means:

> remove recursively and forcefully.

The goal is to understand command semantics rather than memorize incantations.

---

# 16. Git Discipline

Git history is part of the learning record.

Commits should communicate meaningful changes.

Examples:

```text
chore: initialize Java Zenith
docs: define Java foundations curriculum
feat: implement collection exercises
test: add edge cases for transaction service
refactor: extract payment validation
perf: benchmark concurrent transaction processing
docs: document concurrency findings
```

Avoid meaningless commits such as:

```text
stuff
changes
update
final
final-final
please-work
```

The repository should eventually tell a coherent story through its history.

---

# 17. Engineering Journal

File:

```text
notes/learning-journal.md
```

The learning journal records:

- difficult concepts;
- breakthroughs;
- bugs;
- debugging experiences;
- design mistakes;
- useful commands;
- questions;
- discoveries;
- misconceptions;
- and lessons learned.

A useful entry might look like:

```text
## 2026-08-12 — Bash Brace Expansion

### Problem

My directory-generation command created a malformed directory.

### Initial assumption

I assumed the space in the directory name caused the problem.

### Investigation

Checked:

```bash
set -o | grep braceexpand
```

### Discovery

Brace expansion had been disabled when the command was executed.

### Lesson

Bash performs multiple stages of command processing.

### Takeaway

Never assume a shell command means what it visually appears to mean.
Understand how the shell parses it.
```

Mistakes are valuable when documented.

---

# 18. Feynman Method

File:

```text
notes/feynman.md
```

For difficult concepts, use the following structure:

```text
# Concept

## 1. Explain it simply

Explain the concept as if teaching someone who has never encountered it.

## 2. What problem does it solve?

Why does this concept exist?

## 3. Example

Provide a concrete example.

## 4. Common misconception

What do beginners commonly get wrong?

## 5. Technical explanation

Now explain the underlying mechanism precisely.

## 6. Demonstration

Provide executable code or an experiment.

## 7. Where is it useful?

Connect it to real engineering.

## 8. What remains unclear?

Document remaining questions.
```

The goal is not polished prose.

The goal is **clarity of thought**.

---

# 19. Struggle-First Learning

Java Zenith deliberately avoids excessive tutorial dependence.

When encountering a new problem:

### Stage 1

Attempt the problem independently.

### Stage 2

Use compiler errors and runtime errors as information.

### Stage 3

Inspect documentation.

### Stage 4

Experiment.

### Stage 5

Ask for assistance if necessary.

### Stage 6

Implement the solution.

### Stage 7

Explain the solution without looking at the answer.

This produces deeper retention than passive copying.

---

# 20. Mastery Checkpoints

Each curriculum phase should have a checkpoint.

A checkpoint should answer:

> "Can I actually use this?"

For example, the Collections checkpoint might require:

- choosing an appropriate collection;
- explaining the choice;
- implementing the solution;
- testing it;
- analyzing complexity;
- and defending the design.

A concurrency checkpoint might require:

- reproducing a race condition;
- explaining why it occurs;
- implementing a safe version;
- comparing synchronization strategies;
- and measuring the result.

A Spring checkpoint might require:

- creating an application without following a tutorial;
- designing its layers;
- testing its behavior;
- handling errors;
- and explaining the framework mechanisms involved.

---

# 21. Definition of Done

A curriculum section is not "done" because the directory contains code.

A topic is complete when:

- The concept has been studied.
- Relevant documentation has been consulted.
- At least one implementation exists.
- The implementation was written independently.
- Important edge cases were considered.
- Tests exist where appropriate.
- The implementation has been debugged.
- The concept can be explained without notes.
- At least one experiment has been performed where useful.
- A Feynman explanation exists for difficult concepts.
- The concept has been used in a larger exercise or project.
- The trade-offs are understood.
- The checkpoint has been passed.

---

# 22. Projects

Projects exist to force concepts to interact.

## Project 01 — Banking CLI

Purpose:

Learn Java fundamentals and object-oriented design.

Potential features:

- accounts;
- deposits;
- withdrawals;
- transfers;
- transaction history;
- validation;
- persistence to files;
- command-line interface;
- unit tests.

---

## Project 02 — Transaction Analytics

Purpose:

Integrate:

- collections;
- streams;
- generics;
- records;
- functional programming;
- file processing;
- testing;
- performance measurement.

Potential capabilities:

- transaction aggregation;
- filtering;
- categorization;
- statistical analysis;
- reporting.

---

## Project 03 — Financial REST API

Purpose:

Transition from standalone Java to Spring Boot.

Potential components:

```text
REST API
 ↓
Service layer
 ↓
Repository layer
 ↓
PostgreSQL
```

Features:

- authentication;
- accounts;
- transactions;
- validation;
- error handling;
- persistence;
- API documentation;
- tests.

---

## Project 04 — Concurrency Laboratory

Purpose:

Demonstrate understanding of concurrent systems.

Experiments should include:

- race conditions;
- synchronized access;
- locks;
- atomics;
- executor services;
- futures;
- concurrent collections;
- virtual threads;
- throughput;
- latency;
- contention.

The project should contain measurements rather than merely code.

---

## Project 05 — Production Service

Purpose:

Combine Spring Boot with production engineering.

Potential features:

- structured logging;
- metrics;
- tracing;
- health checks;
- Docker;
- configuration management;
- caching;
- retries;
- timeouts;
- database migrations;
- CI/CD.

---

## Project 06 — Zenith Capstone

Purpose:

Demonstrate integrated engineering ability.

The capstone should be sufficiently complex that architecture, concurrency, persistence, security, observability, and operational concerns become real problems rather than theoretical topics.

---

# 23. Capstone

The capstone represents the highest level of the repository.

It should answer:

> Can I independently design and build a production-oriented Java backend system?

The capstone should contain:

```text
Application
API
Domain model
Persistence
Authentication
Authorization
Validation
Testing
Concurrency
Observability
Documentation
Deployment
Performance analysis
Failure handling
Architecture decisions
```

The capstone should also include:

```text
README.md
ARCHITECTURE.md
DESIGN.md
SPEC.md
```

and appropriate decision records.

---

# 24. Anti-Patterns

Java Zenith deliberately avoids the following:

## Tutorial hell

Watching dozens of hours of content without building anything.

## Syntax completionism

Attempting to memorize every Java feature before writing useful programs.

## Framework-first learning

Jumping into Spring annotations without understanding Java fundamentals.

## Cargo-cult architecture

Copying a package structure because a tutorial used it.

## Test theater

Writing tests solely to increase coverage statistics.

## Abstraction addiction

Creating interfaces and layers without a real reason.

## Premature optimization

Optimizing code before measuring it.

## Documentation avoidance

Guessing framework behavior instead of consulting official documentation.

## Copy-paste development

Using generated code without understanding it.

## Complexity worship

Making a project unnecessarily complicated merely to make it look advanced.

The goal is not maximal complexity.

The goal is **appropriate complexity**.

---

# 25. Progress Tracking

Progress should be measured across multiple dimensions.

## Knowledge

Can the concept be explained?

## Implementation

Can the concept be used independently?

## Debugging

Can failures be diagnosed?

## Testing

Can behavior be verified?

## Design

Can trade-offs be explained?

## Integration

Can the concept work inside a larger system?

A simple progress model:

```text
0 — Not encountered

1 — Encountered

2 — Understand the basics

3 — Can implement with guidance

4 — Can implement independently

5 — Can debug and test independently

6 — Can explain trade-offs

7 — Can apply in production-oriented systems

8 — Can teach the concept
```

The objective is not to achieve level 8 for every Java feature.

The objective is to develop deep mastery of the concepts that matter most to backend engineering.

---

# 26. Long-Term Objective

Java Zenith exists to develop a particular kind of engineer.

Not someone who merely knows:

```text
@RestController
@Service
@Repository
```

but someone who understands:

```text
Java
 ↓
JVM
 ↓
Concurrency
 ↓
Networking
 ↓
HTTP
 ↓
Spring
 ↓
Databases
 ↓
Transactions
 ↓
Security
 ↓
Distributed systems
 ↓
Production operations
```

The ultimate target is the ability to reason about an entire backend system.

When an application becomes slow:

> Investigate.

When requests fail:

> Trace.

When data becomes inconsistent:

> Identify the transaction and concurrency model.

When memory usage grows:

> Profile.

When throughput collapses:

> Measure contention, I/O, CPU, allocation, and dependencies.

When a Spring abstraction behaves unexpectedly:

> Understand what Spring is actually doing.

When a distributed system fails:

> Reason about the network, state, timing, and failure model.

---

# 27. Final Principle

Java Zenith is built around one central idea:

> **Do not optimize for completing the curriculum. Optimize for becoming the engineer the curriculum is supposed to produce.**

There is no prize for finishing the textbook quickly.

There is no prize for having hundreds of commits.

There is no prize for having thousands of lines of code.

There is no prize for knowing the most annotations.

The real measure of progress is whether difficult problems become increasingly understandable.

The desired progression is:

```text
"I don't understand this."
        ↓
"I can reproduce it."
        ↓
"I can explain what is happening."
        ↓
"I can fix it."
        ↓
"I understand why the fix works."
        ↓
"I can design the system correctly from the beginning."
```

That final transition is the purpose of Java Zenith.

---

## Zenith

```text
Learn deeply.
Build deliberately.
Break things.
Read the documentation.
Measure what matters.
Test your assumptions.
Understand the abstraction.
Document the lesson.
Repeat.

                     ┌──────────────┐
                     │    LEARN     │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │    BUILD     │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │    BREAK     │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │   UNDERSTAND │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │    TEST      │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │   MEASURE    │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │   DOCUMENT   │
                     └──────┬───────┘
                            ↓
                     ┌──────────────┐
                     │   INTEGRATE  │
                     └──────┬───────┘
                            │
                            └──────────────→ Repeat
```

**Java Zenith is not a course.**

**It is the record of becoming a Java engineer.**
