# TITAN.ATLAS Free

**Free public beta installers for TITAN.ATLAS Free on Windows, macOS and Ubuntu.** No checkout and no account are required to download.

This repository carries the installers, their checksums and an issue tracker for beta feedback. The application source is not published here.

| Platform | Version | Installer | SHA-256 |
| :--- | :--- | :--- | :--- |
| Windows 10 or 11, 64-bit | 0.1.6 beta | `titan-atlas-free_0.1.6_windows-x64-setup.exe` (238.5 MB) | `e6ce05e57d57d03c815b11c519a2746e74ec0d963b9cb6862ac7fe79a0bf0d36` |
| macOS 13 or later, Apple silicon | 0.1.6 beta | `titan-atlas-free_0.1.6_macos-arm64.dmg` (46.7 MB) | `fe041d09a2a3a0abcae948e40d42b54deaac0ff364d4740368ca204573828e25` |
| Ubuntu 24.04 or later, amd64 | 0.1.5 beta | `titan-atlas-free_0.1.5_amd64.deb` (12.7 MB) | `5981edb72da17f57691680ef844e8465f482915b0e290ede098fd0b03c8bd714` |

**[Download from the latest release →](https://github.com/WeAreTitans/atlas-free/releases/latest)**

The same files are published at [titanatlas.world/downloads](https://titanatlas.world/downloads/). Both places serve byte-identical installers.

## Install

**Windows:** run the installer. It installs for your Windows user and includes Microsoft's WebView2 runtime. The installer is not signed yet, so Windows SmartScreen may warn: check its checksum before you run it.

**macOS:** open the disk image and drag **Titan.Atlas Free** to Applications. The disk image and the app are signed with Developer ID and notarized by Apple.

**Ubuntu:**

```bash
sudo apt install ./titan-atlas-free_0.1.5_amd64.deb
```

The Ubuntu package is not signed. Check its checksum before you install it.

## Verify what you downloaded

Download `SHA256SUMS` from the same release and run this in the folder that holds the installer.

On Windows (PowerShell):

```powershell
Get-FileHash .\titan-atlas-free_0.1.6_windows-x64-setup.exe -Algorithm SHA256
```

Compare the result with the Windows line in `SHA256SUMS`.

On macOS:

```bash
shasum -a 256 -c SHA256SUMS --ignore-missing
```

On Ubuntu:

```bash
sha256sum -c SHA256SUMS --ignore-missing
```

On macOS you can also ask Gatekeeper directly. It should report `source=Notarized Developer ID`.

```bash
spctl -a -vvv -t open --context context:primary-signature titan-atlas-free_0.1.6_macos-arm64.dmg
```

## What is in this beta

- **Windows 0.1.6** is the first Windows beta, for Windows 10 and 11, 64-bit. It includes Gmail read and send through your own Google account, with the same test-user limit as macOS, and a Mail screen that uses the whole window.
- **macOS 0.1.6** adds Gmail read and send through your own Google account. Google's app verification is still pending, so Connect Gmail works only for listed test users.
- **Ubuntu 0.1.5** has no mail. Mailbox connection and Gmail setup are not in that build, and the stop switch is not included. It adds a Manage local modules panel: Clocks and Weather can start without pairing a House, one at a time and only when you choose.
- **All three** are local betas for one person, with the Home and Life experiences.

Atlas Free is a beta under active development. Its independent release acceptance is still open. The release notes say what each build does and does not include, and the [Atlas Upgrades board](https://titanatlas.world/atlas/upgrades/) keeps the full engineering record.

## Feedback and bugs

[Open an issue](https://github.com/WeAreTitans/atlas-free/issues/new/choose) using the beta feedback form. **Do not paste emails, passwords, tokens, account names or anything else personal into an issue.** Issues here are public.

Report security problems privately, as described in [SECURITY.md](SECURITY.md).

## Terms

Atlas Free is free to download and use. Use is governed by the [Titan.Atlas Terms](https://titanatlas.world/terms/) and the [Privacy notice](https://titanatlas.world/privacy/). Atlas Free is not open-source software, and this repository grants no licence to its source code.

TITAN.ATLAS is operated by SynOct LLC. Contact: atlas@titanatlas.live · [titanatlas.world](https://titanatlas.world/)
