# MRASC – Malware Research and Study Collection
A curated roadmap and resource archive for learning malware development, reverse engineering, and low-level system concepts. Whether you're aiming to analyze malware, develop offensive tooling, or understand the system from the inside out, this collection gives you a solid foundation and learning path.

## Computer Science Fundamentals
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

* Use **Windows Internals Part 1** as a reference
  * Focus on the first three chapters:
    * Processes
    * Handles
    * Threads

## First project
Try to replicate a malware behavior.
* What is being performed?
* How is it being performed?
* Are there alternative techniques?
* Can we replicate the API usage?

## Reverse Engineering and Pwn
### Foundational Learning
* [OpenSecurityTraining2 – x86_64 Assembly](https://p.ost2.fyi/courses/course-v1:OpenSecurityTraining2+Arch1001_x86-64_Asm+2021_v1/about)
  -> Industry-standard course for understanding assembly, memory models, and the architecture behind reverse engineering.
 
* [pwn.college](https://pwn.college/)
  -> Hands-on platform for learning memory corruption, shellcoding, and RE fundamentals.

* [Z0F Reverse Engineering Course](https://www.debugxp.com/posts/RECourse/)
  -> A Windows-focused RE course using tools like x64dbg, PE-bear, and Ghidra. Includes crackmes and walkthroughs.

* [Nightmare](https://guyinatuxedo.github.io/00-intro/index.html)
  -> Linux-focused binary exploitation tutorial series focused on memory bugs and control flow.

### Applied Reverse Engineering
* [wetw0rk](https://wetw0rk.github.io/)
* [dayzerosec Starter Guide](https://dayzerosec.com/blog/2024/07/11/getting-started-2024.html)
* [Wargames by ret2](https://wargames.ret2.systems/)

### Advanced / Kernel Exploitation

* [HackSysExtremeVulnerableDriver](https://github.com/hacksysteam/HackSysExtremeVulnerableDriver)
  -> Learn kernel-mode exploitation using a custom vulnerable Windows driver.

* [OSED Resource Collection](https://github.com/nop-tech/OSED/tree/main)
  -> Materials for OffSec’s Windows Exploit Development certification.

## Hands-On Practice

Challenge-based platforms and exercises to reinforce your skills.

* [crackmes.one](https://crackmes.one/)
* [pwnable.tw](https://pwnable.tw/challenge/)
* [PicoCTF](https://picoctf.org/)
* [Exploit Education](https://exploit.education/)

## Notable Resources
Trusted tools, references, and learning hubs in malware and reverse engineering.

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

## Miscellaneous
* [VXLab Book Archive](https://github.com/vxlabinfo/lib/tree/master)

## Contributors
Thanks to the following people:
* [@Lattice23](https://github.com/Lattice23) -> Helped with resources and structure

