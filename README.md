# Mark Pierotti

*Following shower thoughts down the AI drainpipe to see what congeals on the other side—then giving it tests, documentation and acceptance criteria.*

I’m studying a **Bachelor of Information Technology**, majoring in **Networking
and Cybersecurity**, with a target completion date of **May 2027**.

I build practical projects in Python, C and Linux. My interests include embedded
systems, observability and AI-assisted engineering with clear validation and
documented limits.

## Featured projects

### [ASUS Router Telemetry](https://github.com/markpierotti/asus-router-telemetry)

A temporary ARM C reporter and an external Python standard-library collector make
a stock ASUS RT-AX56U observable without replacing its firmware. Routine sampling
makes no model calls.

- Supervised healthy-path trial: 14 successful samples.
- Separate Ethernet dropout/recovery trial: 18 attempts, 12 successes and six
  expected unreachable outcomes; incident transitions checked at defined thresholds.
- Experimental-release CI on Linux/macOS with Python 3.11 and 3.13: 368 collector tests passed per job, one
  expected skip, plus reporter checks.
- [Experimental v0.1.0 release](https://github.com/markpierotti/asus-router-telemetry/releases/tag/v0.1.0)
  · [Case study](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/case-study.md)
  · [Design and limits](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/design.md)

I defined scope and acceptance criteria, operated the physical bench and
coordinated AI-assisted research, implementation and review. The project records
human decisions, reproduced findings and what remains unproven.

### [Home Lab — Linux operations and recovery](https://github.com/markpierotti/home-lab)

I run Slim as a Linux home lab for DNS filtering, router telemetry, monitoring,
alerting and private evidence capture. It connects the router project to an
operating environment with Pi-hole/Unbound, Prometheus, Grafana and systemd.

- External missing-heartbeat test, 13 November 2026: I confirmed the down alert
  reached Telegram after the heartbeat was deliberately stopped.
- Mac backup pull restored: 14 archives checked, with Grafana and Pi-hole SQLite
  integrity checks. A full restore onto a clean host remains untested.
- Private evidence tooling: hashed log base/append chains, daily snapshots for two
  SQLite sources, storage guards and a one-way Mac reading copy.

[Project overview and evidence](https://github.com/markpierotti/home-lab/blob/main/docs/portfolio-copy.md)
· [Operations runbook](https://github.com/markpierotti/home-lab/blob/main/docs/slim-operations.md)
· [Roadmap](https://github.com/markpierotti/home-lab/blob/main/docs/home-lab-roadmap.md)

Network segmentation, Project Limbo and detection/investigation exercises remain
planned. I describe this as a home networking and security lab in development;
a deployed SOC is future work.

## Other projects

### [Soul Eats Kitchen](https://souleatskitchen.org)

I developed the live website for a community meal initiative. The site presents its
mission, outreach and catering information, with donation and support options.

### Self-exclusion application and desktop rebuild

My self-exclusion project includes a completed local HTML/JavaScript application
for managing records, preparing forms and supporting a separate read-only viewer,
packaged with a Go launcher. My Tauri/Rust and React/TypeScript desktop rebuild
is in development.

The project is private. I plan to write a sanitized case study documenting the
preserved original, engineering decisions, testing and the transition between
implementations.

### Herbert Tipping

I’m developing a sports tipping application with Next.js, TypeScript and Supabase.
The work includes authentication, competition-rule clarification, scoring review
and user-interface design. It is not presented as a deployed service.

### Hermes Venture Studio

My local AI-assisted development workflow covers product intake, scoped roles,
isolated worktrees, review gates and a shared evidence-based learning register.
I’m preparing a case study of the workflow’s mechanisms, corrections and limits.

### Planned: Project Limbo — networking art

**What if a noisy smart coffee machine got sent to Inception’s Limbo?**

I’m planning a networking art experiment: a simulated IoT coffee machine inside
an Inception-inspired lab topology. The visual theme makes the boundaries memorable;
the engineering will measure traffic visibility, isolation and detection through
controlled experiments. No completed lab results are claimed yet.

## How I work

I aim to make engineering claims traceable to source, tests and observed behavior.
I use AI tools openly, reproduce failures, preserve evidence and distinguish
successful trials from broader reliability claims.

I’m currently focusing on Linux process handling, defensive parsing, embedded
telemetry and reproducible deployment. My next Home Lab milestone is a full restore
rehearsal, followed by controlled restart, power-recovery and longer-running checks.

## Interests and opportunities

- Networking, cybersecurity and security monitoring.
- Applied AI engineering and agent orchestration.
- Embedded Linux, reverse engineering and useful hardware repurposing.
- Practical application development, reproducible tests and documented evidence.

I’m interested in graduate or junior networking and cybersecurity roles, and junior
applied AI engineering or agent-orchestration opportunities.
