<p align="center">
  <img src="https://raw.githubusercontent.com/hypersenseindia/hypersense-memory-analyzer/main/docs/assets/logo.png" width="112" alt="HYPERSENSEGLOBAL">
</p>

<h1 align="center">HYPERSENSEGLOBAL&trade;</h1>

<p align="center">
  <b>Windows security tooling</b> &middot; detection engineering &middot; Android performance<br>
  <sub>Small, dependency-free tools that each do one job properly.</sub>
</p>

<p align="center">
  <a href="https://github.com/hypersenseindia/hypersense-memory-analyzer/releases/latest">
    <img alt="Latest release" src="https://img.shields.io/github/v/release/hypersenseindia/hypersense-memory-analyzer?color=22d3ee&label=release&style=flat-square">
  </a>
  <img alt="Platform Windows x64" src="https://img.shields.io/badge/platform-Windows%20x64-0ea5e9?style=flat-square">
  <img alt="C++17" src="https://img.shields.io/badge/C%2B%2B-17-00599c?style=flat-square">
  <img alt="Licence GPL-3.0" src="https://img.shields.io/badge/licence-GPL--3.0-blue?style=flat-square">
</p>

---

## Flagship &mdash; HyperSense64

<a href="https://github.com/hypersenseindia/hypersense-memory-analyzer">
  <img src="https://raw.githubusercontent.com/hypersenseindia/hypersense-memory-analyzer/main/docs/assets/scan-results.png" width="100%" alt="HyperSense64 scanning explorer.exe">
</a>

**Live usermode memory analysis for Windows.** One 1.7 MB executable with the
[Moneta](https://github.com/forrest-orr/moneta) engine compiled in &mdash; no second binary, no
installer, no driver, no telemetry. Pick a running process, scan its memory for injected
regions and malware IOCs, export the result.

| | |
| --- | --- |
| **Target search** | Filter the process list by image name, full path or PID, with a live match count |
| **Modes** | `IOC` / `ALL` / `REGION` / `REFERENCED`, plus CLR heap, CLR JIT, WOW64 and unsigned-module filters |
| **Live output** | Colour-coded streaming; `STOP` terminates the scan child instantly |
| **Reports** | TXT and HTML, including host, SID, OS build, options, timings and the full engine log |
| **Isolation** | The scanner runs as a hidden child process, so a bad target costs a scan, not the window |

<p>
  <a href="https://github.com/hypersenseindia/hypersense-memory-analyzer/releases/latest">
    <img alt="Download HyperSense64" src="https://img.shields.io/badge/download-HyperSense64.exe-22d3ee?style=flat-square">
  </a>
  <a href="https://github.com/hypersenseindia/hypersense-memory-analyzer">
    <img alt="Source code" src="https://img.shields.io/badge/source-GitHub-181717?style=flat-square">
  </a>
  <a href="https://github.com/hypersenseindia/hypersense-memory-analyzer/blob/main/NOTICE.md">
    <img alt="Changes vs upstream" src="https://img.shields.io/badge/attribution-NOTICE.md-6b7280?style=flat-square">
  </a>
</p>

---

## Security tooling

| Project | What it does | Stack |
| --- | --- | --- |
| [**HyperSense64**](https://github.com/hypersenseindia/hypersense-memory-analyzer) | Usermode memory analysis &mdash; finds injected and suspicious regions in a live process | `C++` `Win32` |
| [**Sysmon Deployment Suite**](https://github.com/hypersenseindia/Sysmon-Deployment-Suite) | Menu-driven Sysmon rollout using the Olaf Hartong config, tuned for Event ID 7 (Image Load) and 10 (Process Access) | `PowerShell` |
| [**HYPERINFO**](https://github.com/hypersenseindia/HYPERINFO-FINAL) | Terminal OSINT &mdash; passive WHOIS, `crt.sh`, Shodan and banner lookups on an IP or hostname | `Bash` |
| [**Phishing Analyzer**](https://github.com/hypersenseindia/-Ultimate-Pro-Phishing-Analyzer) | Flask service that scores a URL with VirusTotal, URLScan.io, WHOIS and DNS, and flags dead or lookalike domains | `Python` |
| [**HX Injector**](https://github.com/hypersenseindia/ADVANCEDHXINJECTOR) | Authorised red-team DLL injector &mdash; indirect syscalls, APC injection, encrypted payload staging | `C++` |

## Android performance (Termux, non-root)

| Project | What it does | Stack |
| --- | --- | --- |
| [**Hypersense MAX v10**](https://github.com/hypersenseindia/Hypersense-MAX-v10) | Frame smoothing, touch response and VRAM/CPU hints with idle/active switching | `Bash` |
| [**Neural vPool / uVRAM Engine**](https://github.com/hypersenseindia/neural-vpool-uvram-engine-v11) | Frame-pacing engine for 60&ndash;144 Hz targets, with a virtual memory pool | `Bash` |
| [**Hypersense Ultimate**](https://github.com/hypersenseindia/Hypersense-Ultimate) | Auto game detection, dynamic touch/FPS scaling, battery and thermal limits | `Bash` |
| [**Hypersense Android V2**](https://github.com/hypersenseindia/Hypersense-Android-V2) | NeuralCore build with per-game profiles | `Bash` |

## Web and experiments

| Project | What it does | Stack |
| --- | --- | --- |
| [**HyperGhostChat**](https://github.com/hypersenseindia/HYPERGHOSTCHAT) | Single-file browser chat interface | `HTML` |
| [**GameDeploy**](https://github.com/hypersenseindia/GameDeploy) | Landing page for the game deploy service | `HTML` |
| [**PC Checking Kit**](https://github.com/hypersenseindia/pc-checking-kit) | Windows health-check log bundle | &mdash; |

<sub>Older builds and duplicates stay public but unmaintained &mdash; the versions above are the ones to use.</sub>

---

## How these are built

| | |
| --- | --- |
| **No magic** | No kernel driver, no background service, no telemetry, no hidden network calls. A tool does what its name says. |
| **Portable first** | Single executables and single scripts. Copy it, run it, delete it &mdash; nothing to install. |
| **Fault isolation** | The scan runs in a child process. A crash costs a scan, not the session. |
| **Honest licences** | Work built on someone else's engine credits it and documents every change ([NOTICE.md](https://github.com/hypersenseindia/hypersense-memory-analyzer/blob/main/NOTICE.md)). |
| **Real output** | Reports carry timestamps, host context and the complete log &mdash; not a summary you have to trust. |

---

<p align="center">
  <sub>
    Engine work on HyperSense64: <a href="https://github.com/forrest-orr/moneta">Moneta</a> by
    Forrest Orr (<a href="https://github.com/forrest-orr">@forrest-orr</a>) and
    Gabriel Landau (<a href="https://github.com/gabriellandau">@gabriellandau</a>), GPLv3.<br>
    Front end, packaging and branding: AG HYDRAXFF &middot;
    <a href="https://www.instagram.com/hydraxff_yt/">@hydraxff_yt</a>
  </sub>
</p>

<p align="center">
  <sub>Use only on systems you own or are authorised to test.</sub>
</p>
