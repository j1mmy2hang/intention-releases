# Intention — releases

This repository exists so that [Intention](https://github.com/j1mmy2hang) can update itself. It
holds two kinds of file and nothing else:

- **`appcast.xml`** — the feed Sparkle reads to learn what the current version is.
- **`Intention-X.Y.Z.zip`** — the signed builds it downloads.

There is no source code here. It is public only because Sparkle has to fetch the feed without
credentials, and a private repository's release assets require authentication.

Every build is signed twice: with an Apple Developer ID certificate and notarised by Apple, and
again with an EdDSA key whose public half is compiled into the app. Intention refuses to install
anything the second signature doesn't verify — so even someone who could replace a file here could
not make an existing copy of Intention accept it.

Both files are written by `scripts/ship.sh` in the (private) source repository. Nothing here is
edited by hand.
