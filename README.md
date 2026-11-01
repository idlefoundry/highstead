# Highstead

Highstead (model CA-74) is Idle Foundry’s circuit model of the Oberheim SEM: two oscillators with sync and pulse-width modulation, a state-variable filter with LP/notch/HP and band-pass, two envelopes, an LFO and a VCA. It includes MONO/POLY/UNISON, stereo placement, DRIVE with AUTO GAIN, 28 factory presets, MIDI Learn and MPE controls in Settings.

## Download 0.1.0

Get the installers and checksums from the [Highstead 0.1.0 release](https://github.com/idlefoundry/highstead/releases/tag/v0.1.0).

| Computer | Download |
|---|---|
| macOS 11 or later, Apple silicon or Intel | `Highstead-0.1.0-macOS.pkg` |
| Windows 10 or 11, 64-bit | `Highstead-0.1.0-Windows-setup.exe` |
| Windows, manual installation | `Highstead-0.1.0-Windows-x86_64.zip` |
| Linux x86-64, Ubuntu 22.04 or equivalent or later | `Highstead-0.1.0-Linux-x86_64.tar.gz` |

The Mac installer is signed and notarized. The Windows installer is unsigned; Windows may show SmartScreen’s “Windows protected your PC” warning. The manual Windows ZIP is available if you prefer not to use an installer.

## Install and play

Close your DAW before installing, then restart it or rescan plug-ins. Choose **Highstead** by **Idle Foundry** as an instrument. VST3 and CLAP are included on all three systems, with Audio Unit on macOS. Each installer also includes the standalone application.

On Linux, unpack the archive and run `./install.sh`. The Windows ZIP includes a README with the manual installation paths. On macOS, launch `Highstead.app` from Applications; on Windows, use the Idle Foundry → Highstead Start menu entry.

In the standalone, choose your audio and MIDI devices in Settings. Begin with a factory preset. LO is the lighter model; HI and ULTRA use the circuit model. When band-pass is selected, NOTCH dims because the band-pass path bypasses it; FREQUENCY and RESONANCE still shape the band.

## Source and checksums

`SHA256SUMS.txt` lists the release assets. The release includes `Highstead-0.1.0-source.tar.gz` (the corresponding Highstead source and documentation), `Highstead-0.1.0-git-sources.tar.gz` (pinned Git dependency sources), and `THIRD-PARTY-NOTICES.txt`. The illustrated quick start is inside the source archive at `docs/quick-start.md`.

Highstead is free software under **GPL-3.0-or-later**. Copyright © 2026 Idle Foundry Ltd. This repository hosts public downloads; the implementation repository is maintained separately.

## Feedback and current limits

Please include your OS, DAW/version, plug-in format, quality mode and steps to reproduce when reporting an issue here. Oscillator aliasing residuals remain at extreme pitch/pulse settings, and downstream behavior under extreme DRIVE/high-frequency input is still being characterized; 0.1.0 does not claim zero aliasing at every setting.
