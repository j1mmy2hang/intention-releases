# Intention for Mac

**Know what you are doing, whenever you are on your Mac.**

Too often we open a laptop without a clear purpose and end up horsing around for hours. Intention
asks one question before that happens, and keeps honest time on the answer.

A Mac should be the *tool* for work, not the *space* for it.

[**intention-for-mac.app**](https://intention-for-mac.app) · [**Download**](../../releases/latest)

---

## What it does

- **Asks what you intend to do** — at login, on waking, and whenever a session ends.
- **Times the answer**, whether that's work or horsing around. Both are honest answers; only one of
  them should quietly become three hours.
- **Counts only the time you are actually there.** Sleep, lock, walking away — none of it accrues.
- **Checks back in** while you're horsing around, on an interval you choose.
- **Never locks you out.** ⌃⌥⌘B dismisses any prompt. It's a gatekeeper with a quiet voice.

The dashboard — your day drawn as it really went — is the one paid feature, a one-time €9.99.
Everything else is free.

Requires macOS 26 or later. Signed and notarised, so it opens without warnings, and it updates
itself from here.

Early days: the version numbers start with `0.` for a reason. Things may still move.

## About this repository

It holds the release feed and the builds — no source code. It's public because Intention updates
itself through [Sparkle](https://sparkle-project.org), which fetches `appcast.xml` without
credentials.

Every build is signed twice over: with an Apple Developer ID certificate and notarised by Apple,
and again with an EdDSA key whose public half is compiled into the app. Intention refuses to install
anything that second signature doesn't verify — so even someone able to replace a file here could
not make an installed copy accept it.

Found a bug, or something feels wrong? [Open an issue](../../issues).
