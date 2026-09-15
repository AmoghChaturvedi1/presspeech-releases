# Presspeech for macOS

Push-to-talk dictation for Apple silicon Macs (macOS 14+). Hold **Fn**, speak, release — the words are pasted where your cursor is. Everything is transcribed on your Mac; no audio or text leaves it.

## Install (once)

1. **[Download Presspeech.zip](https://github.com/AmoghChaturvedi1/presspeech-releases/releases/latest/download/Presspeech.zip)** and unzip it.
2. Drag **Presspeech.app** into your **Applications** folder and open it from there.
3. macOS shows *“Apple could not verify Presspeech is free of malware…”* — this is normal for an app that isn't in the App Store. Click **Done** (not Move to Trash). Then open **System Settings → Privacy & Security**, scroll to the bottom: next to *“Presspeech” was blocked to protect your Mac* click **Open Anyway**, confirm with Touch ID or your password, and click **Open**.
   The Open Anyway button only appears for about an hour after you tried to open the app — if it's missing, double-click Presspeech again and come back. Fallback, in Terminal: `xattr -d com.apple.quarantine /Applications/Presspeech.app`
4. Grant **Microphone** and **Accessibility** when asked. The first launch downloads the speech model (~450 MB).

That's it. Presspeech lives in the menu bar and updates itself — you never see the dialog again and never need to come back here.

This repository holds only the built app and its update feed.
