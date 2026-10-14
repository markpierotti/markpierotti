# Mark Pierotti

I’m studying a **Bachelor of Information Technology**, majoring in **Networking
and Cybersecurity**, with a target completion date of **May 2027**.

I build practical projects in Python, C and Linux. My interests include embedded
systems, observability and AI-assisted engineering with clear validation and
documented limits.

## Featured project

### [ASUS Router Telemetry](https://github.com/markpierotti/asus-router-telemetry)

A temporary ARM C reporter and an external Python standard-library collector make
a stock ASUS RT-AX56U observable without replacing its firmware. Routine sampling
makes no model calls.

- Supervised healthy-path trial: 14 successful samples.
- Separate Ethernet dropout/recovery trial: 18 attempts, 12 successes and six
  expected unreachable outcomes; incident transitions checked at defined thresholds.
- Linux/macOS CI on Python 3.11 and 3.13: 368 collector tests passed per job, one
  expected skip, plus reporter checks.
- [Experimental v0.1.0 release](https://github.com/markpierotti/asus-router-telemetry/releases/tag/v0.1.0)
  · [Case study](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/case-study.md)
  · [Design and limits](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/design.md)

I defined scope and acceptance criteria, operated the physical bench and
coordinated AI-assisted research, implementation and review. The project records
human decisions, reproduced findings and what remains unproven.

## Other projects

### [Soul Eats Kitchen](https://souleatskitchen.org)

Developed the live website for a community meal initiative. The site presents its
mission, outreach and catering information, with donation and support options.

### Self-exclusion application and desktop rebuild

A completed local HTML/JavaScript application for managing self-exclusion records,
preparing forms and supporting a separate read-only viewer, packaged with a Go
launcher. A Tauri/Rust and React/TypeScript desktop rebuild is in development.

Private project. A future sanitized case study will document the preserved
original, engineering decisions, testing and the transition between implementations.

### Herbert Tipping

Sports tipping application in development with Next.js, TypeScript and Supabase.
The work includes authentication, competition-rule clarification, scoring review
and user-interface design. It is not presented as a deployed service.

### Hermes Venture Studio

A local AI-assisted development workflow covering product intake, scoped roles,
isolated worktrees, review gates and a shared evidence-based learning register.
I’m preparing a case study of the workflow’s mechanisms, corrections and limits.

## How I work

I aim to make engineering claims traceable to source, tests and observed behavior.
I use AI tools openly, reproduce failures, preserve evidence and distinguish
successful trials from broader reliability claims.

Current learning focus: Linux process handling, defensive parsing, embedded
telemetry and reproducible deployment. Next project milestone: a Linux-host
integration and longer-running validation.

## Home Lab & Security Operations

I’m building a home networking and security lab to investigate device behavior,
collection failures and traffic containment. ASUS Router Telemetry is the first
completed component. Linux-host integration and longer-running validation are
next, followed by network segmentation, traffic monitoring and detection exercises.

The [home-lab roadmap](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/home-lab-roadmap.md)
separates the released experimental telemetry milestone from planned detection,
alert-triage and response workflows. A deployed SOC remains future work.

### Planned: Project Limbo

A visual networking and cybersecurity lab exploring IoT segmentation and traffic
monitoring. A simulated noisy device will support controlled comparisons of
traffic visibility, isolation and detection. Planned: no completed lab results
are claimed yet.

## Interests and opportunities

- Networking, cybersecurity and security monitoring.
- Applied AI engineering and agent orchestration.
- Embedded Linux, reverse engineering and useful hardware repurposing.
- Practical application development, reproducible tests and documented evidence.

Interested in graduate or junior networking and cybersecurity roles, and junior
applied AI engineering or agent-orchestration opportunities.
