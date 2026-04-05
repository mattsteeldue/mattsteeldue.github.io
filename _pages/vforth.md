---
title: "vForth"
permalink: /vforth/
layout: single
author_profile: true
toc: true
---

### What is vForth?

**vForth** is a Forth system I have been developing since 1990, specific for ZX Spectrum 48K, ZX Spectrum Next, and their emulators.

The project has two main branches:
- **vForth** – the old 48K core system
- **vforth-next** – optimized version and tools specifically for the **ZX Spectrum Next**

### Key Features

- Support for block-based and file-based I/O
- **ANS Forth** (almost) compliant with many extensions
- **Fast inner interpreter** (Direct Threaded Code on supported architectures)
- Built-in assembler for Z80 / Z80N (Spectrum Next)
- **Small memory footprint** – ideal for constrained environments
- **Interactive development** environment with full REPL
- Modular design – easy to add new words and libraries
- **Documentation** and source code included in the repo

### vforth-next for ZX Spectrum Next

This is the most actively developed branch. It takes full advantage of the ZX Spectrum Next hardware:

- Z80N instruction set support (extended opcodes)
- Layer 2 graphics mode support
- Tilemap and sprite engine integration
- DMA and copper support
- NextOS file system access
- Sound (AY and TurboSound FM) primitives
- Easy integration with popular Spectrum Next tools (CSpect emulator, etc.)

#### Z80N Instruction Support (Expanded)

The built-in **assembler vocabulary** fully recognises and supports the complete **Z80N extended instruction set** of the ZX Spectrum Next FPGA core.

This gives you direct access to powerful new opcodes that are not present on a classic Z80:

- **16-bit immediate arithmetic**: `ADD HL/DE/BC,nn`, `ADC/SUB/SBC HL/DE/BC,nn`
- **8-bit multiply**: `MUL` (unsigned 8×8 → 16-bit result)
- **Enhanced bit and nibble operations**: `SWAPNIB`, `MIRROR A`, `PIXELAD`, `PIXELDN`
- **Next-specific helpers**: `SETA`, `TEST`, `LD (HL),nnnn` (extended immediate load), new rotate/shift variants
- **Improved control-flow instructions** and several undocumented Z80 behaviours now officially supported

These instructions are available directly in the Forth-style assembler notation (e.g. `MUL`, `ADDHLNN`, `SWAPNIB`, etc.).  
They allow significantly faster code for:
- graphics routines (Layer 2, sprites, tilemaps)
- sound and copper list handling
- math-heavy or performance-critical inner loops

Thanks to full Z80N support, vforth-next can produce code that runs noticeably faster than classic Z80 Forth systems on the same hardware.

### Current Status (April 2026)

- Core engine stable and actively used
- Regular updates for new Spectrum Next firmware features
- Growing library of example programs and utilities
- Open source under MIT license

### Active Community

Most of my latest updates, discussions, bug reports, and user questions about **vForth-Next** happen in the Facebook group I administer:

**[Forth on the ZX Spectrum, Next and 48K](https://www.facebook.com/groups/1326098804442710)**

This is currently the most active place for:
- Real-time help and questions about vForth
- Sharing demos and code
- Discussions about ZX Spectrum Next hardware integration (Layer 2, sprites, DMA, sound, etc.)
- Announcements of new vForth releases

You are welcome to join and participate — everyone interested in Forth on Spectrum machines is invited.

### Links
- [vforth-next Repository](https://github.com/mattsteeldue/vforth-next)
- [Facebook Community](https://www.facebook.com/groups/1326098804442710)

Feedback and contributions are always appreciated, whether on GitHub or in the group.
If you are interested in Forth, retro computing, or the ZX Spectrum Next, feel free to explore the code, try the system, or contribute ideas.

---

**Want to get started?**  
Clone the repository, or download the most recent .zip archive in the "download" section and follow the instructions in the README. There is a group of Wiki pages too.
Feedback and pull requests are always welcome!
