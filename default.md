# AGENTS.md - NuttX Project Guide

## Project Layout

This project consists of multiple individual git repositories managed via repo tool. For the complete manifest, refer to manifest/default.xml

### Core Repositories

- **nuttx/** - NuttX kernel and operating system (apache/nuttx)
- **nuttx-apps/** - Application layer with examples and tools (apache/nuttx-apps)
- **boards/** - Board-specific configurations and board support packages (custom)
- **nuttx-apps/external/** - External application dependencies

### External Components

- **nuttx-apps/interpreters/wamr/wamr/** - WebAssembly Micro Runtime (bytecodealliance/wasm-micro-runtime)
- **nuttx-apps/graphics/lvgl/lvgl/** - Light and Versatile Graphics Library (lvgl/lvgl)
- **nuttx-apps/external/crates/** - Rust crates index for NuttX
- **manifest/** - Repo tool configuration directory

## Critical Rules
- **NEVER** try to run or test unless explicitly requested
- **MUST** set the **working directory parameter** properly for shell commands; never use `cd` chains
- **MUST** limit output with `head`/`tail` (avoid full logs/compilations)
- **MUST REVIEW and SELECT** proper skills before working
