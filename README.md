# iOS IPA Install — Releases

Public downloads and the [Sparkle](https://sparkle-project.org) auto-update feed
for **iOS IPA Install**, a native macOS app that installs iOS `.ipa` packages onto
development devices via Apple's `cfgutil`, with automatic device detection.

## Download

**[Download the latest release →](https://github.com/jjnicolas/IOS-IPA-Install-releases/releases/latest)**

Unzip and move `IOS IPA Install.app` to `/Applications`. It's Developer ID signed and
notarized by Apple, and updates itself from here via Sparkle.

To install an IPA: right-click any `.ipa` in Finder → **Open With → iOS IPA Install**,
pick the connected device, and click **Install**. Requires Apple Configurator's
`cfgutil` (install Apple Configurator 2 from the Mac App Store).

## What's in this repo

| File | Purpose |
|------|---------|
| `appcast.xml` | The Sparkle feed (`SUFeedURL`) the app polls for updates. |
| `IOS-IPA-Install-X.Y.Z.zip` | Notarized app builds, one per version. |
| `IOS-IPA-Install-X.Y.Z.html` | Changelog embedded in the appcast for each release (when present). |

Each download in the appcast is signed with an EdDSA key; the app verifies the
signature against its embedded public key before installing.

## Source

Source code lives in **[jjnicolas/IOS_IPA_Install](https://github.com/jjnicolas/IOS_IPA_Install)**.
For issues, feedback, or feature requests,
[open an issue](https://github.com/jjnicolas/IOS_IPA_Install/issues) there.

iOS IPA Install is part of Julien Nicolas's apps & utilities — see them all at
**[apps.tnfnet.org](https://apps.tnfnet.org)**.

---

*These files are generated and pushed by `make release` in the source repo —
they aren't edited by hand.*
