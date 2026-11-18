# Brisk

Brisk is a lightweight RSS reader for macOS.

This repository is used for distribution only. It contains no source code. Installers (DMG) are published under [Releases](https://github.com/linus-ground/brisk/releases), and the website and update feed are served from [GitHub Pages](https://linus-ground.github.io/brisk/).

## Requirements

- A Mac with Apple silicon (M1 or later)
- macOS 14 Sonoma or later

Intel-based Macs are not supported.

## Installation

1. Download `Brisk-x.y.z.dmg` from the [latest release](https://github.com/linus-ground/brisk/releases/latest).
2. Open the disk image and drag Brisk into the Applications folder.
3. Launch Brisk from the Applications folder.

## Updates

Brisk checks for updates once a day using [Sparkle](https://sparkle-project.org). When a new version is available, Brisk shows a prompt; choosing **Install Update** downloads, verifies, and installs it, then relaunches the app. To check manually, choose **업데이트 확인…** (Check for Updates) from the Brisk menu or the menu bar icon. Automatic checks can be turned off in Settings.

Subscriptions, read status, and settings are preserved across updates.

## Widgets

Brisk provides two desktop widgets.

| Widget | Sizes | Shows |
|--------|-------|-------|
| **Unread Count** (안 읽은 글 수) | Small | The number of unread articles in all feeds or in a chosen folder or feed |
| **Recent Articles** (최근 글) | Medium, Large | The latest articles. Click an article to open it in Brisk. |

To add a widget:

1. Open Brisk at least once so that the widget has data to show.
2. Right-click the desktop and choose **Edit Widgets**.
3. Search for **Brisk** and drag a widget onto the desktop or into Notification Center.

To configure a widget, right-click it and choose **Edit Widget**:

- **Scope**: all feeds, Unread, Starred, or a specific folder or feed
- **Unread Only**: show only unread articles (on by default)

Text inside the widget follows the language selected in Brisk. The widget names and descriptions in the widget gallery follow the macOS system language.

## License

Brisk is distributed under the [PolyForm Noncommercial License 1.0.0](LICENSE.md). It may be used and shared freely for noncommercial purposes, such as personal use, study, research, and use by noncommercial organizations. Commercial use is not permitted.

Third-party components and their licenses are listed in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

## Repository contents

| Path | Description |
|------|-------------|
| `docs/index.html` | Website (GitHub Pages) |
| `docs/appcast.xml` | Update feed read by the app. Each release is signed with an EdDSA key, and the app installs only updates whose signature matches. |
| `LICENSE.md` | License |
| `THIRD-PARTY-NOTICES.md` | Third-party notices |
