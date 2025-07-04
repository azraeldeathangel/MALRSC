# ORASC – Offensive Research And Study Collection
A curated roadmap and resource archive for learning malware development, reverse engineering, and low-level system concepts. Whether you're aiming to analyze malware, develop offensive tooling, or understand the system from the inside out, this collection gives you a solid foundation and learning path.

## [Computer Science Fundamentals](https://www.youtube.com/watch?v=tpIctyqH29Q&list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)
Understand how computers and systems operate at a fundamental level.
* How computers work
* Numeric systems (binary, hex, decimal)
* How memory and CPU work

  * Reference: [pwn.college](https://pwn.college/)
* High-level understanding of machine code

## Low-Level Concepts
Build core knowledge around system internals, cryptography, and debugging.

* Obfuscation, encryption, decryption, and common algorithms
* Learn to use debuggers (e.g., x64dbg)

## Windows Internals
Deep dive into how the Windows OS works under the hood.

* Use [**Windows Internals Part 1**](https://empyreal96.github.io/nt-info-depot/Windows-Internals-PDFs/Windows%20System%20Internals%207e%20Part%201.pdf) as a reference
  * Focus on the first three chapters:
    * Processes
    * Handles
    * Threads

## Learn C (or [C++](https://www.learncpp.com/), I personally prefer C)
Understanding C is essential for anyone serious about malware development, reverse engineering, or low-level systems work. C is close to the metal, giving you control over memory, system calls, and how programs interact with the OS - exactly what you need to build or dissect offensive tools.

> *“I personally prefer C because it maps directly to how machines work. It’s foundational in both malware development and reverse engineering. C helps you understand how exploits happen, how processes are structured, and how the Windows API is used under the hood.”*

You don’t need to buy expensive courses to get started. I learned C using [**Codecademy**](https://www.codecademy.com/learn/paths/c) because of how interactive and beginner-friendly it is. If you want a completely free alternative, [learn-c.org](https://www.learn-c.org/) is a great browser-based site with hands-on examples.

## First project
Try to replicate a malware behavior.
* What is being performed?
* How is it being performed?
* Are there alternative techniques?
* Can we replicate the API usage?

## Malware Resources
Trusted tools, references, and learning hubs in malware

* [Lseqt – YouTube Channel](https://www.youtube.com/@Lsecqt)
* [cr0w – YouTube](https://www.youtube.com/@crr0ww)
* [VX-API](https://github.com/vxunderground/VX-API)
* [VXUG Papers](https://github.com/vxunderground/VXUG-Papers)
* [Filesec](https://filesec.io/)
* [MalAPI](https://malapi.io/)
* [LOTS Project](https://lots-project.com/)
* [EDR Telemetry](https://www.edr-telemetry.com/)
* [Maldev Links by CodeXTF2](https://github.com/CodeXTF2/maldev-links)
* [mr.d0x](https://mrd0x.com/)
* [pre.empt](https://pre.empt.dev/)
* [0xRick](https://0xrick.github.io/misc/c2/)
* [Capt.Meelo](https://captmeelo.com/)

## Reverse Engineering and Pwn Resources
### Foundational Learning
* [OpenSecurityTraining2 – x86_64 Assembly](https://p.ost2.fyi/courses/course-v1:OpenSecurityTraining2+Arch1001_x86-64_Asm+2021_v1/about)
  -> Industry-standard course for understanding assembly, memory models, and the architecture behind reverse engineering.

* [Z0F Reverse Engineering Course](https://www.debugxp.com/posts/RECourse/)
  -> A Windows-focused RE course using tools like x64dbg, PE-bear, and Ghidra. Includes crackmes and walkthroughs.
  
* [Nightmare](https://guyinatuxedo.github.io/00-intro/index.html)
  -> Linux-focused binary exploitation tutorial series focused on memory bugs and control flow.
 
* [pwn.college](https://pwn.college/)
  -> Hands-on platform for learning memory corruption, shellcoding, and RE fundamentals.

### Applied Reverse Engineering
* [wetw0rk](https://wetw0rk.github.io/)
* [dayzerosec Starter Guide](https://dayzerosec.com/blog/2024/07/11/getting-started-2024.html)
* [Wargames by ret2](https://wargames.ret2.systems/)

### Advanced / Kernel Exploitation

* [HackSysExtremeVulnerableDriver](https://github.com/hacksysteam/HackSysExtremeVulnerableDriver)
  -> Learn kernel-mode exploitation using a custom vulnerable Windows driver.

* [OSED Resource Collection](https://github.com/nop-tech/OSED/tree/main)
  -> Materials for OffSec’s Windows Exploit Development certification.

### Hands-On Practice
Challenge-based platforms and exercises to reinforce your skills.

* [crackmes.one](https://crackmes.one/)
* [pwnable.tw](https://pwnable.tw/challenge/)
* [PicoCTF](https://picoctf.org/)
* [Exploit Education](https://exploit.education/)

## Miscellaneous
* [VXLab Book Archive](https://github.com/vxlabinfo/lib/tree/master)

## Contributors
Thanks to the following people:
* [@Lattice23](https://github.com/Lattice23) -> Helped with resources and structure


## Why include Reverse Engineering in a Malware Dev collection?
Reverse engineering is essential if you want to build effective, undetectable malware.

As a developer, you’re not just writing code, you’re trying to understand how defenders will analyze and detect your tools. Reverse engineering gives you insight into how detection works and how to subvert it.

It helps you:
* Recognize what patterns and behaviors AV/EDR solutions flag
* Modify shellcode, payloads, and loaders at the byte level
* Debug and fix your tools when something silently fails in memory
* Understand the entire kill chain from both red and blue perspectives

### Example from the Field:
In one public lab write-up, a researcher successfully evaded a modern EDR by:
* Using **ThreatCheck** and **Ghidra** to identify flagged byte patterns in a payload
* Modifying a **XOR shellcode decryption routine** to alter memory artifacts
* Customizing the C2 profile to strip suspicious strings
* Building a **C++ loader** to bypass sandbox and static detection

These types of evasion techniques rely heavily on reverse engineering skills, knowing how your code looks under the hood, how defenders analyze it, and how to break that process.

