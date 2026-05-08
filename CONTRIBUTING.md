# Contributing to Fregata

Thanks for your interest in helping out. Fregata is a small project and the most useful contributions are usually not code.

## About this repository

This repository is the **community hub** for Fregata. It does not contain Fregata's source code.

- Fregata's macOS runtime, Apple Silicon optimizations, native CoreML detector, process supervisor, and the Fregata `.app` bundle are **proprietary** and live in a separate private repo.
- The upstream open-source detection engine is [Frigate](https://github.com/blakeblackshear/frigate). Bugs and features that aren't Fregata-specific belong upstream.

## Ways you can help

### Report bugs

[Open a bug report](https://github.com/3rdBitLabs/Fregata/issues/new/choose) using the issue form. The form prompts for the version, system info, and logs we need to reproduce. The more specific you are, the faster we can fix it.

For security bugs, see [SECURITY.md](SECURITY.md). Do not file public issues for vulnerabilities.

### Request features

[Open a feature request](https://github.com/3rdBitLabs/Fregata/issues/new/choose). Lead with the problem you're trying to solve, not the implementation. Concrete use cases are far more persuasive than abstract wishes.

Search existing issues first. If your idea is already filed, add a thumbs-up or a comment with your specific use case rather than opening a duplicate.

### Share benchmarks

If you've run Fregata on real hardware with real cameras, post your results in the [Benchmarks discussion category](https://github.com/3rdBitLabs/Fregata/discussions). Use the benchmark template so the data is comparable across posts. Real-world numbers help other users size their hardware.

### Help other users

The [Discussions](https://github.com/3rdBitLabs/Fregata/discussions) tab is where users ask questions and trade tips. If you've solved a problem yourself, posting your solution there saves the next person hours.

### Improve documentation

Docs live at [docs.fregata.app](https://docs.fregata.app). If you find something unclear, missing, or wrong, open an issue here describing the gap and we'll get it into the docs.

## Issue and discussion etiquette

- **Search first.** Most questions have been asked before.
- **One issue per bug.** Don't bundle unrelated problems into a single report.
- **Stay on topic.** Frigate-upstream questions belong on the [Frigate](https://github.com/blakeblackshear/frigate) repo.
- **Be patient.** Fregata is maintained by a small team. We'll get to your issue.
- **Be kind.** See the [Code of Conduct](CODE_OF_CONDUCT.md).

## Triage labels

Maintainers use a small label set to triage:

- `bug` / `enhancement` - what kind of issue it is.
- `needs-info` - waiting on the reporter for more detail.
- `confirmed` - we've reproduced it.
- `upstream` - the issue belongs in Frigate, not Fregata.
- `wontfix` - we've decided not to act on it (with a comment explaining why).

If your issue gets `needs-info`, please respond. Issues with no response after 30 days may be closed.
