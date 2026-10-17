# Reverse Engineering Lab

A personal lab for practicing binary analysis, recovering program logic, and reimplementing functionality in C, C++, or Rust.

## Getting Started

Course and exercises: [pwn.college — Reverse Engineering](https://pwn.college/program-security/reverse-engineering/).
Start with **Terrible Token (Easy)**, then work through progressively harder challenges.

1. Create an exercise directory, such as `exercises/001-terrible-token/`.
2. Copy the [exercise template](exercise-template.md) into that directory as `README.md`.
3. Record observations, hypotheses, and evidence before reading a solution.
4. Keep your reimplementation and validation data alongside the exercise notes.

## Exercise Structure

```text
exercises/001-exercise-name/
├── README.md        # Analysis and results
├── src/             # Original reimplementation or analysis helpers
├── tests/           # Test data and behavioral comparisons
└── artifacts/       # Local binaries and raw data; excluded from Git
```

Create subdirectories only when needed.

## Completion Criteria

- Explain the inputs, outputs, and main control flow.
- Distinguish confirmed findings from hypotheses that still need evidence.
- Validate conclusions using a debugger, test inputs, or a reimplementation.
- For optimization work, verify correctness before measuring performance and document the benchmark conditions.

Exercise binaries stay in local `artifacts/` directories; this repository contains notes and original code.
