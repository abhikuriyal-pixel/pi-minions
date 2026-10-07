# PiMinions

**Your AI teammates, together on your desktop.**

PiMinions is a Windows desktop assistant with persistent conversations, a central Chief coordinator, approval-gated tools and an integrated DocFoo document-retrieval teammate.

[Download releases](https://github.com/abhikuriyal-pixel/PiMinions/releases) · [Report a problem](https://github.com/abhikuriyal-pixel/PiMinions/issues) · [Support](SUPPORT.md)

> **Code coming soon..**
> This repository currently hosts public documentation and binary releases. Application implementation and development history are maintained privately; no source-publication date is committed.

## Highlights

- Persistent named AI teammates and coordinated task delegation.
- Isolated bot browsing and explicit action approvals.
- Document attachments, citations, figures and indexed DocFoo knowledge retrieval.
- Optional Telegram access and Marimo notebooks.
- Dark/light themes and locally stored conversations/settings.

## Install · Windows x64

Choose a version from [Releases](https://github.com/abhikuriyal-pixel/PiMinions/releases):

| Asset | Use |
| --- | --- |
| `PiMinions-<version>-win-x64-Setup.exe` | Standard NSIS installation |
| `PiMinions-<version>-win-x64.zip` | Extract once, then run `PiMinions.exe` |
| `SHA256SUMS.txt` | SHA-256 values for both downloads |

Verify your download in PowerShell and compare with that release's manifest:

```powershell
Get-FileHash .\PiMinions-<version>-win-x64.zip -Algorithm SHA256
```

Releases are **unsigned**; Windows may show SmartScreen warnings. Do not bypass a warning without checking the repository, artifact and checksum. macOS, Linux and Windows ARM builds are not offered.

## First run and privacy

Connect a supported model provider in **Settings & providers → Providers**. Provider/API usage may be billed by that provider. Optional integrations require their own setup; DocFoo can be installed from its dedicated space using the public [DocFoo CLI releases](https://github.com/abhikuriyal-pixel/docfoo-cli/releases).

Model requests and enabled integrations contact their providers. Provider credentials saved through the app use OS encryption; transcripts, library files and browser storage are not generally encrypted. Approved scripts/Python are not an OS sandbox. Review permissions and avoid sharing private content in issue reports.

## Release policy

Versioned downloads are checksummed and never silently replaced. Migrated historical versions preserve their original bytes and release notes; they do not represent the newest development source. GitHub's automatic **Source code** archives contain this repository's documentation, not the application implementation. Packaged Electron runtime code remains inspectable.

## License and security

[MIT License](LICENSE), with third-party components under their respective licenses. New packaging/license files apply to future builds; historical assets are not rebuilt. See [SECURITY.md](SECURITY.md) for private vulnerability reporting.
