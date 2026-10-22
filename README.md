# WHO IS DEADBYTE?

I like computers I can take apart. Old PCs, boot sectors, ROM dumps, weird bugs. That's the stuff I keep coming back to.

C, Rust and assembly are what I reach for most. I've written compilers, tiny operating systems and Windows tools. I've also drawn boards that still need their first power-on. Sometimes I build something to learn how it works. Sometimes the existing tool just gets on my nerves.

**If I can't figure out what a program is doing, I'll probably write a smaller one.**

## Core stack

I don't use all of this every day. These are the things I've actually worked with.

**Languages**

![C17](https://img.shields.io/badge/C17-24303C?style=flat-square&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C%2B%2B-24303C?style=flat-square&logo=cplusplus&logoColor=white) ![C#](https://img.shields.io/badge/C%23-24303C?style=flat-square&logo=csharp&logoColor=white) ![Rust](https://img.shields.io/badge/Rust-24303C?style=flat-square&logo=rust&logoColor=white) ![x86 Assembly](https://img.shields.io/badge/x86%20Assembly-24303C?style=flat-square) ![DByte](https://img.shields.io/badge/DByte-24303C?style=flat-square) ![HolyC](https://img.shields.io/badge/HolyC-24303C?style=flat-square) ![Io](https://img.shields.io/badge/Io-24303C?style=flat-square) ![Verilog](https://img.shields.io/badge/Verilog-24303C?style=flat-square) ![Python](https://img.shields.io/badge/Python-24303C?style=flat-square&logo=python&logoColor=white) ![PowerShell](https://img.shields.io/badge/PowerShell-24303C?style=flat-square&logo=powershell&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-24303C?style=flat-square&logo=gnubash&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-24303C?style=flat-square&logo=javascript&logoColor=white)

**Systems**

![Win32](https://img.shields.io/badge/Win32-263A49?style=flat-square) ![Linux](https://img.shields.io/badge/Linux-263A49?style=flat-square&logo=linux&logoColor=white) ![WSL](https://img.shields.io/badge/WSL-263A49?style=flat-square) ![x86](https://img.shields.io/badge/x86-263A49?style=flat-square) ![x86-64](https://img.shields.io/badge/x86--64-263A49?style=flat-square) ![BIOS](https://img.shields.io/badge/BIOS-263A49?style=flat-square) ![UEFI](https://img.shields.io/badge/UEFI-263A49?style=flat-square) ![RISC-V](https://img.shields.io/badge/RISC--V-263A49?style=flat-square) ![QEMU](https://img.shields.io/badge/QEMU-263A49?style=flat-square&logo=qemu&logoColor=white)

**Build and debugging**

![Git](https://img.shields.io/badge/Git-38352E?style=flat-square&logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-38352E?style=flat-square&logo=githubactions&logoColor=white) ![CMake](https://img.shields.io/badge/CMake-38352E?style=flat-square&logo=cmake&logoColor=white) ![GCC](https://img.shields.io/badge/GCC-38352E?style=flat-square&logo=gnu&logoColor=white) ![Clang](https://img.shields.io/badge/Clang-38352E?style=flat-square&logo=llvm&logoColor=white) ![MSVC](https://img.shields.io/badge/MSVC-38352E?style=flat-square) ![Cargo](https://img.shields.io/badge/Cargo-38352E?style=flat-square&logo=rust&logoColor=white)

**Hardware**

![KiCad](https://img.shields.io/badge/KiCad-41322E?style=flat-square&logo=kicad&logoColor=white) ![CH341A](https://img.shields.io/badge/CH341A-41322E?style=flat-square) ![PCB Design](https://img.shields.io/badge/PCB%20Design-41322E?style=flat-square) ![FPGA](https://img.shields.io/badge/FPGA-41322E?style=flat-square) ![USB 3.0](https://img.shields.io/badge/USB%203.0-41322E?style=flat-square&logo=usb&logoColor=white) ![RP2040](https://img.shields.io/badge/RP2040-41322E?style=flat-square&logo=raspberrypi&logoColor=white)

[Projects](#projects) · [Bench notes](#bench-notes) · [Experience](#where-the-experience-comes-from) · [DByte website](https://dbytelang.site)

## Projects

Everything here has a public repository. Some projects are released tools, others are experiments with unfinished edges. I've left those edges visible.

### Languages, operating systems and executable formats

**[DBYTE](https://github.com/Deadbytes101/DBYTE)** — My programming language. Lexer, parser, type checker, interpreter, bytecode compiler, VM and native code experiments. There is also a freestanding kernel path and a separate kernel lab. The public repository is a working snapshot; it doesn't pretend to contain every later experiment.

**[BONEBOX-01](https://github.com/Deadbytes101/BONEBOX-01)** — A small x86 real-mode system starting at the boot sector, with a resident nucleus, disk-loaded shell, filesystem and executable format. The repository records 99 passing host tests and an interactive QEMU boot.

**[LOOM](https://github.com/Deadbytes101/LOOM)** — Trying a different OS structure on x86-64. Cells replace one another and the bootstrap gives up ownership. Some stages have machine traces; others are still open problems. It isn't a finished general-purpose OS.

**[SHINESEA](https://github.com/Deadbytes101/SHINESEA)** — A Rust filesystem image core with contiguous extents, mirrored catalogs, checksums and recovery rules. The tests cover failure cases as well as successful reads. Version 1.0 is not claimed as released.

**[CINDER-16](https://github.com/Deadbytes101/CINDER-16)** — A 16-bit virtual computer written in Io. Fixed-width instructions, deterministic cycle counting, strict image loading and a debugger that can step backward. Mostly built because writing a CPU you can inspect is fun.

**[DBLYATEM](https://github.com/Deadbytes101/DBLYATEM)** — C experiments with PE images, AMD64 decoding and strict binary verification on Linux. This is low-level groundwork, not a complete Windows compatibility environment.

**[DBYTE-HOLYC-OPT](https://github.com/Deadbytes101/DBYTE-HOLYC-OPT)** — Studying Terry's HolyC optimizer and experimenting with additional transformations around its original intermediate-code passes. The compiler and native backend remain HolyC. Early research, not a replacement compiler.

### Windows tools, networking and small programs

**[DBYTEPAD](https://github.com/Deadbytes101/DBYTEPAD)** — A native Win32 text editor written in C. File operations, find and replace, diffs and optional DByte integration. The size experiments include deliberately tiny executables with different capabilities; the smallest one is not advertised as a full editor.

**[DEADFLASH](https://github.com/Deadbytes101/DEADFLASH)** — A Windows disk-image writer and verifier. It makes the destructive target explicit, checks it again before writing, flushes, reads back and records evidence. The repository documents seven passing CTest checks for its qualified build.

**[DEADBYTE-RECLAIM](https://github.com/Deadbytes101/DEADBYTE-RECLAIM)** — Plain Win32 software inventory, uninstall and rollback. The graphical interface isn't a second privileged implementation; it passes an operation plan to the CLI and checks what comes back.

**[DBNET](https://github.com/Deadbytes101/DBNET)** — Windows network measurements and diagnosis, including throughput probes and controlled network changes. It keeps package provenance and requires consent before tests that disclose data to an external measurement service.

**[DEADWIRE-HTTPD](https://github.com/Deadbytes101/DEADWIRE-HTTPD)** — A deliberately small HTTP/1.0 static server with assembly-oriented backends. I spend more time on bad paths, request bytes and measured hot paths than on features a small server doesn't need.

**[BYTE-KEEPER](https://github.com/Deadbytes101/BYTE-KEEPER)** — M0TE, a tiny digital creature living in a native Rust program. A persistent habitat, a small simulated room and a taskbar companion. A strange one, but it's a real program with state and tests.

### Pixels and graphics hardware

**[DEADGL](https://github.com/Deadbytes101/DEADGL)** — A C99 software renderer. Text commands go in; framebuffer pixels, PPM output and deterministic hashes come out. The interesting part is seeing every step between the command and the pixel.

**[DGP-1](https://github.com/Deadbytes101/DGP-1)** — Fixed-function graphics processor research inspired by older GPU designs. Command FIFO, triangle coverage, texture units, scanout, memory arbitration, RTL and software reference models. There is no finished physical graphics card.

**[dbyte-dbpx](https://github.com/Deadbytes101/dbyte-dbpx)** — My own small lossless raster-image format. Simple chunks, explicit pixel formats and a decoder you can audit without needing a giant image library.

### Boards, firmware and old PCs

**[DBYTE-370](https://github.com/Deadbytes101/DBYTE-370)** — A Socket 370 ATX motherboard design for a Pentium III and VIA chipsets. CPU and chipset pin contracts, SDRAM, AGP, power delivery, clocks and reset are the actual work. It is still a design, not a board I've powered on.

**[S3CORE01](https://github.com/Deadbytes101/S3CORE01)** — A small RV64 computer built around the SG2002. The routed four-layer CAD revision records zero DRC violations and zero unconnected items. That is a PCB check, not evidence of a manufactured board or a successful Linux boot.

**[USBDEADFLASH](https://github.com/Deadbytes101/USBDEADFLASH)** — Designing a USB 3.0 flash drive from the electrical side. Connector, controller, NAND, controlled impedance, power and KiCad layout. Still engineering work, not a shipping flash drive.

**[A780L3B BIOS research](https://github.com/Deadbytes101/dbyte-a780l3b-bios-research)** — ROM dumps, disassembly, patched firmware, hashes and recovery notes for a BIOSTAR motherboard. This is where the CH341A programmer and real chip reads matter more than a plausible-looking hex edit.

### Other work

**[RIGOS](https://github.com/Deadbytes101/RIGOS)** — A local-first USB-bootable CPU mining appliance under development, with its own hardware and software acceptance work.

**[JOBSIM-DESKTOP](https://github.com/Deadbytes101/JOBSIM-DESKTOP)** — Native keyboard and mouse compatibility work for Job Simulator. Kept as an archived engineering alpha, not presented as a finished release.

**[Shower Game remaster study](https://github.com/Deadbytes101/shower-game-remastered-2015)** — Source provenance and clean-room planning around a 2015 game. It's a research repository, not a playable remake or a mirror of someone else's game files.

## Where the experience comes from

I learned a lot of this by breaking things on my own machines and then trying to understand exactly what broke. That includes BIOS setup and recovery, ROM reading with a CH341A, memory and storage problems, Windows internals, Linux builds, odd boot failures and hardware that refuses to behave like its manual.

On the software side I've worked through parsers, linkers and executable formats, Win32 messages and controls, disk access, sockets, bytecode VMs, x86 boot stages, interrupt handling, fixed-point graphics and native testing. I use debuggers, disassemblers, QEMU, compiler warnings, regression tests and raw binary comparisons. The tools change; the habit of checking the bytes doesn't.

On the hardware side I've used KiCad to work through schematics, footprints, buses, layer stacks, power nets and DRC. I've checked pin maps against component documentation, studied old chipsets and firmware, and experimented with small stepper motors and salvaged hardware. CAD work and simulation are useful, but I don't call them a working physical board.

I also work on game mods and runtime investigations, including My Summer Car. Those projects have taught me plenty about debugging code that I didn't originally write, keeping game behavior intact and finding out whether the value shown by a UI comes from a real source.

This is independent engineering and personal research. I'm not inventing a previous employer, a job title or a shipped product to make the page look better.

## Bench notes

<details>
<summary>What I count as proof</summary>

```text
SOURCE     identify the exact revision
BUILD      record what compiled
RUN        keep the output and failures
COMPARE    check bytes, hashes and behavior
HARDWARE   measure the real thing before claiming it works
```

A passing unit test doesn't prove a PCB works. A benchmark without matching conditions doesn't prove one program is faster. A screenshot isn't a substitute for the program that produced it.

</details>

## GitHub numbers

I don't take these too seriously. If you want to know what actually works, open the code.

<a href="https://github.com/Deadbytes101">
  <img src="https://github-readme-stats.shion.dev/api?username=Deadbytes101&show_icons=true&theme=github_dark&hide_border=true&hide_title=true" height="160" alt="GitHub activity">
</a>
<a href="https://github.com/Deadbytes101?tab=repositories">
  <img src="https://github-readme-stats.shion.dev/api/top-langs/?username=Deadbytes101&layout=compact&theme=github_dark&hide_border=true&langs_count=6" height="160" alt="Languages used in public GitHub repositories">
</a>

<details>
<summary>Courses and certificates</summary>

| Coursework | Issuer | Record |
| --- | --- | --- |
| [MIPS Computer Architecture and Performance Optimization](https://www.coursera.org/verify/2DSRTVQR57DL) | BITS Pilani and Coursera | Course certificate |
| [Google IT Support](https://www.coursera.org/verify/professional-cert/KVMFVDKBTTDL) | Google and Coursera | Professional certificate |
| [IBM IT Support](https://www.coursera.org/verify/professional-cert/GNPDQ9N8IBFD) | IBM and Coursera | Professional certificate |
| [CompTIA A+ Core 1 coursework](https://www.coursera.org/verify/specialization/MKCQF06B5GH6) | Total Seminars and Coursera | Coursework specialization, not CompTIA certification |
| [Computer and ICT Literacy Skills, 45 Hours](https://learner.thaimooc.ac.th/credential-wallet/a98d5c90-68cb-47b2-897e-0ce9aa35da1a/poongsak.phu/public) | Khon Kaen University and Thai MOOC | Certificate of completion |

</details>

---

You can find the rest of the history in the [public repositories](https://github.com/Deadbytes101?tab=repositories). The code and the failures say more than a profile ever will.
