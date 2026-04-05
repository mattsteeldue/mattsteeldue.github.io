---
title: "vForth"
permalink: /vforth/
layout: single
author_profile: true
toc: true
---

### What is vForth?

**vForth** is a Forth system I have been developing since 1990, primarily targeted at the **ZX Spectrum 48K**, **ZX Spectrum Next**, and their emulators.

The project has two main branches:

- **vForth** – the classic 48K core system
- **vforth-next** – the actively developed version optimized for the **ZX Spectrum Next**

### Key Features

- Almost **ANS Forth** compliant with many useful extensions
- **Fast inner interpreter** using Direct Threaded Code
- Built-in assembler for Z80 and Z80N (Spectrum Next extended opcodes)
- Support for block-based and file-based I/O
- Very **small memory footprint** – ideal for 8-bit constrained environments
- Full interactive REPL for live development
- Modular design – easy to extend with new words and libraries
- Complete source code and documentation included in the repository

### vforth-next for ZX Spectrum Next

This is the main focus of current development. It fully leverages the ZX Spectrum Next hardware:

- Z80N instruction set and extended opcodes
- Layer 2 graphics mode support
- Tilemap and sprite engine integration
- DMA and copper support
- NextOS file system access
- Sound primitives (AY and TurboSound FM)
- Easy integration with emulators such as CSpect

### Current Status (April 2026)

- Core engine is stable and actively used
- Regular updates aligned with new Spectrum Next firmware
- Growing collection of example programs and utilities
- Released under the **MIT license**

### Active Community

Most of my latest updates, releases, bug reports, and user questions about **vForth-Next** are shared in the Facebook group I administer:

**[Forth on the ZX Spectrum, Next and 48K](https://www.facebook.com/groups/1326098804442710)**

This is the liveliest place for:
- Real-time help and technical discussions
- Sharing demos and code
- Hardware integration topics (Layer 2, sprites, DMA, sound, etc.)
- Announcements of new vForth releases

Everyone interested in Forth on Spectrum machines is welcome to join.

### Links & Resources

- **[vforth-next Repository](https://github.com/mattsteeldue/vforth-next)**
- **[Wiki](https://github.com/mattsteeldue/forth-next/wiki)** (documentation and guides)
- **[Documentation folder](https://github.com/mattsteeldue/vforth-next/tree/master/doc)** (PDF reference manual)
- **[Facebook Community](https://www.facebook.com/groups/1326098804442710)**

**Want to get started?**  
Clone the repository or download the latest release from GitHub and follow the instructions in the README.  
Feedback, questions, and contributions are always welcome — both on GitHub and in the Facebook group.
