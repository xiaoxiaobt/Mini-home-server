# Mini home server

> **Warning**
>
> This page is still under construction

## Home server in a nutshell

The home server is a desktop computer located at home that provides services for my own convenience and for users who access websites hosted on the server. At the time of writing, the home server is running on Windows 11 Pro, with Ubuntu 22.04 LTS Windows Sub-linux system (WSL) on the side. Currently, the home server is running the following services:

- Secure web hosting (with NGINX)
  - Private JupyterLab: <img alt="Jupyter" style="height:1rem" src="./misc/svg/jupyter.svg" />
  - Private Code Server: <img alt="Code server" style="height:1rem" src="./misc/svg/code-server.svg" /> 
  - Kodimpi (Backup): <img alt="Kodimpi" style="height:1rem" src="./misc/svg/kodimpi.svg" />
- Website monitoring
  - Distill.io (3rd-party managed service)
- Remote desktop
  - TeamViewer (3rd-party managed service)
  - Microsoft Remote Desktop
- SSH Server
- Media and file services
  - SMBv2/v3 local share with SMB Direct
- Dedicated light-weight computing resource in full-control (via SSH/Remote Desktop/Jupyter/Code Server)
  - PyTorch with CUDA
  - FFmpeg with CUDA

## Tasks

Tasks:

- [ ] DDNS
  - [ ] Asus DDNS
  - [ ] CNAME
- [ ] SSH
  - [ ] Connect to intranet computers
  - [ ] Connect to WSL via Windows
  - [ ] Changing default shell for Windows
- [ ] SMB
  - [ ] SMBv2/SMBv3
- [ ] Remote desktop
  - [ ] TODO: Microsoft remote desktop
  - [ ] TeamViewer
- [ ] Website hosting (multiple)
  - [ ] Port forwarding
  - [ ] Reverse proxy with NGINX
    - [ ] Compression
    - [ ] Multiple servers
      - [ ] Sub-domain
      - [ ] (Sub-)directory & slug direction
    - [ ] Redirect HTTP to HTTPS
    - [ ] Supports for IPv6
    - [ ] Fallback
  - [ ] HTTPS with CertBot
- [ ] Security
  - [ ] Router-level protection
    - [ ] DoS protection (Asus)
  - [ ] Website-level protection
    - [ ] DNS CAA
    - [ ] Robots.txt
  - [ ] OS-level protection
    - [ ] UAC
    - [ ] TPM
    - [ ] Memory integrity
    - [ ] Core isolation
- [ ] Automation
  - [ ] Update HTTPS certificates
  - [ ] Launch scripts
- [ ] System architecture
  - [ ] System configurations
    - [ ] UEFI and OS
    - [ ] Hardwares
    - [ ] Softwares
      - [ ] Cuda®
        - [ ] FFmpeg with NVIDIA GPU Hardware Acceleration
      - [ ] Python 3.11
      - [ ] Git
      - [ ] GnuPG
      - [ ] Visual Studio 2022
      - [ ] Visual Studio Code
      - [ ] Ubuntu 22.04 WSL
        - [ ] `screen` in WSL
  - [ ] Limitations
    - [ ] Windows Update
    - [ ] OS
    - [ ] Fallbacks
