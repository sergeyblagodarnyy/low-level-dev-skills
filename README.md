# low-level-dev-skills

A curated suite of AI agent skills for systems and low-level programming — C/C++, bare-metal firmware, Linux kernel/driver development, computer architecture, compiler internals, HPC, and more. These skills provide expert guidance for compilers, debuggers, profilers, build systems, sanitizers, low-level programming, embedded development, observability, virtualization, security, and WebAssembly.

**[View on skills.sh](https://skills.sh/mohitmishra786/low-level-dev-skills)**

## Installation

Install all skills with a single command:

```bash
npx skills add mohitmishra786/low-level-dev-skills --all
```

Or select specific skills interactively:

```bash
npx skills add mohitmishra786/low-level-dev-skills
```

Install globally to make skills available in all projects:

```bash
npx skills add mohitmishra786/low-level-dev-skills --all --global
```

### Install by language / tag

Install specific skill bundles using the `--skill` flag (space-separated list):

```bash
# C/C++ toolchain (compilers, debuggers, build systems, profilers)
npx skills add mohitmishra786/low-level-dev-skills --skill gcc clang llvm cross-gcc cmake make ninja static-analysis gdb lldb core-dumps linux-perf valgrind flamegraphs strace-ltrace heaptrack sanitizers fuzzing elf-inspection linkers-lto binutils dynamic-linking assembly-x86 assembly-arm interpreters simd-intrinsics memory-model cpu-cache-opt modern-c-cpp-standards formal-verification riscv-vector tracing-profilers

# Embedded (RTOS, OpenOCD, linker scripts, bare-metal)
npx skills add mohitmishra786/low-level-dev-skills --skill openocd-jtag linker-scripts baremetal-startup mmio-and-bit-manipulation interrupts-and-exceptions-baremetal gpio-baremetal uart-serial-baremetal spi-i2c-baremetal dma-baremetal stm32-baremetal low-power-embedded

# Bare-metal focused
npx skills add mohitmishra786/low-level-dev-skills --skill baremetal-startup mmio-and-bit-manipulation interrupts-and-exceptions-baremetal peripherals-from-datasheet gpio-baremetal uart-serial-baremetal spi-i2c-baremetal timers-pwm-baremetal adc-dac-baremetal dma-baremetal stm32-baremetal datasheet-and-refmanual-reading bootloaders-embedded low-power-embedded

# Kernel & driver development
npx skills add mohitmishra786/low-level-dev-skills --skill linux-kernel-architecture kernel-memory-management kernel-concurrency device-tree platform-device-model writing-char-drivers bus-drivers-i2c-spi kernel-debugging-advanced kernel-internals device-drivers

# Computer architecture
npx skills add mohitmishra786/low-level-dev-skills --skill cpu-pipelines-and-hazards memory-hierarchy-and-caches virtual-memory-paging-and-tlb abi-and-calling-conventions branch-prediction-and-speculation

# Observability (eBPF, binary hardening)
npx skills add mohitmishra786/low-level-dev-skills --skill ebpf binary-hardening sched-ext

# WebAssembly
npx skills add mohitmishra786/low-level-dev-skills --skill wasm-emscripten wasm-wasmtime

# The core essentials (compiler + debugger + profiler for all languages)
npx skills add mohitmishra786/low-level-dev-skills --skill gcc clang gdb lldb linux-perf cmake

# Build systems only
npx skills add mohitmishra786/low-level-dev-skills --skill cmake make ninja static-analysis build-acceleration include-what-you-use

# Profilers and performance tools
npx skills add mohitmishra786/low-level-dev-skills --skill linux-perf valgrind flamegraphs strace-ltrace heaptrack intel-vtune-amd-uprof hardware-counters

# Runtime safety (sanitizers, fuzzing, Miri, binary hardening)
npx skills add mohitmishra786/low-level-dev-skills --skill sanitizers fuzzing binary-hardening

# Binary analysis (ELF, linkers, dynamic linking, binutils, DWARF)
npx skills add mohitmishra786/low-level-dev-skills --skill elf-inspection linkers-lto binutils dynamic-linking dwarf-debug-format

# Kernel internals and drivers
npx skills add mohitmishra786/low-level-dev-skills --skill kernel-internals device-drivers kernel-debugging kernel-testing os-dev-scratch

# Allocators and NUMA
npx skills add mohitmishra786/low-level-dev-skills --skill custom-allocators numa-programming

# Compiler internals (frontend, IR, passes, codegen, MLIR, JIT)
npx skills add mohitmishra786/low-level-dev-skills --skill compiler-frontend llvm-passes llvm-ir-and-passes compiler-optimizations-deep code-generation-and-backends jit-compilation

# Virtualization
npx skills add mohitmishra786/low-level-dev-skills --skill containers-internals

# HPC and parallel programming
npx skills add mohitmishra786/low-level-dev-skills --skill openmp mpi rdma-verbs

# Security and reverse engineering
npx skills add mohitmishra786/low-level-dev-skills --skill memory-safe-c-cpp

# Platform-specific (ARM SVE, RISC-V privileged, Apple Silicon)
npx skills add mohitmishra786/low-level-dev-skills --skill arm-sve riscv-privileged

# Emerging languages (Carbon, Hare)
npx skills add mohitmishra786/low-level-dev-skills --skill carbon-lang hare-lang
```

## Supported Agents

Skills work with 30+ AI coding agents:

| Agent | Skill Directory |
|-------|-----------------|
| [Claude Code](https://claude.com/product/claude-code) | `.claude/skills/` |
| [Cursor](https://cursor.sh) | `.cursor/skills/` |
| [Codex](https://openai.com/codex) | `.codex/skills/` |
| [GitHub Copilot](https://github.com/features/copilot) | `.github/copilot/skills/` |
| [Cline](https://cline.bot) | `.cline/skills/` |
| [Windsurf](https://codeium.com/windsurf) | `.windsurf/skills/` |
| [Gemini CLI](https://gemini.google.com) | `.gemini/skills/` |
| [Kilo](https://kilo.ai) | `.kilo/skills/` |

And many more including: Amp, Antigravity, Augment, Droid, Goose, Kiro CLI, OpenCode, Roo, Trae, VSCode, and others.

## Usage Examples

After installation, invoke skills in your AI agent:

### C/C++ toolchain
```
/gcc How do I enable link-time optimization?
/gdb Set a conditional breakpoint in GDB
/cmake What's the modern way to find packages?
/static-analysis Run clang-tidy on my whole project
/dynamic-linking My binary can't find its shared library
/cpp-modules How do I write a C++20 named module?
/cpp-templates How do I use concepts as constraints?
/binary-hardening How do I add RELRO and PIE to my binary?
```

### Embedded and bare-metal
```
/openocd-jtag Connect GDB to my STM32 via OpenOCD
/linker-scripts Place my code in CCM RAM with a linker script
/baremetal-startup Fix .bss init so globals are zero before main
/stm32-baremetal Scaffold CMSIS-only STM32F4 without HAL
/bootloaders-embedded Jump from bootloader to app at 0x08010000
```

### Kernel drivers and architecture
```
/linux-kernel-architecture Where does the page fault handler live?
/device-tree Write a DTS node for an I2C sensor with interrupt
/writing-char-drivers Add ioctl to my platform driver
/cpu-pipelines-and-hazards Break a RAW hazard in this hot loop
/llvm-ir-and-passes Explain what -O2 changed in this LLVM IR
```

### Observability and security
```
/ebpf Write a bpftrace one-liner to trace system calls
/binary-hardening Check my binary with checksec
/wasm-emscripten Compile my C library to WebAssembly
/wasm-wasmtime Embed wasmtime in my Rust application
```

### Profiling & analysis
```
/linux-perf Generate a flame graph from perf data
/strace-ltrace Trace system calls to find a missing config file
/sanitizers Which sanitizer should I use for memory leaks?
/valgrind How do I suppress known false positives?
/heaptrack Find allocation hotspots in my C++ server
/intel-vtune-amd-uprof Analyze pipeline stalls in my hot function
/hardware-counters Measure cache miss rate with perf stat
```

### Advanced debugging
```
/concurrency-debugging Read a TSan data race report
/debug-optimized-builds Why does GDB say "value optimized out"?
/dwarf-debug-format Set up debuginfod for automatic symbols
```

### HPC
```
/openmp Parallelize this loop with a dynamic schedule
/mpi Debug a deadlock in my MPI_Send/Recv pattern
```

### Kernel and systems
```
/kernel-internals Interpret /proc/meminfo during memory pressure
/device-drivers Write a platform_driver with threaded IRQs
```

### Security and platform
```
/arm-sve Write a vector-length agnostic SAXPY kernel
```

## Skills

### C/C++ Compilers (7 skills)

| Skill | Purpose |
|-------|---------|
| `gcc` | GCC flags, optimization levels, warnings, diagnostics |
| `clang` | Clang/LLVM tooling, diagnostics, sanitizer integration |
| `llvm` | LLVM IR, passes, opt/llc pipeline |
| `cross-gcc` | Cross-compilation triplets, sysroots, embedded targets |
| `cpp-modules` | C++20 modules: named modules, header units, CMake integration |
| `cpp-templates` | Template error reading, concepts, requires-clauses, Templight |
| `modern-c-cpp-standards` | C23/C2y features, GCC 15/16 default changes, C++26 reflection and contracts, hardening |

### Debuggers (6 skills)

| Skill | Purpose |
|-------|---------|
| `gdb` | GDB sessions, breakpoints, reverse debug, remote debug |
| `lldb` | LLDB commands, GDB migration, IDE integration |
| `core-dumps` | Core file analysis, debuginfod, production crash triage |
| `concurrency-debugging` | TSan reports, deadlock triage, happens-before reasoning |
| `debug-optimized-builds` | RelWithDebInfo, -Og, inlined frames, "value optimized out" |
| `dwarf-debug-format` | DWARF sections, dwarfdump, split DWARF, debuginfod |

### Profilers (8 skills)

| Skill | Purpose |
|-------|---------|
| `linux-perf` | perf record/report, flame data, kernel symbols |
| `valgrind` | memcheck, cachegrind, suppression files |
| `flamegraphs` | perf-to-SVG pipeline, reading frames |
| `strace-ltrace` | Syscall and library call tracing, ENOENT/EPERM triage |
| `heaptrack` | Heap allocation profiling, leak detection, hotspots |
| `intel-vtune-amd-uprof` | VTune hotspots, microarchitecture analysis, roofline model |
| `hardware-counters` | perf stat -e, PAPI, cache miss rates, IPC analysis |
| `tracing-profilers` | Perfetto SDK + trace processor SQL, Tracy zones and headless capture |

### Build Systems (6 skills)

| Skill | Purpose |
|-------|---------|
| `make` | Idiomatic Makefiles, pattern rules, dep generation |
| `cmake` | Modern CMake, targets-first, toolchain files |
| `ninja` | Ninja diagnosis, parallelism, CMake integration |
| `static-analysis` | clang-tidy, cppcheck, scan-build — triage workflow |
| `build-acceleration` | ccache, sccache, unity builds, PCH, split-DWARF |
| `include-what-you-use` | IWYU with CMake, reports, forward declarations |

### Binary Analysis (4 skills)

| Skill | Purpose |
|-------|---------|
| `elf-inspection` | readelf, objdump, nm, ldd, section analysis |
| `linkers-lto` | GNU ld/gold/lld, -flto, link order, symbol issues |
| `binutils` | ar, strip, objcopy, addr2line workflows |
| `dynamic-linking` | dlopen, RPATH/RUNPATH, soname versioning, LD_PRELOAD |

### Runtime Safety (6 skills)

| Skill | Purpose |
|-------|---------|
| `sanitizers` | ASan/UBSan/TSan/MSan decision trees and report triage |
| `fuzzing` | libFuzzer/AFL, corpus, CI integration |
| `binary-hardening` | checksec, RELRO, PIE, CFI, shadow stack, seccomp-bpf |
| `wasm-emscripten` | emcc flags, EXPORTED_FUNCTIONS, memory model, Asyncify |
| `wasm-wasmtime` | wasmtime CLI, WASI preview2, component model, Rust embedding |
| `formal-verification` | Kani, CBMC, Frama-C WP/EVA: proof harnesses, contracts, unwinding, counterexamples |

### Low-Level Programming (10 skills)

| Skill | Purpose |
|-------|---------|
| `assembly-x86` | x86-64 AT&T/Intel syntax, calling conventions, inline asm |
| `assembly-arm` | AArch64/ARM Thumb, AAPCS, inline asm |
| `assembly-riscv` | RV32/RV64 ISA, psABI, inline asm, QEMU simulation |
| `interpreters` | Bytecode VMs, dispatch loops, JIT fundamentals |
| `simd-intrinsics` | SSE2/AVX2/NEON intrinsics, auto-vectorization reports |
| `memory-model` | C++/Rust memory orderings, acquire-release, lock-free patterns |
| `cpu-cache-opt` | Cache misses, AoS vs SoA, false sharing, prefetching |
| `cpp-coroutines` | co_await/co_yield/co_return, promise_type, frame layout, GDB |
| `linux-kernel-modules` | LKMs, Kbuild, /proc, sysfs, char devices, KGDB |
| `riscv-vector` | RVV 1.0 intrinsics and assembly, vsetvli/LMUL, QEMU VLEN testing, RVA23 |

### Observability (2 skills)

| Skill | Purpose |
|-------|---------|
| `ebpf` | bpftool, libbpf, bpftrace, verifier errors, XDP, CO-RE |
| `sched-ext` | BPF CPU schedulers: CONFIG_SCHED_CLASS_EXT, scx schedulers, DSQs, writing and debugging a scheduler |

### Embedded (2 skills)

| Skill | Purpose |
|-------|---------|
| `openocd-jtag` | OpenOCD config, flash programming, GDB remote, JTAG vs SWD |
| `linker-scripts` | MEMORY/SECTIONS, VMA vs LMA, .bss/.data init, weak symbols |

### Bare-Metal (14 skills)

| Skill | Purpose |
|-------|---------|
| `baremetal-startup` | Reset vector, .data/.bss, stack, crt0, Cortex-M/RISC-V bring-up |
| `mmio-and-bit-manipulation` | volatile MMIO, RMW, alignment, endianness, register masks |
| `interrupts-and-exceptions-baremetal` | NVIC, ISRs, priority, HardFault, latency |
| `peripherals-from-datasheet` | Driver methodology from reference manual register maps |
| `gpio-baremetal` | Pin modes, AF mux, EXTI — STM32, nRF, ESP32 patterns |
| `uart-serial-baremetal` | Polling and IRQ UART, baud, framing, DMA basics |
| `spi-i2c-baremetal` | Master transactions, register read/write protocols |
| `timers-pwm-baremetal` | Timer config, PWM, input capture, output compare |
| `adc-dac-baremetal` | Sampling, calibration, DMA, DAC output |
| `dma-baremetal` | Channel setup, memory/peripheral transfers, IRQ completion |
| `stm32-baremetal` | CMSIS-only STM32 project layout without HAL |
| `datasheet-and-refmanual-reading` | Fast extraction from DS/RM, errata, pin tables |
| `bootloaders-embedded` | VTOR relocation, app validation, OTA/DFU basics |
| `low-power-embedded` | Sleep/stop/standby, clock gating, wake sources |

### Kernel & Driver Development (8 skills)

| Skill | Purpose |
|-------|---------|
| `linux-kernel-architecture` | Subsystems, boot flow, initcalls, source navigation |
| `kernel-memory-management` | Buddy, SLUB, kmalloc, vmalloc, zones, OOM |
| `kernel-concurrency` | Spinlocks, mutex, RCU, seqlock, barriers |
| `device-tree` | DTS syntax, bindings, phandles, overlays |
| `platform-device-model` | platform_driver, probe/remove, sysfs, deferred probe |
| `writing-char-drivers` | file_operations, cdev, copy_to/from_user, ioctl, mmap |
| `bus-drivers-i2c-spi` | i2c_driver, spi_driver, regmap client drivers |
| `kernel-debugging-advanced` | ftrace, trace-cmd, kprobes, kgdb, vmcore |

### Computer Architecture (5 skills)

| Skill | Purpose |
|-------|---------|
| `cpu-pipelines-and-hazards` | Pipeline stages, RAW hazards, forwarding, stalls |
| `memory-hierarchy-and-caches` | L1/L2/L3, coherence, false sharing, prefetch |
| `virtual-memory-paging-and-tlb` | Page tables, faults, TLB pressure, huge pages |
| `abi-and-calling-conventions` | SysV AMD64, AAPCS, RISC-V psABI, stack frames |
| `branch-prediction-and-speculation` | Predictors, mispredict, Spectre/Meltdown awareness |

### Kernel Internals (5 skills)

| Skill | Purpose |
|-------|---------|
| `kernel-internals` | Scheduler, buddy/SLUB, VFS, page cache, OOM killer |
| `device-drivers` | platform/i2c/spi drivers, IRQ, DMA, regmap, udev |
| `kernel-debugging` | kgdb, kdb, ftrace, kprobes, dyndbg, crash dumps |
| `kernel-testing` | KUnit, kselftest, syzkaller, LTP, KernelCI |
| `os-dev-scratch` | Bootloader, long mode, IDT, paging, context switch |

### Allocators (2 skills)

| Skill | Purpose |
|-------|---------|
| `custom-allocators` | Pool/arena allocators, jemalloc/mimalloc tuning, GlobalAlloc |
| `numa-programming` | numactl, libnuma, NUMA-aware structures, lstopo |

### Compiler Internals (6 skills)

| Skill | Purpose |
|-------|---------|
| `compiler-frontend` | Lexer, Pratt parser, AST, type checker, LLVM IR emission |
| `llvm-passes` | New Pass Manager, PassPlugin, llvm-lit, analysis utilities |
| `llvm-ir-and-passes` | Read LLVM IR/SSA, opt pipelines, llvm-dis inspection |
| `compiler-optimizations-deep` | RA, vectorization, PGO, BOLT, LICM depth |
| `code-generation-and-backends` | ISel, TableGen, llc, target lowering overview |
| `jit-compilation` | ORC JIT, LLJIT, Cranelift, inline caches, W^X policy |

### Virtualization (1 skills)

| Skill | Purpose |
|-------|---------|
| `containers-internals` | namespaces, cgroups v2, overlayfs, runc, seccomp |

### Security (1 skills)

| Skill | Purpose |
|-------|---------|
| `memory-safe-c-cpp` | -fhardened, FORTIFY, counted_by, auto-var-init, MTE, hardened allocators, Fil-C, CHERI |

### HPC (3 skills)

| Skill | Purpose |
|-------|---------|
| `openmp` | Parallel for, reductions, SIMD, task parallelism, GPU offload |
| `mpi` | Send/recv, collectives, non-blocking, MPI+OpenMP hybrid |
| `rdma-verbs` | libibverbs, queue pairs, RDMA read/write, RoCE, perftest |

### Platform (2 skills)

| Skill | Purpose |
|-------|---------|
| `arm-sve` | SVE/SVE2 intrinsics, predicates, VLA loops, Graviton tuning |
| `riscv-privileged` | M/S/U modes, CSRs, PLIC/CLINT, OpenSBI, Sv39/Sv48 |

### Languages (2 skills)

| Skill | Purpose |
|-------|---------|
| `carbon-lang` | Carbon syntax, C++ interop, carbon-toolchain, migration |
| `hare-lang` | hare build/test, stdlib, C FFI, tagged union errors |

**Total: 100 skills**

## Design

Each skill follows the [SKILL.md format](https://github.com/anthropics/skills). The body stays under 500 lines; detailed reference material lives in `references/` and is loaded only when needed (progressive disclosure).

Skills cross-reference each other where workflows overlap (e.g., `sanitizers` + `fuzzing`, `gdb` + `core-dumps`, `linux-perf` + `flamegraphs`, `openocd-jtag` + `linker-scripts`).

## Contributing

Contributions are welcome! To add or improve a skill:

1. Fork the repository
2. Create or modify skills in `skills/<category>/<skill-name>/SKILL.md`
3. Follow the SKILL.md format with required sections (Purpose, Triggers, Workflow, Related skills)
4. Add reference files in `references/` for content that exceeds 500 lines
5. Submit a pull request

## Topics

`ai-agent-skills` `low-level-programming` `c-cpp-toolchain` `systems-programming` `compilers` `debuggers` `profilers` `build-systems` `embedded` `bare-metal` `cross-compilation` `ebpf` `webassembly` `risc-v` `linux-kernel` `kernel-drivers` `computer-architecture` `hpc` `mpi` `virtualization`
