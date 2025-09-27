# Laboratory 1 – Ubuntu 22.04.5 LTS Installation (VMware)

This repository contains the lesson presentation and setup resources for **Laboratory 1: Ubuntu 22.04.5 LTS Installation on VMware Workstation**. 
It's designed as a learning resource to help students and IT professionals set up Ubuntu in a virtualized environment for lab and training purposes.

---

## 📂 Repository Contents

* `Laboratory 1 Ubuntu 22.04.5 LTS Installations.pptx`
    * A presentation file with step-by-step instructions for installing Ubuntu 22.04.5 LTS on VMware.
* `setup/` *(if included)*
    * Contains the VMware setup file(s) required for creating the virtual machine.

---

## 🖥️ Requirements

* **Host Machine**: Windows, Linux, or macOS with at least **8 GB RAM** and **100 GB** free disk space.
* **Virtualization Software**: **VMware Workstation 17** or later.
* **Ubuntu ISO**: [Ubuntu 22.04.5 Desktop (64-bit)](https://releases.ubuntu.com/releases/22.04.5/ubuntu-22.04.5-desktop-amd64.iso)

---

## ⚙️ Installation Steps (Summary)

1.  Install **VMware Workstation 17** on your host machine.
2.  Create a new virtual machine (`File > New Virtual Machine` or press `CTRL+N`).
3.  Select the Ubuntu 22.04.5 ISO as the installation source.
4.  Allocate resources conservatively (e.g., **2–4 GB RAM**, **1–2 CPUs** per VM).
5.  Configure the virtual hard disk (recommended: **100 GB**, split option enabled).
6.  Complete the installation by following the on-screen steps.
7.  After the first boot, **skip online accounts** and **avoid upgrading to Ubuntu 24.04**.
8.  Run updates for Ubuntu 22.04.5 and install essential tools:

```bash
sudo apt-get update
sudo apt-get install -y build-essential curl wget git vim net-tools ssh rsync nano unzip

## 🔑 Default Lab Credentials

| Component | Value |
| :--- | :--- |
| **Username** | `dde` |
| **Password** | `dde` (lowercase) |

---

## 📌 Notes & Best Practices

* **Do NOT upgrade to Ubuntu 24.04.1 LTS.** This lab requires **Ubuntu 22.04.5 LTS** for compatibility.
* Allocate VM resources carefully to avoid overloading your host system.
* Use the following commands for system management:

```bash
# Check Ubuntu version
lsb_release -a

# Restart system
sudo reboot

# Check hostname
cat /etc/hostname

## 📚 Additional Resources

* **Official Ubuntu Documentation**: [Ubuntu Documentation](https://help.ubuntu.com/)
* **VMware Workstation Pro**: [VMware Workstation Pro](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)
* **YouTube Guide: Ubuntu 22.04 Installation on VMware**: [Install Ubuntu 22.04 on VMware Workstation Pro (Step-by-Step)](https://www.youtube.com/watch?v=uvn7HQcivh4)

---

## 📜 License

This repository is for educational purposes. Please consult your instructor before making modifications to the setup.