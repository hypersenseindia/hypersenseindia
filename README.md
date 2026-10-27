<p align="center">
  <img src="https://raw.githubusercontent.com/hypersenseindia/hypersense-memory-analyzer/main/docs/assets/logo.png" width="116" alt="HYPERSENSEGLOBAL">
</p>

<h1 align="center">HYPERSENSEGLOBAL&trade;</h1>

<p align="center">
  <b>Usermode memory analysis &middot; Windows x64</b><br>
  <sub>Open-source tooling for malware triage, incident response and detection engineering</sub>
</p>

---

### Featured project

<a href="https://github.com/hypersenseindia/hypersense-memory-analyzer">
  <img src="https://raw.githubusercontent.com/hypersenseindia/hypersense-memory-analyzer/main/docs/assets/scan-results.png" width="100%" alt="HyperSense64 scanning explorer.exe">
</a>

**HyperSense64** &mdash; one 1.7 MB executable that scans a live process for injected memory and malware IOCs.

- Target search by image name, full path or PID
- `IOC` / `ALL` / `REGION` / `REFERENCED` modes, plus CLR heap, CLR JIT, WOW64 and unsigned-module filters
- Live colour-coded output, `STOP` cancels instantly
- TXT and HTML reports with host, SID, OS build and full engine log
- Moneta engine built in &mdash; no second binary, no installer, no driver, no telemetry

<p>
  <a href="https://github.com/hypersenseindia/hypersense-memory-analyzer/releases/latest">
    <img alt="Download HyperSense64" src="https://img.shields.io/badge/download-HyperSense64.exe-22d3ee?style=flat-square">
  </a>
  <a href="https://github.com/hypersenseindia/hypersense-memory-analyzer">
    <img alt="Source code" src="https://img.shields.io/badge/source-GitHub-181717?style=flat-square">
  </a>
  <img alt="Licence GPL-3.0" src="https://img.shields.io/badge/licence-GPL--3.0-blue?style=flat-square">
  <img alt="Platform Windows x64" src="https://img.shields.io/badge/platform-Windows%20x64-0ea5e9?style=flat-square">
</p>

### What I care about

| | |
| --- | --- |
| **Fault isolation** | The scanner runs as a hidden child process. A bad target costs you a scan, not the window. |
| **No magic** | No kernel driver, no service, no persistence, no network calls. It reads memory and writes the report you asked for. |
| **Honest licences** | Built on [Moneta](https://github.com/forrest-orr/moneta) (GPLv3). Every change is documented in [NOTICE.md](https://github.com/hypersenseindia/hypersense-memory-analyzer/blob/main/NOTICE.md). |
| **Real reports** | Whatever the UI shows, the report contains &mdash; uncapped, timestamped, reproducible from the equivalent command line. |

### Elsewhere

<a href="https://github.com/hypersenseindia/hypersense-memory-analyzer/releases"><img alt="Releases" src="https://img.shields.io/badge/releases-v1.0.1-22d3ee?style=flat-square"></a>
<a href="https://www.instagram.com/hydraxff_yt/"><img alt="Instagram" src="https://img.shields.io/badge/instagram-@hydraxff__yt-E4405F?style=flat-square"></a>

---

<p align="center">
  <sub>
    Engine: <a href="https://github.com/forrest-orr/moneta">Moneta</a> &mdash;
    Forrest Orr (<a href="https://github.com/forrest-orr">@forrest-orr</a>) &amp;
    Gabriel Landau (<a href="https://github.com/gabriellandau">@gabriellandau</a>), GPLv3.<br>
    Front end, packaging and branding: AG HYDRAXFF.
  </sub>
</p>

<p align="center">
  <sub>Use only on systems you own or are authorised to test.</sub>
</p>
