# System Setup

This repository relies on open-source EDA tools that are best supported on Ubuntu 20.04 or later. While other Linux distributions may work, we recommend Ubuntu for maximum compatibility. If your system doesn't run Ubuntu (or Linux) natively, setting it up in a virtual machine (VM) is a straightforward way to get started.

For Windows users, Oracle VM VirtualBox is a solid choice. macOS users can opt for UTM or similar tools. Regardless of your VM software, aim for these minimum specifications to ensure smooth performance with the EDA tools:

- **RAM:** 6 GB
- **Storage:** 50 GB
- **OS:** Ubuntu 20.04 or later (LTS versions preferred for stability)
- **vCPU:** 4

## Alternative Setup: Dual-Booting for Better Performance

VMs are convenient but can reduce performance by sharing resources with your host OS (Windows or macOS). For direct hardware access and optimal efficiency, consider dual-booting Ubuntu alongside your primary OS.

### For Apple Silicon Macs
You can install Ubuntu natively using Asahi Linux. Follow this step-by-step tutorial by YouTuber kskroyal:  
[Install Ubuntu 24.04 on M1/M2 Macs Natively Using Asahi Linux](https://www.youtube.com/watch?v=60wxAi8EJow)  

**Note:** I've successfully installed Ubuntu 24.04 on an M1 Mac (8GB RAM, 256GB storage) via Asahi Linux, allocating 70GB to Ubuntu. Ensure you allocate sufficient storage based on your needs.
