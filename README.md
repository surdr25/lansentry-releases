# LANsentry

**Network security scanning for Windows — host discovery, CVE prioritization, AI analysis, and active pentesting in a single standalone app. No cloud, all data stays local.**

🔗 **Website & full feature list: [lansentry.com](https://lansentry.com)**

---

## What is this repository?

This repo hosts **only the release binaries** for LANsentry — the application's
source code is closed/private. It exists to give users a trusted, publicly
verifiable download source (with SHA256 checksums) alongside the primary
download at [lansentry.com](https://lansentry.com).

**👉 [Download the latest installer](../../releases/latest)**

## What LANsentry does

- **Smart network discovery** — ICMP ping, TCP-connect fallback for firewalled hosts, plus SSDP/mDNS for UPnP and Bonjour devices with friendly names
- **Native port scanner** — parallel TCP scan with banner grabbing and version detection, no nmap required (optional nmap integration adds OS detection)
- **CVE prioritization** — CISA KEV flags actively-exploited vulnerabilities, EPSS scores exploitation probability — not just raw CVSS
- **AI-powered analysis** — Anthropic, OpenAI, OpenRouter, or local Ollama — returns an executive summary and a remediation plan
- **Active pentest module** — nmap NSE vulnerability scripts + 5,000+ nuclei templates (SSL/TLS, SMB, default credentials, HTTP security headers, and more)
- **WAN scan** — detects your public IP and checks which ports/CVEs are exposed from the outside
- **Network topology map** — visual host map with severity coloring, exportable as PNG/SVG
- **Reports & export** — HTML, Excel, JSON, CSV, PDF — all generated locally, no cloud round-trip
- **Device fingerprinting** — classifies hosts into router, server, NAS, printer, IP camera, smart home, and more
- **Background monitoring** — an optional Windows service keeps scanning while the app is closed and alerts via email, Slack or Telegram when a new device appears or a device goes offline
- **Wake-on-LAN**, persistent device labels/groups, scan history with diffing, scheduled automatic scans, SNMP interface stats, DHCP/ARP overview, and firewall/port-knock detection
- **Bilingual UI** (English/German) — switchable anytime in Settings
- **7-day free trial**, then **€69 one-time per device** (no subscription) via Polar.sh — [pricing details](https://lansentry.com/pricing.txt)

See the full feature breakdown, screenshots and FAQ at **[lansentry.com](https://lansentry.com)**.

## Guides

Practical network-security guides on lansentry.com (English and German):

- [CVE, CVSS, EPSS and KEV explained](https://lansentry.com/guides/cve-cvss-epss-kev-explained.html) — prioritize patching by real-world exploitation
- [How to find and close open ports](https://lansentry.com/guides/open-ports-guide.html)
- [How to find unknown devices on your network](https://lansentry.com/guides/unknown-devices-network.html)
- [Secure Windows network checklist](https://lansentry.com/guides/secure-windows-network-checklist.html)
- [Network pentesting and the law](https://lansentry.com/guides/network-pentesting-legal-guide.html)
- [Network topology mapping](https://lansentry.com/guides/network-topology-mapping.html)
- [All guides in German](https://lansentry.com/de/guides/)

## Verifying a download

Every release lists the installer's SHA256 checksum in its notes. On Windows, verify with:

```powershell
Get-FileHash LANsentry-Setup-X.Y.Z.exe -Algorithm SHA256
```

Compare the output against the checksum shown on the [latest release](../../releases/latest)
or on [lansentry.com](https://lansentry.com).

## Support & contact

- Website: https://lansentry.com
- Support: mail@247-it.de

---

*LANsentry is developed and published by 247-IT. This repository intentionally contains no application source code.*
