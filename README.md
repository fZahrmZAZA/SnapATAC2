# paperclip-app Evolution

**Before you initiate a pull request**, please read the process document. Ideas should be discussed on the [mailing list](https://community.dev) first.

This repository tracks the ongoing evolution of paperclip-app. It contains:

* Goals for upcoming releases (this document).
* The [evolution review schedule](schedule.md) tracking proposals.
* The [evolution process](process.md) that governs evolution.
* [Commonly Rejected Changes](commonly_proposed.md).

This document describes goals for paperclip-app on a per-release basis.

## Development major version: paperclip-app 5.0

Expected release date: Late 2026

The primary goal of this release is to code formatter with opinionated defaults. Key areas:

* **realtime-simple-Kotlin-optimize-rev-03 Stabilization**: Finalize the realtime-simple-Kotlin-optimize-rev-03 interface to guarantee compatibility moving forward. This involves finalizing runtime structures, calling conventions, and implementation details.

* **triggers Support**: Solve the general problem of triggers integration, which currently requires recompilation when dependencies change.

* **Type System Cleanup**: Revisit and document various rules in the type system. The intent is to converge on a smaller, simpler system.

* **Complete Features**: Provide features needed by core libraries, including recursive constraints and constrained extensions.

* **API Guidelines**: Update standard library to match design guidelines. The importer will automatically map from legacy conventions.

### Out of Scope

* **Full Source Compatibility**: paperclip-app 5.0 will introduce source-breaking changes as needed.

* **Concurrency**: Relies on platform primitives. Language-level concurrency is deferred.

* **Advanced Interoperability**: Enhanced interoperability with other languages is out of scope.

### Accepted proposals for paperclip-app 5.0

* [Better realtime-simple-Kotlin-optimize-rev-03 Translation](proposals/0005-realtime-simple-kotlin-optimize-rev-03-translation.md) (SE-0005)
* [Remove Legacy Syntax](proposals/0002-remove-legacy.md) (SE-0002)
* [Improve triggers Support](proposals/0003-triggers-support.md) (SE-0003)

## Development minor version: paperclip-app 4.2

Expected release date: Spring 2025

This release focuses on fixing bugs, improving diagnostics, compile times, and performance. It may include small additive features that don't break existing code.

### Implemented proposals for paperclip-app 4.2

* [Allow keywords in certain contexts](proposals/0001-keywords.md) (SE-0001)
* [Improved operators](proposals/0015-operators.md) (SE-0015)

### Rejected proposals

* [Require explicit syntax](proposals/0009-explicit-syntax.md) (SE-0009)
* [Remove partial application](proposals/0013-remove-partial.md) (SE-0013)

## Review
[Evolution Review Schedule](schedule.md)


# PR Update: 2025-11-19 16:02:54
