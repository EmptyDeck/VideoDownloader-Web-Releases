# Video Downloader Web for macOS

**Mac only · macOS 13 or later · public beta, not notarized.**

[Download the Mac app](https://github.com/EmptyDeck/VideoDownloader-Web-Releases/releases/download/v0.8.3-public-beta.1/VideoDownloader-Web-0.8.3-macOS-Universal-Public-Beta.dmg) · [All release files and checksums](https://github.com/EmptyDeck/VideoDownloader-Web-Releases/releases/tag/v0.8.3-public-beta.1) · [Privacy policy](https://emptydeck.github.io/VideoDownloader-Web-Releases/privacy.html)

## Install and use

1. Download the DMG, open it, and copy **Video Downloader Web.app** to Applications.
2. Open the app. This beta has an ad-hoc integrity signature and has not been notarized by Apple. If macOS cannot verify the developer, and you trust the official download, first try opening it, then use **System Settings → Privacy & Security → Open Anyway** for this app. See [Apple’s instructions](https://support.apple.com/en-us/102445). Do not disable system-wide security. If macOS reports malware or a damaged download, stop and check the file/checksum instead.
3. Leave the app running and choose a language once. The local connection starts automatically.
4. While Chrome Web Store review is pending, open `chrome://extensions`, enable **Developer mode**, choose **Load unpacked**, and select `~/Library/Application Support/VideoDownloaderWeb/ChromeExtension`. The app creates that folder when it runs. The separate Chrome ZIP is an alternative.
5. Open a permitted video page and click the extension. Download a selected format, or click a heart to save its link to the Mac library. [Try the sample clip](https://emptydeck.github.io/VideoDownloader-Web-Releases/demo.html).

In the Mac library, Space previews and double click plays. Incognito needs **Allow in Incognito**; hearts intentionally remain in the Mac library after private windows close. Downloaded files remain until you delete them.

## App Lock in 0.8.3

Set an optional password in **Settings → App Lock**. Use **⇧⌘L** to lock now. Opening a new app session, closing all windows, hiding the app, or locking/sleeping the Mac locks the interface again. Downloads continue while locked. Change/disable needs the current password; recovery uses macOS owner authentication and keeps the library and files.

Only a salted password verifier is kept in the Mac Keychain. This is an interface lock, not encryption of library/download files or authentication of the existing extension connection. There is no separate menu bar icon; reopen the library from the Dock.

## What is public

This repository provides installers, public product information and sample media. The original Swift and Go application source remains private. Third-party notices and applicable source archives are bundled in `Contents/Resources/ThirdParty`.

## Beta limits

The local download, audio/video merge and native startup checks passed. A separate recipient Mac and physical Intel hardware have not been tested. Managed Macs may restrict opening an unnotarized beta. Site permissions, DRM, deleted media and expired links can prevent downloads. Chrome Web Store availability depends on Google’s review; until approval, use the manual extension setup above.

Mac 전용 공개 베타입니다. macOS 13 이상이 필요하며 Apple 공증 전이므로 첫 실행 때 공식 다운로드를 신뢰하는 사용자의 직접 허용이 필요할 수 있습니다. 크롬 웹스토어 심사 전에는 위 경로의 확장을 수동으로 설치해 사용할 수 있습니다. 원본 Swift·Go 코드는 비공개로 유지합니다.

Contact: [imsejikpark@gmail.com](mailto:imsejikpark@gmail.com)
