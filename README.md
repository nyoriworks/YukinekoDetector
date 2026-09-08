# YukinekoDetector

YukinekoDetector is an on-device AI image detector for iPhone, iPad, and Mac. It adds a Safari Web Extension and Share extensions that estimate whether an image is AI-generated or non-AI-like.

> A detector score is an estimate, not proof of an image's origin. Use it as one signal alongside source, context, and other evidence.

## Features

- **On-device inference** — image analysis uses Core ML and Apple Neural Engine where available.
- **Safari badges** — optionally scan visible page images and display `AI-likely` or `Non-AI-likely` badges.
- **Manual inspection** — inspect images from the Safari context menu or the extension popup.
- **Share extensions** — share an image or supported web link to YukinekoDetector from iOS and macOS.
- **Video-aware scanning** — when Auto-Scan is enabled, playing video is rechecked at a measured interval rather than continuously.
- **Encrypted model bundles** — the Core ML model is encrypted as part of each extension build.

## Privacy

Images are analyzed locally on the device. YukinekoDetector does not operate an analysis server, collect analytics, use advertising SDKs, or sell personal data. See [Privacy.md](Privacy.md) for the complete policy.

## Requirements

- iOS and iPadOS 15 or later
- macOS 12 or later
- Xcode with the matching platform SDKs to build from source

## Build from source

1. Open `YukinekoDetector.xcodeproj` in Xcode.
2. Select **YukinekoDetector (iOS)** or **YukinekoDetector (macOS)**.
3. Choose your signing team and run the selected scheme.
4. Enable the YukinekoDetector Safari extension in Safari settings after installing the app.

The project includes the app, Safari Web Extension, and iOS/macOS Share extensions. The Core ML model is built from `Shared (Model)/NGNetUnified.mlpackage`; its key is used at build time and is not bundled as a standalone key in the extensions.

## Repository layout

| Path | Purpose |
| --- | --- |
| `iOS (App)` / `macOS (App)` | Host applications for the Safari extension |
| `Shared (Extension)` | Safari extension UI, page scanning, and Core ML bridge |
| `iOS (Share)` / `macOS (Share)` | Native Share extensions |
| `Shared (Model)` | Core ML model source and build-time encryption key |
| `tools` | Local validation and model-encryption notes |

## Support

For bugs and feature requests, open an [issue](https://github.com/nyoriworks/YukinekoDetector/issues).

## Privacy Policy

The current policy is available in [Privacy.md](Privacy.md).
