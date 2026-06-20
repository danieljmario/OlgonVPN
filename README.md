<div align="center">

# OlgonVPN

**Fast, secure and reliable VPN for everyday privacy.**

Windows · Linux · Portable · Installer

</div>

---

## About

OlgonVPN is a privacy-focused VPN client that encrypts your internet traffic and
protects your data on public and private networks. It adapts the connection
automatically to keep your session stable and responsive.

---

## Download

### Windows

| File | Type | Architecture |
|------|------|-------------|
| [`OlgonVPN_0.1.0_x64-setup.exe`](windows/OlgonVPN_0.1.0_x64-setup.exe) | Installer (NSIS) | 64-bit |
| [`OlgonVPN_0.1.0_x64_en-US.msi`](windows/OlgonVPN_0.1.0_x64_en-US.msi) | Installer (MSI) | 64-bit |
| [`olgonvpn-desktop-windows-amd64.zip`](windows/olgonvpn-desktop-windows-amd64.zip) | Desktop (no install) | 64-bit |
| [`olgonvpn-portable-windows-amd64.zip`](windows/olgonvpn-portable-windows-amd64.zip) | Portable | 64-bit |
| [`olgonvpn-portable-windows-x86.zip`](windows/olgonvpn-portable-windows-x86.zip) | Portable | 32-bit |

### Linux

| File | Type | Architecture |
|------|------|-------------|
| [`olgonvpn-portable-linux-amd64.tar.gz`](linux/olgonvpn-portable-linux-amd64.tar.gz) | Portable | 64-bit (PC / Server) |
| [`olgonvpn-portable-linux-arm64.tar.gz`](linux/olgonvpn-portable-linux-arm64.tar.gz) | Portable | ARM64 (Raspberry Pi / ARM) |

> Current version: **0.1.0**

---

## Installation

### Windows — Installer (recommended)

1. Download `OlgonVPN_0.1.0_x64-setup.exe`.
2. Run it and follow the wizard.
3. Open **OlgonVPN** from the Start menu.

### Windows — MSI (enterprise / GPO)

```powershell
msiexec /i OlgonVPN_0.1.0_x64_en-US.msi
```

Silent install:

```powershell
msiexec /i OlgonVPN_0.1.0_x64_en-US.msi /qn
```

### Windows — Portable (no install required)

1. Download the portable ZIP for your architecture (amd64 = 64-bit, x86 = 32-bit).
2. Extract to any folder.
3. Run `olgonvpn-portable.exe` as **Administrator**.

### Linux — Portable

```bash
tar -xzf olgonvpn-portable-linux-amd64.tar.gz
sudo ./olgonvpn-portable
```

For ARM64 (Raspberry Pi, etc.):

```bash
tar -xzf olgonvpn-portable-linux-arm64.tar.gz
sudo ./olgonvpn-portable
```

> Linux portable opens a browser-based UI at `http://127.0.0.1:17070` automatically.

---

## Requirements

### Windows
- Windows 10 or 11
- Administrator privileges on first launch (to create the network interface)
- WinTUN driver — included in the portable ZIP and installed automatically by the installer

### Linux
- Kernel 4.14+ with WireGuard support (most distros since 2020)
- `root` / `sudo` to create TUN interface
- A browser for the web UI (opens automatically)

---

## Getting started

1. Open the app.
2. Log in with your OlgonVPN account (or create one).
3. Choose a server.
4. Click **Connect**.

To get a voucher or activate a plan: <https://olgonvpn.wmzs.link>

---

## Verify integrity (optional)

```powershell
# Windows
Get-FileHash .\windows\olgonvpn-portable-windows-amd64.zip -Algorithm SHA256
```

```bash
# Linux
sha256sum olgonvpn-portable-linux-amd64.tar.gz
```

---

## Support

- Website: <https://olgonvpn.wmzs.link>
- Email: support@olgonvpn.com

---

## Notice

This repository is intended for **distribution** of the application only.
Do not include source code, private keys, or debug files in this folder.
Use OlgonVPN in accordance with your local laws and your network provider's terms of service.

<div align="center">

© 2026 OlgonVPN. All rights reserved.

</div>
