Research & Development: Fun and Learning​​​​​​​​​​​​​​​​

- [Venom (2021-2022)](https://github.com/memN0ps/venom-rs) - Shellcode Reflective DLL Injection (sRDI): converts a DLL into position-independent shellcode using a prepended reflective loader that can be injected and executed using any shellcode injection technique

- [Eagle (2021-2022)](https://github.com/memN0ps/eagle-rs) - Windows Kernel Rootkit: process, thread, and registry hiding via DKOM, token privilege elevation to SYSTEM, kernel callback enumeration, and Driver Signature Enforcement bypass

- [RedLotus (2022-2023)](https://github.com/memN0ps/redlotus-rs) - Windows UEFI Bootkit: executes before the kernel loads, hooks the boot manager to manually map an unsigned driver and bypass DSE at the firmware level

- [Matrix (2023-2024)](https://github.com/memN0ps/matrix-rs) - Windows Kernel Type-2 Hypervisor: virtualizes the running OS from a kernel driver using dual-EPT context switching, PatchGuard-compatible hidden inline hooks, hidden SSDT syscall hooks, and stealthy execution redirection via trampoline without modifying guest memory

- [Illusion (2024-2025)](https://github.com/memN0ps/illusion-rs) - Windows UEFI Type-1 Hypervisor: boots before the OS using Intel VT-x and EPT, intercepts kernel initialization at boot to install execute-only shadow pages, replays displaced instructions via Monitor Trap Flag single-stepping, and exposes a user-mode hypercall channel to toggle kernel hooks at runtime, all without touching guest memory or triggering PatchGuard

- [Armory (2026)](https://github.com/memN0ps/armory-rs) - 115 TrustedSec BOFs ported from C to Rust: in-process situational awareness, remote operations, and injection tradecraft that execute inside the Beacon process, avoiding fork-and-run

- [DoublePulsar (2026)](https://github.com/memN0ps/doublepulsar-rs) - Cobalt Strike UDRL: a ~65KB position-independent reflective loader with module stomping, synthetic call stack spoofing, sleep obfuscation, memory encryption, return address spoofing, IAT hooking, and heap isolation

- Private Hyper-V Hyperjacking Framework (2023-2025) - A fully custom framework written entirely in Rust that injects into Microsoft Hyper-V at boot via a UEFI bootkit, hooks the VMEXIT handler to intercept and control guest execution, and performs arbitrary guest physical memory read/write from below the OS using EPT-backed page table manipulation, invisible to anything running in the guest

- Private C2 Framework (2022-2026) - A fully custom Command and Control framework written entirely in Rust. The public research above represents the building blocks.

The language doesn't matter. The primitives are the same. Rust just happens to be the one I enjoy.

Research and writeups: [secret.club](https://secret.club/author/memn0ps) | [memn0ps.github.io](https://memn0ps.github.io)
