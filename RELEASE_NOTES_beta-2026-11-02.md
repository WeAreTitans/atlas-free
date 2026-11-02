The current public beta installers of TITAN.ATLAS Free. They are byte-identical to the ones at [titanatlas.world/downloads](https://titanatlas.world/downloads/).

| Installer | Platform | SHA-256 |
| :--- | :--- | :--- |
| `titan-atlas-free_0.1.6_macos-arm64.dmg` | macOS 13 or later, Apple silicon | `fe041d09a2a3a0abcae948e40d42b54deaac0ff364d4740368ca204573828e25` |
| `titan-atlas-free_0.1.5_amd64.deb` | Ubuntu 24.04 or later, amd64 | `5981edb72da17f57691680ef844e8465f482915b0e290ede098fd0b03c8bd714` |

### macOS 0.1.6 beta
- New: Gmail read and send through your own Google account. Google's app verification is pending, so Connect Gmail works only for listed test users.
- The disk image and the app are signed with Developer ID and notarized by Apple.
- To install, open the disk image and drag Titan.Atlas Free to Applications.

### Ubuntu 0.1.5 beta
- This is the build published on 27 October 2026 at 10:46 UTC. Atlas now opens Home, not "Find your House", while a House pairing is still unfinished.
- The package is not signed. Check the checksum before you install it.
- It has no mail: mailbox connection and Gmail setup are not in this build, and the stop switch is not included.
- Manage local modules: Clocks and Weather can start without pairing a House, one at a time and only when you choose.
- To install, run `sudo apt install ./titan-atlas-free_0.1.5_amd64.deb`.

### Both
- Local betas for one person, with the Home and Life experiences and the Clocks and Weather local modules.
- This is a beta. Independent release acceptance is still open, and Windows is not released.

### Check your download
Run `shasum -a 256 -c SHA256SUMS --ignore-missing` on macOS, or `sha256sum -c SHA256SUMS --ignore-missing` on Ubuntu.

Full engineering record: [Atlas Upgrades board](https://titanatlas.world/atlas/upgrades/). Feedback goes in the [issue tracker](https://github.com/WeAreTitans/atlas-free/issues/new/choose); keep anything personal out of it.
