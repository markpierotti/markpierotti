# AI-assisted engineering in practice

I use AI coding tools for research, implementation, tests and review. My role is
to define the problem, set constraints, connect the system to its real environment,
challenge conclusions and decide what the evidence supports.

The public projects below show that approach in concrete situations. They do not
establish that every change is independently reviewed or that AI improves delivery
speed or reliability by a measured amount.

## Example 1: a successful connection does not settle failed cleanup

[ASUS Router Telemetry](https://github.com/markpierotti/asus-router-telemetry)
collects measurements from a stock router using a temporary ARM reporter and an
external Python collector.

A supervised Ethernet disconnect/reconnect trial recorded 18 attempts: 12
successful samples and six expected unreachable outcomes. Collection recovered,
but one temporary directory remained. It was tracked, removed manually and
checked absent through a separate SSH connection.

The engineering decision was to keep cleanup uncertainty visible after successful
collection resumed. A recovered connection could not silently erase an unfinished
cleanup obligation.

My contribution included defining acceptance criteria, operating the physical
bench and directing the investigation and assisted implementation. The published
records distinguish the accepted hardware version from later software changes.

Evidence: [trial record](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/dropout-recovery-20261014.md)
· [design](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/design.md)
· [human and AI attribution](https://github.com/markpierotti/asus-router-telemetry/blob/main/docs/provenance.md).

## Example 2: a working repair still needs the full publication checks

The [Home Lab](https://github.com/markpierotti/home-lab) backup pull initially
retrieved only one archive. SSH inside a filename-reading loop was consuming the
remaining standard input. Adding `ssh -n` corrected the download loop; the recorded
manual rerun retrieved all 14 available archives.

During the subsequent publication review, the full suite found a second issue:
the deployment manifest still contained the old script checksum. The checksum was
updated before merge. The corrected branch passed the four Linux/macOS CI jobs,
including privileged Linux fixtures.

This was AI-assisted implementation and review. I authorized the work and owned
the scope; the assistant identified and corrected the publication mismatch. The
record credits the assistant's check rather than presenting it as a manual test
I personally performed.

Evidence: [backup validation](https://github.com/markpierotti/home-lab/blob/main/docs/slim-backup-validation-20261113.md)
· [reviewed and merged change](https://github.com/markpierotti/home-lab/pull/5)
· [CI results](https://github.com/markpierotti/home-lab/actions/runs/43524828396).

## The principles I apply

- State what success means before relying on an implementation.
- Test failure and recovery paths as well as the normal path.
- Keep human decisions, assistant work and automated checks distinguishable.
- Preserve unresolved failures instead of hiding them behind later success.
- Separate source tests, deployment observations and recovery evidence.
- Keep credentials, operational data and private client information out of public repositories.

The Home Lab's external heartbeat test confirmed Telegram delivery after a
deliberate interruption. It did not test actual power loss. Archive and SQLite
integrity checks passed, but a full restore onto a clean host remains outstanding.

My local Venture Studio work explores more structured task roles, reviews and
delivery records. I treat that as a developing workflow. These public examples
demonstrate specific decisions and corrections, not a benchmark of an autonomous
engineering system.
