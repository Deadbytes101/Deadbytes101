______  _______  __   __  _______  _______
|      ||  _    ||  | |  ||       ||       |
|  _    || |_|   ||  |_|  ||_     _||    ___|
| | |   ||       ||       |  |   |  |   |___
| |_|   ||  _   | |_     _|  |   |  |    ___|
|       || |_|   |  |   |    |   |  |   |___
|______||_______|  |___|    |___|  |_______|

GOD IS PERFECTLY JUST / HIGHS AND LOWS BALANCE / I WROTE A COMPILER NIGGER I AM SMARTER THAN LINUS I WROTE A KERNEL AND COMPILER

# [DBYTE](https://dbytelang.site/)

DBYTE IS A STATICALLY CHECKED, PYTHON-LIKE SCRIPTING LANGUAGE WITH A BYTECODE VM AND A LOW-LEVEL STANDARD LIBRARY FOR BINARY PARSING AND BUFFER PATCHING. IT IS BUILT FOR BYTE WORK, BINARY PATCHING, SMALL TOOLS, AND PERSONAL COMPUTING EXPERIMENTS, WITH AN EMPHASIS ON DIRECT FILES, DIRECT OUTPUT, AND FEWER LAYERS BETWEEN THE USER AND THE MACHINE. [SOURCE](https://dbytelang.site/docs) [SOURCE](https://dbytelang.site/about)

## [ABOUT DEADBYTE](https://dbytelang.site/about)
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
DEADBYTE IS THE INDEPENDENT BUILDER BEHIND DBYTE. THE PROJECT IS PRESENTED PLAINLY: NOT A COMPANY, NOT A COMMITTEE, AND NOT A CORPORATE LANDING PAGE. THE STATED DIRECTION IS HANDMADE SOFTWARE WITH VISIBLE FINGERPRINTS RATHER THAN POLISHED ABSTRACTION FOR ITS OWN SAKE. [SOURCE](https://dbytelang.site/about)

## [WHAT DBYTE DOES](https://dbytelang.site/)

THE PUBLIC SITE DESCRIBES DBYTE AS A FAST LOW-LEVEL SCRIPTING LANGUAGE FOR BINARY PARSING, BUFFER PATCHING, BYTE SEARCH, TYPED INTEGER WORKLOADS, AND AUTOMATION SCRIPTS THAT NEED SIMPLE SYNTAX WITH PREDICTABLE PERFORMANCE. THE LISTED STANDARD LIBRARY AREAS INCLUDE FILESYSTEM ACCESS, ENCODING, HASHING, BUFFERS, BINARY OPERATIONS, MATH, AND ENVIRONMENT ACCESS. [SOURCE](https://dbytelang.site/)

## [DBYTEOS](https://dbytelang.site/docs)

DBYTEOS IS DESCRIBED AS A HOST-RUNNABLE USERLAND BUILT ON TOP OF THE DBYTE RUNTIME. IT IS NOT PRESENTED AS A STANDALONE OPERATING SYSTEM: THE DOCS EXPLICITLY SAY IT IS NOT A KERNEL, BOOTLOADER, HARDWARE DRIVER LAYER, OR OS PASSTHROUGH. ITS CURRENT DIRECTION IS A DETERMINISTIC PERSONAL COMPUTING ENVIRONMENT WITH SHELL, PREFERENCES, DIAGNOSTICS, PROJECTS, SNAPSHOT, AND MANUAL-PAGE STYLE DOCUMENTATION. [SOURCE](https://dbytelang.site/docs) [SOURCE](https://dbytelang.site/about)

## FOCUS

- BINARY PATCHING
- BYTE PATTERN SEARCH
- TOOL SCRIPTS
- REPL AND SHELL WORKFLOW
- SMALL LANGUAGE DESIGN
- SYSTEM EXPERIMENTS THROUGH DBYTEOS USERLAND
- PERSONAL COMPUTING WORKSPACE CONCEPTS [SOURCE](https://dbytelang.site/about) [SOURCE](https://dbytelang.site/)

## CURRENT PUBLIC LINE

THE PUBLIC DOWNLOAD LINKED ON THE MAIN SITE IS **DBYTE 3.3.0** FOR **WINDOWS-X64**, WHILE THE DOCS CURRENTLY DESCRIBE THE **DBYTEOS PERSONAL ALPHA V5.1.0** LINE. THE DOCS EXPLICITLY NOTE THAT THE V5.1.0 DOCUMENTATION DOES NOT MEAN THERE IS A PUBLIC V5.1.0 ZIP AVAILABLE YET. [SOURCE](https://dbytelang.site/) [SOURCE](https://dbytelang.site/docs) [SOURCE](https://dbytelang.site/about)

## COMMAND SURFACE

THE PUBLIC MATERIALS SHOW DBYTE AS A TOOLCHAIN BUILT AROUND DIRECT COMMAND-LINE USAGE, INCLUDING RUNNING FILES, CHECKING FILES, TESTING, DISASSEMBLY, TOKEN AND AST INSPECTION, REPL ACCESS, AND SHELL ACCESS. THE DOCS ALSO DESCRIBE DBYTEOS-SIDE COMMANDS FOR BOOT, STATUS, SYSINFO, PROFILE, CONFIG, PREFS, SNAPSHOT, DOCTOR, DIAGNOSE, AND PROJECT MANAGEMENT. [SOURCE](https://dbytelang.site/) [SOURCE](https://dbytelang.site/docs)

## EXAMPLE SHAPE

THE OFFICIAL EXAMPLES SHOW TYPED VARIABLES, FUNCTIONS, BYTE LITERALS, AND BUFFER-ORIENTED WORKFLOWS. ONE PUBLISHED EXAMPLE CREATES A BINARY FILE, FINDS A BYTE PATTERN, REPLACES IT, SAVES THE PATCHED OUTPUT, AND PRINTS THE RESULT AS HEX. [SOURCE](https://dbytelang.site/) [SOURCE](https://dbytelang.site/docs)

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

## DESIGN NOTES

THE LANGUAGE AND SITE PRESENTATION CONSISTENTLY PUSH A DIRECT STYLE: PLAIN HTML, PLAIN CSS, NORMAL LINKS, ONE DOWNLOAD BUTTON, AND A STATED DISLIKE OF "CLOUD ALTAR" OR "DASHBOARD SMELL." THE SAME TONE APPEARS AGAIN IN THE ABOUT PAGE, WHERE THE PROJECT FRAMES ITSELF AS DIRECT, INSPECTABLE, AND DELIBERATELY NON-CORPORATE. [SOURCE](https://dbytelang.site/) [SOURCE](https://dbytelang.site/about)

## LINKS

- SITE: [DBYTELANG.SITE](https://dbytelang.site/)
- DOCS: [DBYTELANG.SITE/DOCS](https://dbytelang.site/docs)
- ABOUT: [DBYTELANG.SITE/ABOUT](https://dbytelang.site/about)
- GITHUB: [DEADBYTES101/DBYTE](https://github.com/Deadbytes101/DByte)
- PUBLIC RELEASE: [V3.3.0](https://github.com/Deadbytes101/DByte/releases/tag/v3.3.0)
- DISCORD COMMUNITY: [DISCORD.GG/HWUWUBRUJB](https://discord.gg/hWuwUbrujb) [SOURCE](https://dbytelang.site/about)

```text
READABLE CODE IS NOT SOFT.
CODE THAT EXPLAINS ITSELF IS A BLADE WITH A HANDLE.
```
