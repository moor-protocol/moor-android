# Moor for Android

Moor's leveraged funds on Solana as an Android app: mint and redeem 2×/3× long and −1×/−2× short fund shares from
your mobile wallet.

> **Part of Moor** — leveraged funds on Solana.
> The protocol's home is moor-program (private). Use the web app at [app.moor.fund](https://app.moor.fund)
> or read the [whitepaper](https://github.com/moor-protocol/whitepaper).

> **Devnet only.** Test tokens; nothing here uses real money.

## Where it fits

This repository hosts only the app's signed APK releases; the source is not public. The app is the mobile
counterpart of [app.moor.fund](https://app.moor.fund) and trades the same devnet funds, with phone alerts for trades
and rebalances and shareable position cards.

## Download

**[⬇ Download the latest APK](https://github.com/moor-protocol/moor-android/releases/latest/download/moor.apk)**
· all versions and notes: [Releases](https://github.com/moor-protocol/moor-android/releases)

## Install

1. Open the download link on your Android phone (Android 7 or newer, 64-bit).
2. Allow your browser to install apps when asked, then tap **Install**.
3. Install a Solana wallet such as **Solflare** (or Phantom) and switch it to **devnet**.
4. Open Moor, tap **Connect wallet**, sign the free sign-in message, and tap **Get test tokens**.

Updates install over the previous version and keep your connection.

## Verify the download

Every APK is signed with the Moor key; Android refuses an update signed by any other key. To check it yourself
(Android SDK build-tools):

```bash
apksigner verify --print-certs moor.apk
# Signer #1 certificate SHA-256 digest:
# d067b1a37eca7dd126f9f638f3073ba20fbba4d01e6658f6f15d8e277d6a5a00
```

Each release lists its APK's SHA-256 checksum. The same APKs are also published as the public package
`ghcr.io/moor-protocol/moor-android` (one tag per version).

## About

The app bundles `@moor-protocol/sdk`, licensed under BUSL-1.1.
