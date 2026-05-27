<div align="center">

# DEADBYTE
[![SITE](https://img.shields.io/badge/DBYTELANG.SITE-0d0d0d?style=for-the-badge&logoColor=red)](https://dbytelang.site/)
[![DOCS](https://img.shields.io/badge/DOCS-0d0d0d?style=for-the-badge&logoColor=red)](https://dbytelang.site/docs)
[![DISCORD](https://img.shields.io/badge/DISCORD-0d0d0d?style=for-the-badge&logo=discord&logoColor=red)](https://discord.gg/hWuwUbrujb)

</div>

## CORE STACK

<p align="left">
  <img src="https://img.shields.io/badge/C-0d0d0d?style=for-the-badge&logo=c&logoColor=red" />
  <img src="https://img.shields.io/badge/Rust-0d0d0d?style=for-the-badge&logo=rust&logoColor=red" />
  <img src="https://img.shields.io/badge/x86__64_ASM-0d0d0d?style=for-the-badge&logo=gnubash&logoColor=red" />
  <img src="https://img.shields.io/badge/Python-0d0d0d?style=for-the-badge&logo=python&logoColor=red" />
  <img src="https://img.shields.io/badge/Linux-0d0d0d?style=for-the-badge&logo=linux&logoColor=red" />
  <img src="https://img.shields.io/badge/Shell-0d0d0d?style=for-the-badge&logo=gnu-bash&logoColor=red" />
  <img src="https://img.shields.io/badge/Kernel_Research-0d0d0d?style=for-the-badge&logo=linux&logoColor=red" />
  <img src="https://img.shields.io/badge/Reverse_Engineering-0d0d0d?style=for-the-badge&logo=hackaday&logoColor=red" />
  <img src="https://img.shields.io/badge/Byte-0d0d0d?style=for-the-badge&logo=dependabot&logoColor=red" />
</p>

---

## [DBYTE](https://dbytelang.site/)

> STATICALLY CHECKED. PYTHON-LIKE. BYTECODE VM. LOW-LEVEL STDLIB.
> BUILT FOR BYTE WORK — NOT FOR YOUR CLOUD ALTAR.

```dbyte
import std.buffer as buf
import std.encoding as enc
import std.fs as fs

fs.write_bytes("sample.bin", b"\x00\xDE\xAD\xBE\xEF\x00")

let b: buffer = buf.load("sample.bin")
let pos: int = buf.find(b, b"\xDE\xAD\xBE\xEF")

if pos >= 0:
    buf.replace(b, pos, b"\x90\x90\x90\x90")
    buf.save("sample.patched.bin", b)

let patched: bytes = fs.read_bytes("sample.patched.bin")
print(enc.hex_encode(patched))
```

**CURRENT PUBLIC RELEASE → [`v3.3.0` windows-x64](https://github.com/Deadbytes101/DByte/releases/tag/v3.3.0)**
**DBYTEOS PERSONAL ALPHA → `v5.1.0` (DOCS ONLY — NO ZIP YET)**

---

## WHAT I BUILD

| DOMAIN | DETAIL |
|---|---|
| `BINARY PATCHING` | FIND. REPLACE. SAVE. NO WRAPPER. |
| `BYTE PATTERN SEARCH` | RAW BUFFER WORK, TYPED INTEGERS |
| `TOOL SCRIPTS` | DIRECT CLI. ONE JOB. DONE. |
| `SMALL LANGUAGE DESIGN` | COMPILER + VM FROM SCRATCH |
| `KERNEL RESEARCH` | LOW LEVEL. NO APOLOGIES. |
| `REVERSE ENGINEERING` | DISASSEMBLE. INSPECT. UNDERSTAND. |
| `REPL / SHELL WORKFLOW` | DBYTEOS USERLAND EXPERIMENTS |

---

## [DBYTEOS](https://dbytelang.site/docs)

A **HOST-RUNNABLE USERLAND** BUILT ON THE DBYTE RUNTIME.

- NOT A KERNEL. NOT A BOOTLOADER. NOT AN OS PASSTHROUGH.
- A **DETERMINISTIC PERSONAL COMPUTING ENVIRONMENT**
- SHELL · PREFERENCES · DIAGNOSTICS · PROJECTS · SNAPSHOT · MANUAL PAGES

---

## LINKS

<div align="left">

| | |
|---|---|
|  **SITE** | [dbytelang.site](https://dbytelang.site/) |
|  **DOCS** | [dbytelang.site/docs](https://dbytelang.site/docs) |
|  **ABOUT** | [dbytelang.site/about](https://dbytelang.site/about) |
|  **GITHUB** | [Deadbytes101/DByte](https://github.com/Deadbytes101/DByte) |
|  **RELEASE** | [v3.3.0](https://github.com/Deadbytes101/DByte/releases/tag/v3.3.0) |
|  **DISCORD** | [discord.gg/hWuwUbrujb](https://discord.gg/hWuwUbrujb) |

</div>
<div align="center">
