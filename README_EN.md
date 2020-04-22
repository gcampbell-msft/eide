# EIDE

[![](https://vsmarketplacebadge.apphb.com/version/cl.eide.svg)](https://marketplace.visualstudio.com/items?itemName=CL.eide) [![](https://vsmarketplacebadge.apphb.com/installs/cl.eide.svg)](https://marketplace.visualstudio.com/items?itemName=CL.eide) [![](https://vsmarketplacebadge.apphb.com/downloads/cl.eide.svg)](https://marketplace.visualstudio.com/items?itemName=CL.eide) [![](https://vsmarketplacebadge.apphb.com/rating/cl.eide.svg)](https://marketplace.visualstudio.com/items?itemName=CL.eide)

## Summary 📑

A 8051/STM8/ARM **IDE** with multiple toolchains for Vs Code, A Keil C51/STM32 **project migration tool**. Provide development, compilation, burning, management functions for **8051/stm8/arm** projects on vscode.

**Keil 5 version is mainly supported.**

**Only for Windows platform**

***

![preview](./res/preview/show.png)

***

## Feature 🎉

* Import Keil uVision 5 project as a vscode workspace
* Export eide project as a Keil project file (.uvprojx, .uvproj)
* Create, Open eide project
* Create, Import eide project template
* Build, Fast build project; support all of Keil's toolchains, and additional toolchains
* Generate hex, bin, elf
* Download to device board
* Serialport monitor
* manage project
* Generate `cortex-debug` debug configurations for STM32 project

***

## Toolchain support 🔨

#### ![8051](https://img.shields.io/badge/-8051_:-grey.svg) ![status](https://img.shields.io/badge/Keil_C51-done-brightgreen.svg) ![status](https://img.shields.io/badge/SDCC-done-brightgreen.svg)

#### ![ARM](https://img.shields.io/badge/-ARM_:-grey.svg) ![status](https://img.shields.io/badge/ARMCC_V5-done-brightgreen.svg) ![status](https://img.shields.io/badge/ARMCC_V6-done-brightgreen.svg) ![status](https://img.shields.io/badge/ARM_GCC-done-brightgreen.svg)

***

## Syntax support

* Standard C syntax highlights, code snippets
* 8051 C syntax highlights, code snippets
* 8051 assembly(A51) syntax highlights, code snippets

***

## Usage 📖

#### There is a simple [user's manual](https://github0null.github.io/eide-manual) for foreign friends

***

## Version changes 🔔

> #### Feedback 👉 [Github Issue](https://github.com/github0null/eide/issues)

### [v1.11.0]
- New: You can exclude unwanted source files. Excluded files are not added to the compilation process
- New: SDCC can optionally generate s19, elf
- Fixed: The GCC toolchain syntax prompts for incomplete problems
- Change: Remove options not commonly used in SDCC
- Improve: Optimize some details
***

### [v1.10.1]
- remove: Utf8 conversion options at import time
- improved: A more complete directory structure is created for the source files when imported
- improved: Open workspace directly when switching projects
- improved: Improve the use experience
- Fixed: STM8 download problem
***

### [v1.10.0]
- New: STLink flash support
- New: downloads of related tools
- Optimization: build the output of the tool
- Fixed: some other problems
***

## Attention 🚩
  + **The multi-objective Keil project is not supported**
  + **Make sure that JLink is installed on your computer before using the ARM burn tool**
  + **Import keil project will be failed if Keil uVision's version is tool low**
  + **Import process: source files in Keil project structure will be copied to eide project directory, header search path, macro, compile configuration inherited from Keil**