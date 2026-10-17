### Hi, I'm Viktor

My focus is test design and the hardest part of testing: I reproduce elusive bugs and bisect regressions down to the commit that caused them, then send a fix or a minimal repro. I test on macOS 26 and 15 (Apple Silicon) and on Linux and Windows VMs that I spin up per issue.

**Recent contributions**
- [rust-lang/rust#164272](https://github.com/rust-lang/rust/pull/164272): added a regression test for an ICE in the new trait solver ([#155977](https://github.com/rust-lang/rust/issues/155977)). I bisected the fix to #156976 and checked the test on builds before and after it. Merged, ships in Rust 1.101.
- [rust-lang/rust#163374](https://github.com/rust-lang/rust/issues/163374#issuecomment-6102691483): bisected an ICE regression in the Rust 1.100 beta to the PR that caused it (#161349), pinpointed the failing code path, confirmed it on macOS and Linux, and scanned the beta crater runs: it shows up in one crate only.
- [rustdesk/rustdesk#15623](https://github.com/rustdesk/rustdesk/pull/15623): fixed unbounded memory growth of the macOS server (a missing autorelease pool around `NSScreen` calls). Merged; an affected user confirmed the fix, and the issue was closed. Root-cause analysis: [#14603](https://github.com/rustdesk/rustdesk/issues/14603#issuecomment-5012040507).

**Background.** Six years at YCLIENTS (a SaaS platform with 250k+ active users), from senior QA engineer to Head of QA: the team grew from 6 to 20+ people across 8 product teams. I shaped the QA process from requirements review to release (4,500+ reviewed test cases, requirements-to-release time down 40%+), ran group trainings on test design, led the rollout of a zero-bug policy, and validated the whole reproducible part of a 15,000+ bug backlog; most blockers and criticals were fixed. Earlier: monitoring software for CNC plants, and system administration since 2006. Today I work in information security.

Russian (native), English (B1).
