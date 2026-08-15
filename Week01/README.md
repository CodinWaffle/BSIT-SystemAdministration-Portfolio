# Week 1 – Building My Professional Environment

## Student Information
- **Name:** Jose Martin R. Imperial
- **Course:** Bachelor of Science in Information Technology (BSIT) – ITEP 414 System Administration and Maintenance
- **Section:** 4D
- **Date:** August 15, 2026

---

# Objectives
This session covered all three Week 1 activities — Software Installation, Professional Account Creation, and the Professional Portfolio Repository. The goals were:
1. **Environment Setup:** Install and configure the core tools required for system administration work: Git, GitHub Desktop, Visual Studio Code, and VirtualBox.
2. **Virtualization Practice:** Create and successfully install a working Ubuntu Server VM and a Windows 11 VM using VirtualBox, gaining hands-on experience with manual OS installation and VM troubleshooting.
3. **Digital Identity:** Establish and customize professional online profiles on GitHub and LinkedIn for technical branding and portfolio showcasing.
4. **Repository Architecture:** Create and structure the semester-long GitHub portfolio repository (`BSIT-SystemAdministration-Portfolio`) containing folders from `Week01` to `Week15`.
5. **Version Control Management:** Practice git repository initialization, commit operations, and remote synchronization with GitHub.
6. **Documentation:** Document software installation, account verification, and repository layout in Markdown.

---

# Software Installed
- Git (version 2.55.0)
- GitHub Desktop (Linux community build via the shiftkey-desktop repository, since GitHub does not officially support Linux)
- Visual Studio Code
- VirtualBox
- Ubuntu Server 26.04 LTS (installed as a VirtualBox VM)
- Windows 11 (installed as a VirtualBox VM)

---

# Activity 2: Professional Accounts

- **GitHub Profile:** https://github.com/CodinWaffle
- **LinkedIn Profile:** https://www.linkedin.com/in/jose-martin-r-imperial-53a2b429a/

---

# Activity 3: Repository Structure

The semester portfolio repository has been initialized with the standard 15-week directory hierarchy:

```text
BSIT-SystemAdministration-Portfolio/
├── Week01/
│   ├── accounts/
│   ├── screenshots/
│   └── README.md
├── Week02/
├── Week03/
├── Week04/
├── Week05/
├── Week06/
├── Week07/
├── Week08/
├── Week09/
├── Week10/
├── Week11/
├── Week12/
├── Week13/
├── Week14/
└── Week15/
```

---

# Installation Screenshots
See `Week01/screenshots/` for verification screenshots of Git, GitHub Desktop, VS Code, VirtualBox, the Ubuntu Server VM, and the Windows 11 VM. Each screenshot shows the software running alongside a text file with my name and section for verification.

---

# Challenges Encountered

1. **Ubuntu Server install hanging during file copy**
   During my first attempt to install Ubuntu Server, the installer got stuck on "Copying files..." for over an hour, and the logs showed a repeating `rsync: connection unexpectedly closed` error. I resolved this by powering off the VM, deleting it, and starting a fresh install.

2. **Kernel crash during file extraction**
   On a later attempt, the install crashed with a kernel panic while `rsync` was extracting install files, likely due to insufficient RAM allocated to the VM (2048 MB). I increased the VM's base memory to 4096 MB, which allowed the installation to complete successfully without further crashes.

3. **Losing track of login credentials from an unattended install**
   An ISO I used triggered an automated "unattended" installation that set a username and password automatically, which I did not note down and could not later recall. Rather than trying to recover the forgotten credentials, I deleted the VM and reinstalled Ubuntu Server, this time watching for autoinstall prompts and confirming my own credentials as I set them.

4. **Typo in a package installation command**
   While installing GitHub Desktop via `dnf`, I initially ran `sudo dnf github-desktop -y`, missing the required `install` subcommand, which caused an "Unknown argument" error. Re-running the command as `sudo dnf install github-desktop -y` resolved it.

---

# Reflection

This week gave me a much deeper understanding of what it actually takes to set up and maintain a working system administration environment — not just the tools themselves, but the troubleshooting process around them. Installing Ubuntu Server was the most instructive part of the week: my first two attempts failed for different reasons (a wrong boot mode, then a memory-related kernel crash), and each failure taught me something concrete about how virtual machines behave, how to read installer logs, and how resource allocation affects stability during installation.

I also learned that virtual machines are genuinely isolated from the host system, which meant I could break, delete, and rebuild my Ubuntu VM multiple times without any risk to my actual Fedora installation. That gave me the confidence to keep troubleshooting instead of panicking when something failed. Losing track of login credentials from an unattended install was frustrating, but it taught me a habit I will carry forward: always confirm and record credentials the moment they are set, especially during automated or scripted setups.

Setting up GitHub, LinkedIn, and the semester portfolio repository felt more straightforward by comparison, but it reinforced why documentation and organization matter from day one. Keeping every activity, script, and screenshot properly tracked in version control means my work is reproducible and easy to hand off or present later, which is exactly the kind of discipline a System Administrator needs. Overall, this week's mix of small technical wins and repeated failures gave me a realistic first taste of what ongoing system administration work actually looks like.

---

# References
- Git documentation – https://git-scm.com/doc
- GitHub Desktop (Linux build) – https://github.com/shiftkey/desktop
- Ubuntu Server documentation – https://ubuntu.com/server/docs
- VirtualBox documentation – https://www.virtualbox.org/wiki/Documentation
- LinkedIn Help Center – https://www.linkedin.com/help/linkedin