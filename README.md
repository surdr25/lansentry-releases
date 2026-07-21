# LANsentry — Releases

This repository hosts the official installer downloads for **LANsentry**, a
Windows network security scanner (host discovery, port scan, CVE
prioritization, AI analysis, active pentest).

**This repository contains no source code.** LANsentry's source is closed /
private; this repo exists solely so release binaries can be distributed via
a public, trusted `github.com` URL alongside the primary download at
[lansentry.com](https://lansentry.com).

## Verifying a download

Each release lists the installer's SHA256 checksum. On Windows, verify with:

```powershell
Get-FileHash LANsentry-Setup-X.Y.Z.exe -Algorithm SHA256
```

Compare the output against the checksum shown on the [Releases page](../../releases)
or on [lansentry.com](https://lansentry.com).

## More info

- Website: https://lansentry.com
- Support: dirk@247-it.de
