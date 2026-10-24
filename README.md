<p align="center">i keep coming back to old pcs and machines i can take apart</p>

<p align="center">i write c rust and assembly and build compilers boot code and windows tools<br>some of my boards are still waiting for their first power on</p>

<p align="center"><strong>if i cannot tell what a program is doing i will write a smaller one</strong></p>

<p align="center"><a href="#projects">projects</a> · <a href="#core-stack">core stack</a> · <a href="#bench-notes">bench notes</a> · <a href="#where-the-experience-comes-from">experience</a> · <a href="https://dbytelang.site">dbyte site</a></p>

## projects

every project here has a public repo
some are useful tools and some are still experiments
nothing is polished up to hide what is unfinished

### start here

**[DBYTE](https://github.com/Deadbytes101/DBYTE)** — my programming language with a lexer parser type checker interpreter bytecode compiler vm and native code work
there is a freestanding kernel path too and the public repo is only a snapshot of what has been built

**[BONEBOX-01](https://github.com/Deadbytes101/BONEBOX-01)** — a small x86 real mode system that boots from its own sector and loads a shell from disk
it has a filesystem and executable format with 99 passing host tests and an interactive qemu boot

**[A780L3B BIOS research](https://github.com/Deadbytes101/dbyte-a780l3b-bios-research)** — reading and pulling apart firmware from a BIOSTAR motherboard
rom dumps chip reads with a CH341A disassembly patches hashes and recovery notes
actual bytes from the chip matter more than a patch that only looks right

<details>
<summary>the other 20 projects</summary>

### languages and systems

**[LOOM](https://github.com/Deadbytes101/LOOM)** — an x86-64 os experiment where cells replace one another and the bootstrap gives up control
some stages have machine traces and some are still unresolved
this is not a finished operating system

**[SHINESEA](https://github.com/Deadbytes101/SHINESEA)** — a rust filesystem image core built around contiguous extents mirrored catalogs checksums and recovery rules
tests cover damaged images as well as successful reads
not claiming a finished release from the work in the source tree

**[CINDER-16](https://github.com/Deadbytes101/CINDER-16)** — a 16 bit virtual computer written in io with fixed width instructions cycle counting strict image loading and a debugger that can step backward
i wanted a cpu i could inspect from end to end

**[DBLYATEM](https://github.com/Deadbytes101/DBLYATEM)** — c experiments with pe images amd64 decoding and strict binary checks on linux
low level groundwork rather than a complete windows compatibility layer

**[DBYTE-HOLYC-OPT](https://github.com/Deadbytes101/DBYTE-HOLYC-OPT)** — studying the original HolyC optimizer and trying more transformations around its intermediate code passes
the compiler and native backend are still HolyC and the extra work is experimental

### windows tools and small programs

**[DBYTEPAD](https://github.com/Deadbytes101/DBYTEPAD)** — a native win32 text editor written in c with file handling search replace diffs and optional DByte integration
there are tiny executable experiments too but the smallest builds do not have every editor feature

**[DEADFLASH](https://github.com/Deadbytes101/DEADFLASH)** — a windows disk image writer that makes the target explicit and checks it again before writing
flush readback and verification are part of the job
the repo records seven passing ctest checks for the qualified build

**[DEADBYTE-RECLAIM](https://github.com/Deadbytes101/DEADBYTE-RECLAIM)** — plain win32 software inventory removal and rollback
the graphical interface passes an operation plan to the cli instead of inventing another privileged path

**[DBNET](https://github.com/Deadbytes101/DBNET)** — windows networking diagnostics with throughput probes and controlled configuration changes
package sources are tracked and external measurement tests require consent

**[DEADWIRE-HTTPD](https://github.com/Deadbytes101/DEADWIRE-HTTPD)** — a small http 1 point 0 static server with assembly oriented backends
more attention goes to request bytes bad paths and measured hot paths than feature count

**[BYTE-KEEPER](https://github.com/Deadbytes101/BYTE-KEEPER)** — m0te is a little digital creature running in a native rust program
it has persistent state a room and a taskbar companion
weird idea but there is working code and there are tests

### graphics and pixels

**[DEADGL](https://github.com/Deadbytes101/DEADGL)** — a c99 software renderer that takes text commands and produces framebuffer pixels ppm output and deterministic hashes
i want to see what happens between the command and the pixel

**[DGP-1](https://github.com/Deadbytes101/DGP-1)** — old style fixed function graphics hardware research with a command fifo triangle coverage texture units scanout memory arbitration rtl and software reference models
no finished physical graphics card

**[dbyte-dbpx](https://github.com/Deadbytes101/dbyte-dbpx)** — a small lossless raster image format with explicit chunks and pixel formats
built so the decoder can be read without dragging in a massive image library

### boards and old pcs

**[DBYTE-370](https://github.com/Deadbytes101/DBYTE-370)** — a socket 370 atx motherboard design for a pentium iii and via chipsets
cpu and chipset pins sdram agp power clocks and reset are the work here
not claiming a board has been powered on

**[S3CORE01](https://github.com/Deadbytes101/S3CORE01)** — a small rv64 computer design around the sg2002
one four layer cad revision has zero drc violations and zero unconnected items
that does not mean a physical board or linux boot has been proven

**[USBDEADFLASH](https://github.com/Deadbytes101/USBDEADFLASH)** — a usb flash drive designed from the connector inward
controller nand controlled impedance power and kicad layout
still a design and not a manufactured drive

### other work

**[RIGOS](https://github.com/Deadbytes101/RIGOS)** — an old usb bootable cpu mining appliance experiment kept here for the record
i stopped working on this one and do not maintain it anymore

**[JOBSIM-DESKTOP](https://github.com/Deadbytes101/JOBSIM-DESKTOP)** — keyboard and mouse compatibility work for job simulator
archived as an engineering alpha rather than passed off as a finished release

**[Shower Game remaster study](https://github.com/Deadbytes101/shower-game-remastered-2015)** — source provenance and clean room planning for an old game
research only and not a playable remake or a copy of someone else's files

</details>

## core stack

<details>
<summary>languages systems tools and hardware </summary>

i do not use all of this every day
this is the stuff i have actually worked with

**languages**

![C17](https://img.shields.io/badge/C17-20252B?style=flat-square&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C%2B%2B-20252B?style=flat-square&logo=cplusplus&logoColor=white) ![C#](https://img.shields.io/badge/C%23-20252B?style=flat-square&logo=csharp&logoColor=white) ![Rust](https://img.shields.io/badge/Rust-20252B?style=flat-square&logo=rust&logoColor=white) ![x86 Assembly](assets/core-badges/x86-assembly.svg) ![DByte](assets/core-badges/dbyte.svg) ![HolyC](assets/core-badges/holyc.svg) ![Io](assets/core-badges/io.svg) ![Verilog](assets/core-badges/verilog.svg) ![Python](https://img.shields.io/badge/Python-20252B?style=flat-square&logo=python&logoColor=white) ![PowerShell](https://img.shields.io/badge/PowerShell-20252B?style=flat-square&logo=powershell&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-20252B?style=flat-square&logo=gnubash&logoColor=white)

**systems**

![Win32](assets/core-badges/win32.svg) ![Linux](https://img.shields.io/badge/Linux-20252B?style=flat-square&logo=linux&logoColor=white) ![WSL](assets/core-badges/wsl.svg) ![x86](assets/core-badges/x86.svg) ![x86-64](assets/core-badges/x86-64.svg) ![BIOS](assets/core-badges/bios.svg) ![Legacy BIOS](assets/core-badges/legacy-bios.svg) ![UEFI](assets/core-badges/uefi.svg) ![RISC-V](https://img.shields.io/badge/RISC--V-20252B?style=flat-square&logo=riscv&logoColor=white) ![QEMU](https://img.shields.io/badge/QEMU-20252B?style=flat-square&logo=qemu&logoColor=white)

**build and debugging**

![Git](https://img.shields.io/badge/Git-20252B?style=flat-square&logo=git&logoColor=white) ![CMake](https://img.shields.io/badge/CMake-20252B?style=flat-square&logo=cmake&logoColor=white) ![GCC](https://img.shields.io/badge/GCC-20252B?style=flat-square&logo=gnu&logoColor=white) ![Clang](https://img.shields.io/badge/Clang-20252B?style=flat-square&logo=llvm&logoColor=white) ![MSVC](assets/core-badges/msvc.svg) ![Cargo](https://img.shields.io/badge/Cargo-20252B?style=flat-square&logo=rust&logoColor=white)

**hardware**

![KiCad](https://img.shields.io/badge/KiCad-20252B?style=flat-square&logo=kicad&logoColor=white) ![CH341A](assets/core-badges/ch341a.svg) ![PCB Design](assets/core-badges/pcb-design.svg) ![FPGA](assets/core-badges/fpga.svg) ![USB 2.0](assets/core-badges/usb-2.svg) ![USB 3.0](assets/core-badges/usb-3.svg) ![USB 3.2 Gen 1](assets/core-badges/usb-3-2-gen1.svg) ![RP2040](https://img.shields.io/badge/RP2040-20252B?style=flat-square&logo=raspberrypi&logoColor=white) ![BIOSTAR](assets/core-badges/biostar.svg)

</details>

## where the experience comes from

<details>
<summary>windows linux bios firmware software and hardware</summary>

most of this started with breaking things on my own machines and figuring out why
bios setup and recovery rom reads with a CH341A memory and storage trouble windows internals linux builds and boot failures

on the software side i have worked with parsers linkers executable formats win32 controls disk access sockets bytecode virtual machines x86 boot stages interrupts fixed point graphics and native tests
i use debuggers disassemblers qemu compiler warnings regression tests and raw binary comparisons
checking the bytes is the part that never changes

on the hardware side i use kicad for schematics footprints buses layer stacks power nets and drc
i check pin maps against documentation and work on old chipsets firmware small stepper motors and salvaged hardware
cad and simulation are not proof that a real board works

i also make game mods and investigate runtimes including my summer car
reading someone else's code keeping the original behavior intact and tracing a value back to its actual source are all part of that work

this is independent engineering and personal research
no made up employers no invented job titles and no pretending a prototype has shipped

</details>

## bench notes

<details>
<summary>what counts as proof</summary>

```text
source     identify the exact revision
build      record what compiled
run        keep the output and failures
compare    check bytes and hashes and behavior
hardware   measure the real thing before claiming it works
```

a passing unit test does not prove a pcb works
a benchmark with different conditions proves nothing
a screenshot is not the program that made it

</details>

<details>
<summary>courses and certificates</summary>

| coursework | issuer | record |
| --- | --- | --- |
| [MIPS Computer Architecture and Performance Optimization](https://www.coursera.org/verify/2DSRTVQR57DL) | BITS Pilani and Coursera | course certificate |
| [Google IT Support](https://www.coursera.org/verify/professional-cert/KVMFVDKBTTDL) | Google and Coursera | professional certificate |
| [IBM IT Support](https://www.coursera.org/verify/professional-cert/GNPDQ9N8IBFD) | IBM and Coursera | professional certificate |
| [CompTIA A+ Core 1 coursework](https://www.coursera.org/verify/specialization/MKCQF06B5GH6) | Total Seminars and Coursera | coursework specialization not CompTIA certification |
| [Computer and ICT Literacy Skills, 45 Hours](https://learner.thaimooc.ac.th/credential-wallet/a98d5c90-68cb-47b2-897e-0ce9aa35da1a/poongsak.phu/public) | Khon Kaen University and Thai MOOC | certificate of completion |

</details>

## github numbers

i do not take these numbers seriously
open the code if you want to know what works

<a href="https://github.com/Deadbytes101">
  <img src="https://github-readme-stats.shion.dev/api?username=Deadbytes101&show_icons=true&theme=github_dark&hide_border=true&hide_title=true" height="160" alt="GitHub activity">
</a>
<a href="https://github.com/Deadbytes101?tab=repositories">
  <img src="https://github-readme-stats.shion.dev/api/top-langs/?username=Deadbytes101&layout=compact&theme=github_dark&hide_border=true&langs_count=6" height="160" alt="Languages used in public GitHub repositories">
</a>

---

the rest is in the [public repositories](https://github.com/Deadbytes101?tab=repositories)
the code and the failures are there too
