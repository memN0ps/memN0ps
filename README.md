**GitHub is my sole online presence. I do not maintain any social media accounts; any other profiles claiming to be me are impersonations.**

Research & Development: Practical proof-of-concept research built for security awareness, detection engineering, and the love of Rust, Windows internals, and reverse engineering.

- [Venom (2021-2022)](https://github.com/memN0ps/venom-rs) - Shellcode Reflective DLL Injection (sRDI): converts a DLL into position-independent shellcode using a prepended reflective loader that can be injected and executed using any shellcode injection technique

- [Eagle (2021-2022)](https://github.com/memN0ps/eagle-rs) - Windows Kernel Rootkit: process, thread, and registry hiding via DKOM, token privilege elevation to SYSTEM, kernel callback enumeration, and Driver Signature Enforcement bypass

- [RedLotus (2022-2023)](https://github.com/memN0ps/redlotus-rs) - Windows UEFI Bootkit: executes before the kernel loads, hooks the boot manager to manually map an unsigned driver and bypass DSE at the firmware level

- [Matrix (2023-2024)](https://github.com/memN0ps/matrix-rs) - Windows Kernel Type-2 Hypervisor: virtualizes the running OS from a kernel driver using dual-EPT context switching, PatchGuard-compatible hidden inline hooks, hidden SSDT syscall hooks, and stealthy execution redirection via trampoline without modifying guest memory

- [Illusion (2024-2025)](https://github.com/memN0ps/illusion-rs) - Windows UEFI Type-1 Hypervisor: boots before the OS using Intel VT-x and EPT, intercepts kernel initialization at boot to install execute-only shadow pages, replays displaced instructions via Monitor Trap Flag single-stepping, and exposes a user-mode hypercall channel to toggle kernel hooks at runtime, all without touching guest memory or triggering PatchGuard

- [Armory (2026)](https://github.com/memN0ps/armory-rs) - A collection of Rust Beacon Object Files (BOFs) for Cobalt Strike. It covers situational awareness, local and remote operations, Active Directory and Microsoft Entra ID (Azure AD), Kerberos and LDAP tradecraft, process injection, and post-exploitation. It also includes a Bring Your Own Vulnerable Driver (BYOVD) BOF for removing kernel callbacks, disabling ETW Threat Intelligence, bypassing PPL, enabling WDigest credential caching, swapping process tokens, running a DSE disable-and-restore cycle, and dumping credentials that remain in VTL0 LSASS without `OpenProcess`, even when Credential Guard is enabled. Secrets isolated in VTL1 remain protected.
  
- [DoublePulsar (2026)](https://github.com/memN0ps/doublepulsar-rs) - Cobalt Strike UDRL: a ~65KB position-independent reflective loader with module stomping, synthetic call stack spoofing, sleep obfuscation, memory encryption, return address spoofing, IAT hooking, and heap isolation

- Private Hyper-V Hyperjacking Framework (2023-2025) - A fully custom framework written entirely in Rust that injects into Microsoft Hyper-V at boot via a UEFI bootkit, hooks the VMEXIT handler to intercept and control guest execution, and performs arbitrary guest physical memory read/write from below the OS using EPT-backed page table manipulation, invisible to anything running in the guest

- Private C2 Framework (2022-2026) - A fully custom Command and Control framework written entirely in Rust. The public research above represents the building blocks.

- Private RISC-V VM Obfuscation Framework (2026) - A general-purpose RISC-V bytecode interpreter written in Rust for VM-based code obfuscation and reverse engineering research, with per-build encryption, opcode shuffling, steganography, Mixed Boolean Arithmetic (MBA), opaque
  predicates, and Control Flow Flattening (CFF).

The language doesn't matter. The primitives are the same. Rust just happens to be the one I enjoy.

Research and writeups: [secret.club](https://secret.club/author/memn0ps) | [memn0ps.github.io](https://memn0ps.github.io)
