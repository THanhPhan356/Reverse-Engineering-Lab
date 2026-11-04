# Reverse Engineering Lab

A personal notebook for learning low-level computing and building a foundation for reverse engineering: reading machine code, questioning assumptions, and gradually making sense of what a program does beneath its source code.

I plan to work through both [Computing 101](https://pwn.college/computing-101/) and [Reverse Engineering](https://pwn.college/program-security/reverse-engineering/) on pwn.college. Computing 101 will strengthen the foundations in machine code, memory, the stack, and control flow that connect with my university microprocessor course. I will then build on that foundation through Reverse Engineering, learning to analyze binaries and recover program logic. This repository is where I will share the knowledge, practical experience, and lessons I take away from that journey. The aim is to leave behind something useful for another learner while preserving the opportunity to discover each challenge for themselves.

## What I Will Share

- Notes on publicly available concepts and learning resources, with links and attribution to their sources.
- Practical experience with tools such as GDB and Ghidra, including mistakes, debugging habits, and lessons learned.
- Independent examples I write myself in assembly, C, C++, or Rust, together with analysis and validation.
- Reflections on what I understand, what changed my thinking, and what I still need to learn.

Every example published here will be an original, standalone demonstration outside the course challenges. I will not reproduce a challenge's distinctive logic or disguise its solution by changing names, constants, or inputs.

## Publication Commitment

**I will not publish solutions or walkthroughs for any challenge in this repository.**

Challenge-specific analysis, recovered keys, flags, solver scripts, and screenshots or pseudocode that reveal how to solve a challenge will stay out of this repository. Hiding the final answer alone does not make a walkthrough suitable for publication. My challenge solutions and detailed working notes will remain offline, separate from this public lab.

Before committing, I will check whether a note teaches a general concept through an independent example or gives away the reasoning needed to solve a course challenge. Only the former belongs here.

## Respecting pwn.college's Ground Rules

pwn.college explains that its challenges are educational material used to grade students at Arizona State University, and asks learners not to publish challenge writeups, solution videos, or livestreams. Its registration page requires this commitment:

> I have read the ground rules and commit to not publish pwn.college writeups on the internet.

Source: [pwn.college Ground Rules](https://pwn.college/register). This is a short excerpt and summary; please read the original rules directly. The same page asks that platform vulnerabilities be reported to the team rather than exploited.

I intend to respect that commitment throughout this learning journey. This is a personal learning repository, unaffiliated with pwn.college.

## Getting Started

1. Choose a general concept and write an independent demonstration of it.
2. Create an exercise directory, such as `exercises/001-loop-analysis/`.
3. Copy the [exercise template](exercise-template.md) into that directory as `README.md`.
4. Record observations, hypotheses, evidence, and lessons without including course challenge details.
5. Keep your original code and validation data alongside the notes.

## Exercise Structure

```text
exercises/001-exercise-name/
├── README.md        # Analysis and results
├── src/             # Original standalone examples or analysis helpers
├── tests/           # Test data and behavioral comparisons
└── artifacts/       # Local binaries and raw data; excluded from Git
```

Create subdirectories only when needed.

## Completion Criteria

- Explain the inputs, outputs, and main control flow.
- Distinguish confirmed findings from hypotheses that still need evidence.
- Validate conclusions using a debugger, test inputs, or a reimplementation.
- For optimization work, verify correctness before measuring performance and document the benchmark conditions.
- Confirm that the example is independent and the notes do not reveal a challenge solution.

Generated demo binaries stay in local `artifacts/` directories; this repository contains notes and original code. Course challenge binaries and private solution notes are kept outside this repository entirely.
