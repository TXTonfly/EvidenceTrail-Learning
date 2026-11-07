# EvidenceTrail — Project Charter

**Established:** November 6, 2026  
**Project type:** Personal engineering education / portfolio preparation  
**Current phase:** Planning

## Purpose

Develop independent competence in Python, Linux, Git, software design, debugging, testing, and technical presentation. Build toward a possible HackUTD 2027 participation goal while pursuing UT Dallas admission. Admission and hackathon eligibility are not assured.

## Product definition

A claim and source tracking app designed for education, starting with a command-line prototype. Planned growth:

- **v0.1:** Capture and display one claim and one source.
- **v0.2:** Record multiple claim/source entries.
- **v0.3:** Add manual evidence assessment labels (supporting, contradicting, insufficient).
- **v0.4:** Read and write local files safely.
- **v0.5:** Validate inputs and test expected behavior.
- **v1.0 candidate:** Demonstrate a clear, usable interface, if the foundations are strong.

These versions are *proposals*, not completed features.

## Engineering principles

- Manual-first: learner authors, runs, and debugs implementation.
- AI is a tutor, not the coder. It may review and suggest what to investigate without authoring solutions.
- No hidden external data, no AI-generated implementation, no imported AXIORYTH SI Core evaluation artifacts.
- Results and assessments remain traceable to user-entered sources.
- Avoid claiming that this app independently establishes scientific correctness.

## Education roadmap

1. **November 2026 — Python fundamentals.** Review variables, input, output, conditions, loops, lists, functions, parameters, and returns.
2. **November–December 2026 — First working script.** Build the smallest complete command-line flow.
3. **After prototype — Persistence.** Learn local file formats, loading/saving, and basic error handling.
4. **During 2027 — Testing and Git.** Add input validation, independent test cases, and meaningful commits.
5. **Before HackUTD 2027 — Presentation.** Complete an optional interface and practice a time-limited solo build.

## Working definition of done

A milestone is complete only when the learner can:
- Run it on their own laptop;
- Demonstrate the expected behavior;
- Explain the logic;
- Diagnose basic mistakes;
- Describe what is finished and what remains.

## First assignment

See [`../assignments/001-claim-recorder.md`](../assignments/001-claim-recorder.md).

## Boundaries and ownership

EvidenceTrail is a distinct, personal training project. It is not an official hackathon challenge or an AXIORYTH product. Protected AXIORYTH benchmarks, repositories, and scientific evaluation assets stay out of this project.

## Next review

Await the learner's own `evidence_trail.py` implementation, terminal output, and three sample input cases for feedback.
