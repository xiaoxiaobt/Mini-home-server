# Mini home server

> **Warning**
>
> This page is still under construction

## Home server in a nutshell

The home server is a desktop computer located at home that provides services for my own convenience and for users who access websites hosted on the server. At the time of writing, the home server is running Windows 11 Pro, with Ubuntu 22.04 LTS WSL on the side. The home server will be migrated to utilize Proxmox VE at some point to allow multiple systems running in parallel. Currently, the home server is running the following services:

- Secure web services (with NGINX)
  - Private JupyterLab: <img alt="Jupyter" style="height:1rem" src="./misc/svg/jupyter.svg" />
  - Private Code Server: <img alt="Code server" style="height:1rem" src="./misc/svg/code-server.svg" />
  - Kodimpi (Backup): <img alt="Kodimpi" style="height:1rem" src="./misc/svg/kodimpi.svg" />
  - TODO: Backend server that connects to ChatGPT API
- Website monitoring
  - Distill.io (3rd-party managed service)
- Remote desktop
  - Microsoft Remote Desktop
- SSH Server
- Media and file services
  - SMBv2/v3 local share
  - Plex media server
- Local llama (7B)
- Dedicated light-weight computing resources in full-control (via SSH/Remote Desktop/Jupyter/Code Server)
  - PyTorch with CUDA
  - TODO: FFmpeg with CUDA

## Tasks

Tasks:

- [X] DDNS
  - [X] Asus DDNS
  - [X] CNAME
  - [ ] IPv6
- [X] SSH
  - [X] Connect to intranet computers
  - [X] Changing default shell for Windows
- [X] Remote desktop
  - [X] Microsoft remote desktop
- [X] Website hosting (multiple)
  - [X] Port forwarding
  - [X] Reverse proxy with NGINX
    - [X] Compression
    - [X] Multiple servers
      - [X] Sub-domain
      - [X] (Sub-)directory & slug direction
    - [X] Redirect HTTP to HTTPS
    - [X] Supports for IPv6
    - [X] Fallbacks
    - [X] HTTP/2
    - [ ] HTTP/3
    - [ ] NGINX 64-bit
- [ ] Security
  - [ ] Cloud security
    - [ ] Cloudflare tunnel
  - [X] Router-level measurements
    - [X] DoS protection (Asus)
    - [X] Wireguard VPN
  - [X] Website-level protection
    - [X] DNS CAA
    - [X] Robots.txt
  - [X] Windows OS-level protection
    - [X] UAC
    - [X] TPM
    - [X] Memory integrity
    - [X] Core isolation
- [X] Automation
  - [X] CertBot auto-renewal
  - [X] Launch scripts
- [ ] System architecture
  - [ ] System configurations
    - [X] UEFI and OS
    - [X] Hardwares
    - [ ] OS and Softwares
      - [ ] Proxmox VE and configurations
      - [X] Windows 11 Pro
        - [X] Visual Studio 2022
        - [X] GnuPG
        - [X] Plex media server
        - [X] SMBv2/v3 local share
        - [X] Microsoft Remote Desktop
        - [X] NGINX
        - [X] CertBot
        - [X] CUDA (in TCC mode)
        - [X] Ubuntu 22.04 LTS WSL
      - [ ] Ubuntu 22.04 LTS
        - [ ] Mamba and Conda
        - [ ] CUDA
          - [ ] FFmpeg with NVIDIA GPU Hardware Acceleration
          - [ ] PyTorch with CUDA
        - [ ] Docker
        - [ ] GnuPG
- [ ] System monitoring
- [ ] Limitations
  - [ ] Windows Update
  - [ ] OS
  - [ ] Fallbacks
