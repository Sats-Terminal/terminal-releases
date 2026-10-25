# Terminal for Mac

Downloads of the Terminal Mac app, an AI-native trading terminal for Hyperliquid.
The source code is private; this repository holds the releases only.

**[Download the latest release](https://github.com/Sats-Terminal/terminal-releases/releases/latest)**

Requires macOS on Apple silicon (M1 or later).

## Installing an unsigned beta

Beta builds are not yet signed by Apple, so macOS blocks them the first time:

1. Open the `.dmg` and drag **Terminal** into **Applications**.
2. Open Terminal from Applications. macOS says it cannot verify the app; click **Done**.
3. Open **System Settings → Privacy & Security**, scroll down, and click **Open Anyway** next to Terminal.

If macOS instead says the app "is damaged", run this once in the Terminal app (Utilities), then open it again:

```
xattr -dr com.apple.quarantine /Applications/Terminal.app
```

Check the download against the `.sha256` file published with each release:

```
shasum -a 256 -c Terminal_<version>_aarch64.dmg.sha256
```
