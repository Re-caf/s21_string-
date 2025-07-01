# Project: Custom String Library Implementation (s21_string)

## Part 1: string.h Functions
- **Task**: Reimplement `string.h` functions with prefix `s21_`
- **Requirements**:
  - C11 standard, GCC compiler
  - Static library: `s21_string.a` (header: `s21_string.h`)
  - POSIX.1-2017 compliance, Google C++ Style
  - 80%+ test coverage via Check (vs standard `string.h`)
  - Makefile targets: `all`, `clean`, `test`, `gcov_report`
- **Constraints**:
  - No legacy functions or standard library usage
  - ASCII z-strings only
  - Custom error handling (no `sys_nerr`/`sys_errlist`)

## Part 2: Basic sprintf
- **Implementation**: Partial `sprintf` in `s21_string.h`
- **Supported**:
  - Specifiers: `%c`, `%d`, `%f`, `%s`, `%u`, `%%`
  - Flags: `-`, `+`, space
  - Width/Precision: `(num)`, `.(num)`
  - Length: `h`, `l`

## Part 3: Extended sprintf (Bonus)
- **Additional Support**:
  - Specifiers: `%g`, `%G`, `%e`, `%E`, `%x`, `%X`, `%o`, `%p`
  - Flags: `#`, `0`
  - Dynamic: `*` width/precision
  - Length: `L`

## Part 4: sscanf (Bonus)
- **Implementation**: Full `sscanf` in `s21_string.h`
- **Scope**: Complete formatting (flags, width, modifiers)
