# Moor for Android

Moor's leveraged funds on Solana, as a native Android app: connect your mobile wallet, get test USDC, mint and
redeem 2×/3× long and −1×/−2× short fund shares, follow your portfolio, get phone alerts when a trade lands or a fund
you hold rebalances, and share a position card.

> **Part of Moor** — leveraged funds on Solana.
> The protocol's home is moor-program (private). To learn more, use the web app at [app.moor.fund](https://app.moor.fund)
> or read the [whitepaper](https://github.com/moor-protocol/whitepaper).

> **Devnet only.** Moor runs on Solana devnet with test tokens. Nothing here uses real money.

## Where it fits

This repository only hosts the app's releases: signed APKs you can download and install. The app's source is not
public. It is the mobile counterpart of the web app at [app.moor.fund](https://app.moor.fund) and trades the same
funds on devnet.

## Download

**[⬇ Download the latest APK](https://github.com/moor-protocol/moor-android/releases/latest/download/moor.apk)**

Every version and its notes: [Releases](https://github.com/moor-protocol/moor-android/releases).

## Install

1. Open the download link on your Android phone (Android 7 or newer, 64-bit).
2. When Android asks, allow your browser to install apps, then tap **Install**.
3. Install a Solana wallet such as **Solflare** (or Phantom) and switch it to **devnet**.
4. Open Moor, tap **Connect wallet**, sign the free sign-in message, and tap **Get test tokens**.

Updates install over the previous version and keep your connection.

## Verify the download

Every APK is signed with the Moor key. Android refuses an update signed by any other key. You can also check it
yourself (Android SDK build-tools):

```bash
apksigner verify --print-certs moor.apk
# Signer #1 certificate SHA-256 digest:
# d067b1a37eca7dd126f9f638f3073ba20fbba4d01e6658f6f15d8e277d6a5a00
```

Each release lists its APK's SHA-256 checksum.

## Package

The same APKs are published as a public package: `ghcr.io/moor-protocol/moor-android` (one tag per version).

## About

- Web app: [app.moor.fund](https://app.moor.fund)
- Whitepaper: [moor-protocol/whitepaper](https://github.com/moor-protocol/whitepaper)
- This repository only hosts releases; the app's source is not public.
- The app bundles `@moor-protocol/sdk`, licensed under BUSL-1.1.
