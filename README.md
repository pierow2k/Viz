<!-- markdownlint-disable no-inline-html -->
# Viz

## About this fork

This is a community-maintained fork of
[alienator88/Viz](https://github.com/alienator88/Viz).

The upstream project is currently [on indefinite hold](https://github.com/alienator88/Viz#project-status-on-hold)
for feature development, pull-request reviews, and new releases. This fork
exists to keep Viz usable on current versions of macOS and to address small
bugs as they are encountered.

### Differences from upstream

- **Original signing configuration removed.** The upstream project references
  signing certificates and provisioning profiles belonging to the original
  developer. Those settings have been removed so the application can be built
  and signed locally without access to the original developer account.

- **iCloud support removed.** Viz's iCloud entitlements were tied to the
  original developer's Apple account and cannot be used by independent builds.
  This fork therefore does not provide iCloud history synchronization.

- **macOS 27 compatibility.** Button icons that disappeared on macOS 27 have
  been restored by updating the way SF Symbols are rendered.

The goal is otherwise to remain close to upstream behavior. Changes are kept
as focused commits so they can be reviewed or adopted by the original project
if development resumes.

This fork is not affiliated with or maintained by the original Viz author.

---

<p align="center">
  <img src="https://github.com/alienator88/Viz/assets/6263626/46db3bc2-e5ac-48e6-af45-4affe6aeb55c" width="128" height="128" alt="logo"/>
   <br />
   <strong>Status: </strong>Community maintained
   <br />
   <strong>Version: </strong>2.3.3
   <br />
   <a href="https://github.com/pierow2k/viz/releases"><strong>Download</strong></a>
    · 
   <a href="https://github.com/pierow2k/viz/commits">Commits</a>
   <br />
   <br />
</p>
</br>

Extract text from images, videos, QR codes, barcodes and colors with a simple snip mechanism.

## Features

- Very quick extraction process (Can set fidelity between fast and accurate as per the Apple Vision framework)
- Can extract text based on all languages or select your language in settings for quicker/accurate captures
- Copies to clipboard automatically, ready to paste
- Post-processing option to execute shell commands when capture is taken. Can use the captured text via `[ocr]` token within the shell commands
- Customizable hotkeys for the main app functions
- Shows copied text in a floating window, which can be set to auto-hide as well after a custom wait period
- Enable or disable line breaks in the extracted text
- Append multiple text snippets to the clipboard by enabling Append option in Settings, otherwise it only holds one snippet at a time
- Saves captures in History and persists app restarts
- Also saves History to iCloud Drive if enabled
- Launch at login option
- Custom auto-updater that pulls latest release notes and binaries from GitHub Releases

## Preview

![Screenshot 2025-03-28 at 4 01 31 PM](https://github.com/user-attachments/assets/fdf8c000-b892-4632-8404-b985931f418f)

### Text Extraction Demo

https://github.com/user-attachments/assets/409044dd-3765-48df-9017-0f6376ed11f8

### QR/Barcode Extraction Demo

https://github.com/user-attachments/assets/c75c9b47-9724-4b5a-ab51-363e8249fabb

### Color Picker Demo

https://github.com/user-attachments/assets/bacbf405-d2e4-496c-b79e-fde000361962

### History View

![history](https://github.com/user-attachments/assets/66c7c6f7-60e0-49fd-8050-0741e829aa6f)

## Requirements

- MacOS 13.0+ (App uses some newer SwiftUI functions/modifiers which don't work on anything lower than 13.0)

<!-- ## Getting Viz

<details>
  <summary>Releases</summary>

Pre-compiled, always up-to-date versions are available from my [releases](https://github.com/pierow2k/viz/releases) page.
</details>

<details>
  <summary>Homebrew</summary>

You can add the app via Homebrew:
```
brew install viz
```
</details> -->

## License

> [!IMPORTANT]
> Viz is licensed under Apache 2.0 with [Commons Clause](https://commonsclause.com/). This means that you can do anything you'd like with the source, modify it, contribute to it, etc., but the license explicitly prohibits any form of monetization for Viz or any modified versions of it. See full license [HERE](https://github.com/alienator88/Sentinel/blob/main/LICENSE.md)

## Some of alienator88's other apps

[Pearcleaner](https://github.com/alienator88/Pearcleaner) - An opensource app cleaner with privacy in mind

[Sentinel](https://github.com/alienator88/Sentinel) - A GUI for controlling gatekeeper status on your mac

<!-- [Viz](https://github.com/alienator88/Viz) - Utility for extracting text from images, videos, qr/barcodes -->

[PearHID](https://github.com/alienator88/PearHID) - Remap your macOS keyboard with a simple SwiftUI frontend
