# Phase 1: C Fundamentals (8 weeks, ~10 hrs/week)

**Weekly rhythm:** 4 hrs study · 4 hrs exercises · 1 hr deliberate debugging · 1 hr notes + Git commits

**Core resources (pick one main text, use the rest as reference):**
- *C Programming: A Modern Approach*, K. N. King (best structured main text)
- *The C Programming Language*, Kernighan & Ritchie (concise reference)
- *Beej's Guide to C* (free online) and *Modern C*, Jens Gustedt (free online)
- Exercism C track for extra practice problems
- Unity (ThrowTheSwitch) for unit testing in Weeks 7-8

---

## Weeks 1-2: Core language and memory
- [ ] Types, operators, control flow, functions, arrays
- [ ] Use fixed-width types (`uint8_t`, `int32_t`) by default
- [ ] Understand integer overflow, signed vs. unsigned, implicit conversions
- [ ] Input handling with `fgets` + `sscanf` (avoid bare `scanf`)
- [ ] Compile with `-Wall -Wextra` and fix every warning
- [ ] **Mini-project:** CLI tool that parses and validates user input
- [ ] Commit code + short write-up

## Weeks 3-4: Pointers and memory layout
- [ ] Pointers, pointer arithmetic, arrays vs. pointers
- [ ] `const` correctness, strings as `char` arrays
- [ ] Stack vs. heap vs. static storage
- [ ] Pointer to pointer: when and why
- [ ] **Mini-project:** implement `memcpy`, `strlen`, `strcmp`
- [ ] **Mini-project:** fixed-size ring buffer (no `malloc`)
- [ ] Order and set up an STM32 Nucleo board; confirm it connects to your PC
- [ ] Commit code + short write-up

## Weeks 5-6: Bits, structs, and embedded idioms
- [ ] Bitwise operators: set, clear, toggle, test bits with masks and shifts
- [ ] Structs, unions, enums; why bitfields are risky across compilers
- [ ] `volatile`, `static`, `inline`
- [ ] Function pointers and callback tables
- [ ] **Mini-project:** state machine (e.g., button debouncer or command parser) driven by a table of function pointers
- [ ] Commit code + short write-up

## Weeks 7-8: Multi-file C and toolchain
- [ ] Headers, include guards, `extern`, translation units
- [ ] What the preprocessor, compiler, and linker each do
- [ ] Makefile or CMake basics
- [ ] Set up GCC alongside MSVC (WSL2 or MSYS2)
- [ ] Run a static analyzer (e.g., `cppcheck`) on your code
- [ ] **Mini-project:** split ring buffer + state machine into modules with unit tests
- [ ] Blink an LED on the Nucleo (any method) to verify the toolchain
- [ ] Commit code + short write-up

---

## Exit criteria (can do without looking things up)
- [ ] Explain a pointer to a pointer and when to use one
- [ ] Set, clear, and test specific bits in a register-like variable
- [ ] Trace data flow through an unfamiliar ~200-line C program
- [ ] Diagnose a segfault or off-by-one with a debugger, not print statements
- [ ] Build a multi-file project from the command line with warnings clean

When all boxes are checked, move to **Phase 2: bare-metal STM32**.