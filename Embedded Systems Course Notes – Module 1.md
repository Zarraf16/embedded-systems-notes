# 📘 Embedded Systems Course Notes – Module 1

## 🧩 1. What is an Embedded System?
- A computerized system purpose-built for a specific application.
- Always includes a **processing core** (e.g., microcontroller).
- Operates under **resource constraints**: limited memory, CPU, and peripherals.

## ⚙️ 2. Hardware & Software Roles
- Hardware = processor + external circuits (sensors, power, I/O).
- Software installer loads software image into the processor’s memory.
- PCBs interconnect components including the processor and power converters.
- An **external programmer** is used to flash the software into memory.

## 💻 3. Host vs Target
- **Host Machine**: where development happens (source code lives).
- **Target System**: the actual embedded hardware where code runs.

## 🧠 4. Microcontroller vs Microprocessor
- **Microcontroller** = microprocessor + memory + I/O in one chip.
- CPU executes instructions, performs logic, math, and data transfer.
- CPU Includes: Registers, ALU, interrupt controller, debug interface, clock system, power management.
- Registers store system state.
- ALU handles arithmetic/logical ops.
- **Interrupt Controller** manages asynchronous events.
- Debug Interface allows real-time program troubleshooting.
- Clock system synchronizes all components.
- Power management hardware handles regulation.

## 🎛 5. Peripheral Hardware
- Includes communication (UART, I2C, SPI), analog processing (ADC), I/O, timers, and system support.

## 🧬 6. Firmware and HAL
- **Bare-metal firmware**: code written directly to interface with hardware.
- **HAL (Hardware Abstraction Layer)**: isolates higher software from hardware; makes code portable and modular.

## 🧩 7. Component Design
- Software is broken into **reusable modules** with clearly defined specs.
- Promotes cross-platform compatibility and team collaboration.

## 🔍 8. On-Target Testing
- Running the compiled code on actual embedded hardware, not simulators.

## 🛠 9. Development Tools
1. **Simulators**: imitate hardware behavior without real devices.
2. **Emulators**: mimic target hardware on a development platform.
3. **Compilers**: convert source code to target machine code.
4. **Installers**: flash the compiled code into the target hardware.
5. **Debuggers**: test and step through code on actual or simulated hardware.

## ✅ 10. Code Quality Goals
- Code should be maintainable, testable, portable, robust, efficient, and consistent.

## 🧾 11. Embedded C vs Standard C
- Focuses on:
  - Efficient memory use
  - Timing-sensitive operations
  - Low-level I/O control
  - Small code size
  - Fast execution

## 📚 12. SCM – Software Configuration Management
- Manages the software project: version control, build/release process, testing, issue tracking, etc.
- **Version Control** is critical — tracks all project changes indefinitely.

## 🧱 13. Legacy Systems
- Older products may still need support for reference, reuse, or validation.
- Legacy hardware/software may be outdated but still valuable.

## 🐞 14. Common Bug Sources
- Race conditions
- Timing issues
- Misconfigured hardware/software
- Logic errors
- Typos

## 🖥 15. Development Environment
- Tools: Linux command line + Vendor IDE.
- Command line = more control but steeper learning curve.
- Commands prefixed with `$` indicate CLI instructions.
- Portable code can be tested on the host machine.

## 🐛 16. Debugging
- **GDB** (GNU Debugger) used for host debugging.
- On-target debugging uses network or hardware-based tools.

---

# 🧾 Version Control System (VCS)

## 🔄 17. Overview
- Tracks changes to source code, build files, and configuration.
- Collection of files + history = **repository** or **repo**.

## 🧠 18. Commits
- Each change = a **commit** with:
  - Author + email
  - Date
  - Change list
  - Message
  - SHA-1 hash

## 🌐 19. Remote Tracking
- Map another developer’s repo as a **remote**.
- Use `clone` to copy a remote repo to your local machine.

## 🌳 20. Branches
- **Branch**: safe way to experiment without affecting main codebase.
- Allows multiple feature tracks (feature branches, bug fix branches).
- Workflow:
  - Make changes → **stage** → **commit**.

## 🔍 21. Compare & Merge
- `git diff` shows changes between commits.
- `git merge` or `git rebase` combines branches.
- Metadata links features, bug fixes, and code versions.

## 🤝 22. Team Collaboration
- VCS encourages collaboration by syncing changes across team members.
- Everyone works on the latest version of code and shares updates via pushes and pulls.

---
