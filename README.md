# Balinese Calendar v0.5.0 - Calendar Library 2026

> **Balinese Calendar is a Rust library for computing Saka, Pawukon, Wewaran, Sasih, and Wariga information. Version 0.5.0 also supports astronomical day boundaries and WebAssembly targets.**

[![Platform](https://img.shields.io/badge/Platform-Rust-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v0.5.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/brunom51/balinese-calendar-rust?style=flat-square)](https://github.com/brunom51/balinese-calendar-rust)

---

<p align="center">
  <a href="https://brunom51.github.io/balinese-calendar-rust/">
    <img src="https://img.shields.io/badge/Download-Balinese%20Calendar%20Latest-brightgreen?style=for-the-badge" alt="Download Balinese Calendar">
  </a>
</p>

> **[Download Balinese Calendar v0.5.0](https://brunom51.github.io/balinese-calendar-rust/)**

---

[Download Latest Build](https://brunom51.github.io/balinese-calendar-rust/)

---

## Overview

Balinese Calendar provides a Rust-based implementation of the Balinese Saka Calendar and organizes several traditional Indonesian calendar systems into a programmable library. It covers the 210-day Pawukon cycle, Wewaran names, Sasih lunar months, Saka years, ceremony dates, and Wariga calculations.

The library is suitable for Rust software and browser applications compiled to WebAssembly. Its date calculations can use astronomical sunrise or a configurable day boundary. Climate-aware seasonal states and batch marker generation are also available for applications handling larger calendar workflows.

---

## Capabilities

- Evaluate dates within the 210-day Pawukon cycle.
- Work with the recurring Wewaran day-name cycles.
- Calculate Sasih lunar months and Saka-year values.
- Identify Rahinan ceremony dates.
- Produce Wariga classifications and compatibility results.
- Base calendar days on astronomical sunrise or a custom boundary.
- Return traditional calendar information in structured form.
- Derive seasonal states with climate-aware calculations.
- Create markers for multiple dates in a batch.
- Compile for browser use through WebAssembly.

---

## Getting Started

Clone the source repository and move into its directory:

```bash
git clone https://github.com/brunom51/balinese-calendar-rust.git
cd balinese-calendar
```

Compile the library with Cargo:

```bash
cargo build
```

For an optimized compilation, run:

```bash
cargo build --release
```

The built library can be consumed by a Rust application or used as the basis of a WebAssembly integration.

---

## Using the Library

A normal calendar calculation flow consists of the following steps:

1. Supply the date or range of dates to process.
2. Choose a calendar-day boundary, either astronomical sunrise or a custom time.
3. Request the Pawukon, Wewaran, Sasih, Saka, Rahinan, or Wariga information required by the application.
4. Export the resulting calendar values as structured data for presentation or additional processing.
5. Use batch marker generation for groups of dates.

To use the library in a browser application, compile it to WebAssembly and connect its exported calendar data to the application UI.

---

## Calendar Settings

The selected day boundary determines how calendar calculations are interpreted. Astronomical sunrise is appropriate when dates should follow local solar transitions; a custom boundary can be supplied when the host application uses different calendar-day rules.

A conceptual configuration is shown below:

```toml
[calendar]
day_boundary = "astronomical_sunrise"
location = "Indonesia"
```

The surrounding Rust application or WebAssembly wrapper determines the precise integration format. When calculating a sequence of dates, use consistent location and day-boundary settings throughout the range.

---

## Requirements

- A Rust toolchain and Cargo.
- A development environment compatible with Rust.
- WebAssembly tooling for browser-oriented builds.
- Location and date values when astronomical sunrise is part of the calculation.
- Storage needs determined by the application that embeds the library.

---

## Frequently Asked Questions

### What kind of projects can use Balinese Calendar?

The library is intended for developers creating Rust or WebAssembly applications that require Balinese Saka Calendar data and related traditional calendar computations.

### Which traditional calendars and calculations are included?

Supported data covers Pawukon, Wewaran, Sasih, Saka years, Rahinan ceremony dates, and Wariga classifications.

### Can applications define their own day boundary?

Yes. A calculation may follow astronomical sunrise or use a custom day-boundary value.

### Does the project work with WebAssembly?

Yes. WebAssembly support is provided for browser environments.

### How do I bring an existing checkout up to date?

Fetch the newest repository changes, then rebuild the library:

```bash
git pull
cargo build
```

### What should I verify when a result does not look right?

Check the date, location, selected day boundary, and any custom seasonal or calendar settings before comparing the generated output.

### How can I ask for assistance?

Create an issue in the project repository and include the version, target platform, configuration, and a concise description of the behavior you observed.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
