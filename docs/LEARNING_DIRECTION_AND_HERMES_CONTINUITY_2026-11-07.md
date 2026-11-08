# Developer Learning Direction & Hermes Continuity
Updated: 2026-11-07 (America/Chicago)
Owner: personal engineering learning; NOT an AXIORYTH technical authorization.

## Guiding distinction
**Guided configuration is exposure, not demonstrated mastery.** Installing or configuring software successfully does not mean the learner understands Docker, systemd, permissions, networking, packages, or agent security.

Track two separate modes:
1. **Guided development / configuration:** accomplish a bounded task together; explain commands and verify results. Log as "encountered / configured", not "learned / passed".
2. **Structured engineering education:** teach one concept at a time, let the learner type commands and implement code, predict outcomes, debug independently, answer knowledge checks, and pass practical checkpoints. Only grade final submitted work. Do not point out mistakes already self-corrected.

## Priority and boundaries
- Continue Python fundamentals (especially parameters and return values, list loops, conditional filtering), Linux fundamentals, Git, and ethical hacking labs. Do not skip earlier lessons because advanced tools have been encountered.
- EvidenceTrail is a **separate personal manual-first software-engineering learning challenge** for HackUTD 2027. Learner writes all implementation code; AI may tutor, hint, review, and grade, but does not generate the project's implementation.
- AXIORYTH/SI Core is separate. No access to protected assets, confidential evaluations, company secrets, or credential stores for exploratory agents.
- Claude Code / Codex may be read-only explainers/reviewers where permitted; no autonomous edits or execution without express decision and configured controls.

## Hermes experiment — status as observed Nov 7
Purpose: curiosity and study of multi-model agent frameworks, not production deployment or proof of skill.
- Hermes installed on Omarchy and its setup wizard completed; no external agent imports were intended.
- Chose minimal/blank setup; model provider unchanged; Docker/Podman terminal backend selected; egress firewall requested. Do not assume these are enforced without verification.
- User declined starting the gateway immediately and automatic-start choice; diagnostics nevertheless report systemd linger enabled. Linger is not proof the gateway is active; verify service state.
- hermes doctor showed Python and configuration checks mostly healthy, but Docker daemon inaccessible. Terminal, code_execution, browser and other tools appear *available* in diagnostics; availability is not proof of safe/disabled runtime permissions.
- Docker CLI 29.9.2 installed. system docker.service reported inactive/disabled; /var/run/docker.sock root:root mode srw-rw----. No working Docker sandbox verified.
- Podman, rootlesskit, slirp4netns, and rootless setup utility not found at observed checks. 'yay' available, subordinate UID/GID ranges configured (100000:65536).
- Inspected 'yay -Si docker-rootless-extras' (AUR version 29.9.3-1) and part of PKGBUILD via 'yay -Gp'. Package not confirmed installed. Review all source checks and package compatibility before installation. AUR build scripts require scrutiny.
- No evidence of a verified rootless container, firewall policy, restricted mounts, isolated Hermes host process, or approved credential handling. DO NOT treat this as a finished security setup.

## Next session — safe continuation
1. Verify whether any Hermes gateway service is running/enabled and whether unexpected permissions changed.
2. Finish reviewing AUR PKGBUILD and source integrity before deciding whether to install rootless Docker; never change host Docker socket privileges or add user to privileged docker group reflexively.
3. Inspect Hermes config with secrets redacted: model/provider, tool enablement, command execution controls, terminal backend, mounts, credential forwarding, networking/egress; do not expose ~/.hermes/.env.
4. Use a disposable, isolated practice workspace with no AXIORYTH/other personal project mounts; validate isolation *before* any agent execution.
5. Keep learning outcomes labeled "configured", "observed", "practiced", or "passed" accurately.

## Teaching cadence
When resuming study, start with a short recap and one hands-on concept. Ask learner to predict or explain the result before running commands. Do not over-credential their skills based on copying instructions. Maintain cumulative command cheat sheets and checkpoints.

## Continuity handoff
When a conversation restarts, read this note before proposing new Hermes commands or new lessons. Ask what terminal screen is currently shown. Continue from verified results, not assumptions. No blanket authorization for agent actions or system changes is granted by this note.
