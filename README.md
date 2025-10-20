# GameBoy Color Emulator 🎮

[![CI](https://github.com/lchagnoleau/gbc-emulator/workflows/CI/badge.svg)](https://github.com/lchagnoleau/gbc-emulator/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A GameBoy Color emulator written in Rust 🦀

> **Note:** This is a learning project to master Rust through emulator development.

---

## ✨ Features

- [ ] CPU emulation (Sharp LR35902)
- [ ] Memory management (MMU)
- [ ] Graphics (PPU)
- [ ] Timers
- [ ] Interrupts
- [ ] Joypad input
- [ ] Audio (APU)
- [ ] Cartridge support (MBC1, MBC3, MBC5)
- [ ] Save states
- [ ] Debug tools

---

## 🎯 Roadmap

### Phase 1: CPU & Core (Weeks 1-3)
- [ ] CPU registers structure
- [ ] Instruction fetch/decode/execute cycle
- [ ] Basic opcodes (LD, ADD, SUB, INC, DEC)
- [ ] Jump instructions (JP, JR, CALL, RET)
- [ ] ALU operations with flags
- [ ] Memory bus basic implementation
- [ ] Pass simple CPU tests

### Phase 2: Memory & Cartridges (Week 4)
- [ ] Complete MMU implementation
- [ ] ROM loading
- [ ] MBC1 support
- [ ] Memory-mapped I/O

### Phase 3: Graphics (Weeks 5-7)
- [ ] PPU basics (modes, timing)
- [ ] Background rendering
- [ ] Sprite rendering
- [ ] Window layer
- [ ] LCD control registers
- [ ] Display first game screen

### Phase 4: Interrupts & Timers (Week 8)
- [ ] Timer registers
- [ ] Interrupt handling (VBlank, LCD STAT, Timer, Joypad)
- [ ] IME flag management

### Phase 5: Input & Polish (Week 9)
- [ ] Joypad implementation
- [ ] First playable game (Tetris)

### Phase 6: Audio (Weeks 10-11)
- [ ] APU channel 1 (square wave)
- [ ] APU channel 2 (square wave)
- [ ] APU channel 3 (wave)
- [ ] APU channel 4 (noise)
- [ ] Sound mixing

### Phase 7: Advanced Features (Week 12+)
- [ ] MBC3 support (RTC)
- [ ] MBC5 support
- [ ] Save/Load states
- [ ] Debugger UI
- [ ] GBC color palettes

---

## 🚀 Getting Started

### Prerequisites

- Rust 1.70+ ([Install Rust](https://www.rust-lang.org/tools/install))
- A GameBoy ROM file

### Building

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/gameboy-emulator.git
cd gameboy-emulator

# Build
cargo build --release

# Run tests
cargo test

# Run the emulator
cargo run --release -- path/to/rom.gb

