The current public beta installers of TITAN.ATLAS Free, now including Windows. They are byte-identical to the ones at [titanatlas.world/downloads](https://titanatlas.world/downloads/).

| Installer | Platform | SHA-256 |
| :--- | :--- | :--- |
| `titan-atlas-free_0.1.6_windows-x64-setup.exe` | Windows 10 or 11, 64-bit | `e6ce05e57d57d03c815b11c519a2746e74ec0d963b9cb6862ac7fe79a0bf0d36` |
| `titan-atlas-free_0.1.6_macos-arm64.dmg` | macOS 13 or later, Apple silicon | `fe041d09a2a3a0abcae948e40d42b54deaac0ff364d4740368ca204573828e25` |
| `titan-atlas-free_0.1.5_amd64.deb` | Ubuntu 24.04 or later, amd64 | `5981edb72da17f57691680ef844e8465f482915b0e290ede098fd0b03c8bd714` |

### Windows 0.1.6 beta (new)
- The first Windows beta of Atlas Free, for Windows 10 and 11, 64-bit. It installs for your Windows user and includes Microsoft's WebView2 runtime.
- Gmail read and send through your own Google account. Google's app verification is pending, so Connect Gmail works only for listed test users.
- A Mail screen that uses the whole window, with larger list text and the reading pane beside the list.
- The installer is not signed yet, so Windows SmartScreen may warn. Check the checksum before you run it.

### macOS 0.1.6 and Ubuntu 0.1.5
Unchanged from [beta-2026-11-02](https://github.com/WeAreTitans/atlas-free/releases/tag/beta-2026-11-02): macOS has Gmail read and send for listed test users and is signed and notarized; Ubuntu has no mail and is not signed.

### All three
- Local betas for one person, with the Home and Life experiences.
- This is a beta. Independent release acceptance is still open.

### Check your download
On Windows run `Get-FileHash .\titan-atlas-free_0.1.6_windows-x64-setup.exe -Algorithm SHA256` in PowerShell and compare with `SHA256SUMS`. On macOS run `shasum -a 256 -c SHA256SUMS --ignore-missing`, on Ubuntu `sha256sum -c SHA256SUMS --ignore-missing`.

Full engineering record: [Atlas Upgrades board](https://titanatlas.world/atlas/upgrades/). Feedback goes in the [issue tracker](https://github.com/WeAreTitans/atlas-free/issues/new/choose); keep anything personal out of it.
