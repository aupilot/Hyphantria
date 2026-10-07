# Hyphantria

**A new way of PCB design. Built by a professional electronics designer for fellow engineers.**

Hyphantria is a PCB design environment for macOS built around a simple idea:

> **PCB design should be about engineering decisions, not repetitive CAD work.**

Hyphantria is **not YAC — Yet Another CAD**. It is not intended to reproduce the traditional PCB CAD workflow with a different user interface. Instead, Hyphantria explores a new way of designing electronics where AI handles much of the repetitive, time-consuming work that engineers have traditionally had to perform manually.

You remain the engineer. Hyphantria takes care of the boring parts.

## A Different Workflow

Traditional PCB design often involves a surprising amount of work that has little to do with the actual engineering problem:

- searching for datasheets
- extracting component parameters
- creating schematic symbols
- creating and checking footprints, or matching packages and manufacturer naming conventions
- finding reference designs
- translating reference circuits into schematics
- adjusting components for required operating modes
- maintaining component libraries
- repeatedly entering information that already exists elsewhere

Hyphantria is designed to automate as much of this work as practical.

Instead of treating AI as an optional assistant bolted onto a conventional CAD package, **AI is part of the workflow itself**.

The goal is simple: spend less time operating CAD software and more time designing electronics.

## Unique Features

Hyphantria is not simply a conventional PCB CAD package with AI added on top. Several parts of the workflow are designed differently from the beginning.

### Tuners

Many circuits require component values to be calculated or adjusted for a particular operating point. Switching regulators, LED drivers, filters, timing circuits and similar designs often require repeatedly moving between the schematic, datasheet equations and external calculators.

Hyphantria introduces **Tuners** — interactive tools associated with a circuit or component that allow important operating parameters to be adjusted directly as part of the design workflow.

Instead of manually recalculating a group of resistors, capacitors or inductors, a Tuner can understand the relationships between them and help select appropriate values for the required operating conditions.

The engineer specifies **what the circuit should do**; Hyphantria helps with the repetitive calculations required to make it happen.

### Automatic Versions

Hyphantria follows the macOS document model rather than the traditional **Save / Save As / project-copy** workflow.

Changes are automatically preserved, allowing previous versions of a design to be revisited without requiring the engineer to continually create files such as:

`Board_v3_final_really_final_2`

Version history is intended to be part of the normal design process rather than a separate version-control task.

### Visual Version Comparison

Previous versions are more useful when you can understand **what actually changed**.

Hyphantria is designed to provide graphical comparison of design versions, making it possible to inspect changes to schematics and PCB layouts visually rather than comparing opaque binary project files.

This makes experimentation safer: try an idea, compare the result with an earlier version, and return to the previous design when necessary.

### AI Reference-Design Adoption

Reference designs should be reusable engineering knowledge, not pictures that have to be manually copied.

Hyphantria uses AI to interpret manufacturer reference designs and help turn them into editable circuitry. The goal is to reduce the work involved in finding a suitable reference design, understanding it, recreating it in CAD and adapting it to the required operating conditions.

### Intelligent Component Library

Component information should not have to be entered repeatedly.

Hyphantria maintains reusable components, packages and footprints while understanding that manufacturers frequently use different names for electrically or mechanically equivalent packages.

AI-assisted part creation can extract information from datasheets and reuse existing packages and footprints where appropriate instead of creating another slightly different copy of the same thing.

### Native macOS Workflow

Hyphantria is built specifically for macOS. Rather than maintaining a cross-platform abstraction layer, the project takes advantage of the native Mac environment and Apple frameworks where they provide a better experience.

The intention is to create a PCB design tool that feels like a Mac application. 
Hyphantria makes use of native macOS concepts such as automatic document saving and version history, while taking advantage of Apple's graphics and hardware-acceleration technologies.

## AI-Assisted by Design

Hyphantria can use AI to help with tasks such as component discovery, datasheet interpretation, parameter extraction, part creation and reference-design analysis.

AI-generated information is integrated into the design workflow rather than simply presented in a chat window.

This does **not** mean that AI replaces engineering judgement.

Datasheets, manufacturer recommendations, electrical rules and the engineer's own decisions remain authoritative. AI is used to accelerate the work around those decisions.

## Human-Controlled Engineering

Automation should remove repetitive work — not remove control.

Hyphantria is designed so that important engineering decisions remain visible and editable. AI-generated results should be treated in the same way as work produced by a junior engineer: extremely useful, often fast, but something that should still be reviewed where correctness matters.

The objective is not:

**"Let AI design my PCB."**

It is:

**"Let AI do the tedious work so I can design my PCB."**


## Work in Progress

Hyphantria is under active development and is currently at the **alpha stage**. As the project develops, file formats and AI-assisted workflows may change. Designs created with development or preview versions should therefore be treated accordingly.

The binary distribution may contain incomplete features, experimental workflows and functionality that changes between releases.

Do not assume that AI-generated component data, footprints, electrical parameters or design recommendations are always correct without verification.

For production hardware, always verify critical information against the original component datasheet and manufacturer documentation.

## Binary Distribution

This package contains a pre-built version of Hyphantria for macOS.

Bug reports and feedback are particularly valuable when they concern:

- problematic component or package identification
- symbol or footprint generation
- incorrect AI extraction of reference designs
- missing or incorrect Tuners
- PCB or schematic workflow friction
- cases where Hyphantria requires unnecessary repetitive work

The last category is especially important.

**If you find yourself repeatedly doing something boring, there is a good chance Hyphantria should eventually be doing it for you.**

---

**Hyphantria**

*Not another CAD. A different way to design electronics.*
