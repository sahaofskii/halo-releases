# Halo

**A fast, simple VPN client for Windows, built on Xray and sing-box.**

Paste your subscription link, press Connect, and Halo keeps you on the fastest server that actually works.

**[Download the latest version](../../releases/latest)** · Windows 10 (1809) or newer, 64-bit · English and Persian

---

## Why Halo

### Always on the best server
- **Smart Auto-Switch.** Halo tests your servers every few minutes and moves you only when another one is clearly faster, or at once when yours stops working. Connections you already have open are never cut.
- **It knows when the problem is your internet, not the server.** Before Halo marks a server as failed, it checks your own connection. If your internet is down, no server is blamed; Halo waits and carries on by itself.
- **A UDP check for calls and games.** Halo finds servers that drop UDP, where voice calls, games and some video fail, marks them "no UDP" and prefers servers that carry it.
- **Best now.** One card shows the fastest server right now. One click connects.

### Works with the apps other VPNs miss
- **No more "not available in your region" in developer tools.** Cursor, VS Code, Codex, npm, git, pip and many other tools ignore the Windows proxy. Halo also sets the proxy variables they read, so they go through the VPN too, without TUN.
- **System Proxy or TUN, switch any time.** TUN takes every app on your PC; System Proxy needs no administrator rights.
- **Split tunneling per app.** Choose the apps that skip the VPN, or the only apps that use it. Or go Full tunnel: everything through the VPN.
- **Smart routing for Iran.** Iranian sites go direct, everything else through the VPN. Add your own sites that always go direct, or always through the VPN.
- **Anti-sanction DNS.** The DNS tab finds the fastest DNS for Windows and opens games and stores that block Iranian users, even with the VPN off.

### Protected
- **A Kill Switch that survives a crash.** In TUN mode, if Halo closes without Disconnect (a crash, Task Manager, a power cut), your traffic stays blocked. Nothing leaves outside the VPN.
- **No leaks around the tunnel.** In TUN mode, programs that try to go around the tunnel, such as a browser's WebRTC, are blocked.
- **TLS fragment and Mux** for heavily filtered networks.
- **Encrypted on your PC.** Subscription links and server passwords are encrypted with Windows' own protection (DPAPI) for your account only.
- **Signed updates.** Every update is signed; Halo checks it before it installs anything.

### Everything in sight
- **Built-in speed test.** Ping, jitter, download and upload, through the VPN or direct, with test servers by region.
- **Data use per app, per server and per day,** with a chart and any date range.
- **Speed tests that respect your data.** At most 2 MB per server, and "fastest real speed" is measured from your own traffic at no cost.
- **Subscription data and days left** at a glance, with automatic updates on your schedule.

### Easy
- Add servers from a link, a subscription, a QR code (even one on your screen), or a sing-box JSON or Clash YAML file.
- VLESS, VMess, Trojan, Shadowsocks, Hysteria2, TUIC, SSH and SOCKS.
- Share a server or a whole subscription with a QR code.
- Built-in Help in English and Persian, linked from the errors you see.
- The installed version updates itself from inside the app.

---

## Download

Get the newest version from **[Releases](../../releases/latest)**.

| File | For |
|---|---|
| `Halo-Setup-<version>.exe` | **Most people.** Installs Halo and updates itself from inside the app. |
| `Halo-Portable-<version>.zip` | No install: unzip and run `Halo.exe`. Settings stay in its own folder. |

## Check the file

Each release has a `SHA256SUMS.txt`. In PowerShell:

```powershell
Get-FileHash .\Halo-Setup-<version>.exe -Algorithm SHA256
```

The hash must match the line for that file.

## Privacy

Halo has no crash upload and no third-party analytics. It sends only a few anonymous counts per day (such as the version and whether connecting works), and only through your VPN server, never from your own address.

## License

Halo is free software under the GPL-3.0. It includes sing-box (GPL-3.0), Xray-core (MPL-2.0) and Wintun; their licenses are in the `licenses` folder of every download.
