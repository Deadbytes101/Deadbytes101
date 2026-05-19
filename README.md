```text
 ______  _______  __   __  _______  _______
|      ||  _    ||  | |  ||       ||       |
|  _    || |_|   ||  |_|  ||_     _||    ___|
| | |   ||       ||       |  |   |  |   |___
| |_|   ||  _   | |_     _|  |   |  |    ___|
|       || |_|   |  |   |    |   |  |   |___
|______||_______|  |___|    |___|  |_______|

GOD IS PERFECTLY JUST / HIGHS AND LOWS BALANCE / I WROTE A COMPILER NIGGER I AM SMARTER THAN LINUS I WROTE A KERNEL AND COMPILER
```

# [DByte](https://dbytelang.site/)

DByte is a statically checked, Python-like scripting language with a bytecode VM and a low-level standard library for binary parsing and buffer patching. It is built for byte work, binary patching, small tools, and personal computing experiments, with an emphasis on direct files, direct output, and fewer layers between the user and the machine. [Source](https://dbytelang.site/docs) [Source](https://dbytelang.site/about)

## [About DEADBYTE](https://dbytelang.site/about)
---

## ☣️ CORE STACK

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
DEADBYTE is the independent builder behind DByte. The project is presented plainly: not a company, not a committee, and not a corporate landing page. The stated direction is handmade software with visible fingerprints rather than polished abstraction for its own sake. [Source](https://dbytelang.site/about)

## [What DByte Does](https://dbytelang.site/)

The public site describes DByte as a fast low-level scripting language for binary parsing, buffer patching, byte search, typed integer workloads, and automation scripts that need simple syntax with predictable performance. The listed standard library areas include filesystem access, encoding, hashing, buffers, binary operations, math, and environment access. [Source](https://dbytelang.site/)

## [DByteOS](https://dbytelang.site/docs)

DByteOS is described as a host-runnable userland built on top of the DByte runtime. It is not presented as a standalone operating system: the docs explicitly say it is not a kernel, bootloader, hardware driver layer, or OS passthrough. Its current direction is a deterministic personal computing environment with shell, preferences, diagnostics, projects, snapshot, and manual-page style documentation. [Source](https://dbytelang.site/docs) [Source](https://dbytelang.site/about)

## Focus

- binary patching
- byte pattern search
- tool scripts
- REPL and shell workflow
- small language design
- system experiments through DByteOS userland
- personal computing workspace concepts [Source](https://dbytelang.site/about) [Source](https://dbytelang.site/)

## Current Public Line

The public download linked on the main site is **DByte 3.3.0** for **windows-x64**, while the docs currently describe the **DByteOS Personal Alpha v5.1.0** line. The docs explicitly note that the v5.1.0 documentation does not mean there is a public v5.1.0 zip available yet. [Source](https://dbytelang.site/) [Source](https://dbytelang.site/docs) [Source](https://dbytelang.site/about)

## Command Surface

The public materials show DByte as a toolchain built around direct command-line usage, including running files, checking files, testing, disassembly, token and AST inspection, REPL access, and shell access. The docs also describe DByteOS-side commands for boot, status, sysinfo, profile, config, prefs, snapshot, doctor, diagnose, and project management. [Source](https://dbytelang.site/) [Source](https://dbytelang.site/docs)

## Example Shape

The official examples show typed variables, functions, byte literals, and buffer-oriented workflows. One published example creates a binary file, finds a byte pattern, replaces it, saves the patched output, and prints the result as hex. [Source](https://dbytelang.site/) [Source](https://dbytelang.site/docs)

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

## Design Notes

The language and site presentation consistently push a direct style: plain HTML, plain CSS, normal links, one download button, and a stated dislike of “cloud altar” or “dashboard smell.” The same tone appears again in the about page, where the project frames itself as direct, inspectable, and deliberately non-corporate. [Source](https://dbytelang.site/) [Source](https://dbytelang.site/about)

## Links

- Site: [dbytelang.site](https://dbytelang.site/)
- Docs: [dbytelang.site/docs](https://dbytelang.site/docs)
- About: [dbytelang.site/about](https://dbytelang.site/about)
- GitHub: [Deadbytes101/DByte](https://github.com/Deadbytes101/DByte)
- Public release: [v3.3.0](https://github.com/Deadbytes101/DByte/releases/tag/v3.3.0)
- Discord community: [discord.gg/hWuwUbrujb](https://discord.gg/hWuwUbrujb) [Source](https://dbytelang.site/about)

```text
Readable code is not soft.
Code that explains itself is a blade with a handle.
```
