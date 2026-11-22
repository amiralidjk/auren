# Auren

Auren for Windows: release downloads and update checks.
Download the latest installer from [Releases](https://github.com/amiralidjk/auren/releases/latest).

## System requirements

|                 | Minimum                                                    | Recommended                                              |
|-----------------|------------------------------------------------------------|----------------------------------------------------------|
| **Windows**     | Windows 10 64-bit, version 1809 or newer                   | Windows 11 64-bit, fully updated                         |
| **Processor**   | 64-bit dual-core, x64 (Intel or AMD)                       | Quad-core or better                                      |
| **Memory**      | 4 GB RAM                                                   | 8 GB RAM or more                                         |
| **Graphics**    | DirectX 11 GPU with hardware acceleration on (most built-in Intel/AMD graphics from 2015 on) | A dedicated GPU, or recent built-in graphics, for many widgets on a 4K or high-refresh screen |
| **Storage**     | 500 MB free                                                | SSD with 1 GB free                                       |
| **Internet**    | Needed for sign-in and payment, then at least once every 14 days | Always-on connection for lyrics, artwork, weather and updates |

Auren draws every widget with your graphics card. The more widgets you turn on, and the bigger and faster your screen, the more GPU it uses. On a slower PC, turn on fewer widgets or lower the frame rate in **Performance**.

## Where Auren does not run

- **Windows 7, 8 and 8.1**: not supported (Auren is built on Electron 45, which needs Windows 10 or newer).
- **Windows 10 older than version 1809**: the Now Playing and lyrics widgets need the media controls added in 1809.
- **32-bit Windows**: not supported. The installer is 64-bit (x64) only.
- **Windows 10 on ARM**: not supported (it can't run x64 apps).
- **Windows 11 on ARM** (Snapdragon and similar): it may run through Windows' x64 emulation, but it has not been tested and is not supported.
- **Windows in S mode**: it can only install apps from the Microsoft Store. Leave S mode first.
- **Windows Server, virtual machines and remote desktop sessions**: not tested. Without a real GPU, widgets can be slow or blank.
- **macOS, Linux and ChromeOS**: no version exists. Auren uses Windows-only features (desktop layering, the taskbar, Windows media controls, system audio capture).

## Installing

1. Open the [official GitHub release](https://github.com/amiralidjk/auren/releases/latest). Under **Assets**, choose the Windows x64 installer.
2. To verify the download, open PowerShell in the folder containing the installer and calculate its SHA-256. Use the filename shown in the release. For example, for 0.1.45:

   ```powershell
   Get-FileHash -Algorithm SHA256 -LiteralPath .\Auren-0.1.45-Setup-x64.exe
   ```

   Compare the result with the SHA-256 displayed next to the installer in GitHub's Assets list. A match confirms you have the same file published on GitHub.

The installer is currently unsigned. On Windows 11, Smart App Control may block it if Windows can’t verify the publisher. If the installer is blocked, keep Windows protection enabled and [contact Auren support](https://github.com/amiralidjk/auren/issues) with the exact message and release version. [Microsoft’s Smart App Control guidance](https://support.microsoft.com/en-us/windows/security/threat-malware-protection/smart-app-control-frequently-asked-questions)
