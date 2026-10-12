# Moor for Android

> **Summary:** Trade Moor's leveraged funds on Solana from your Android phone.

[![Latest release](https://img.shields.io/github/v/release/moor-protocol/moor-android)](https://github.com/moor-protocol/moor-android/releases/latest)
[![Solana: Devnet](https://img.shields.io/badge/Solana-Devnet-blue)](https://explorer.solana.com/?cluster=devnet)
[![Android 7+](https://img.shields.io/badge/Android-7%2B-3DDC84)](#3-install)

---

## 1. Overview

With Moor you can mint and redeem fund shares that keep a fixed leverage: 2× and 3× long, or −1× and −2× short. The
app trades the same funds as the web app at [app.moor.fund](https://app.moor.fund), sends phone alerts for your trades
and for rebalances, and makes position cards you can share.

> **Devnet only.** The app uses test tokens; nothing here uses real money.

This repository hosts the signed APK releases. The app's source is in
[moor-mobile](https://github.com/moor-protocol/moor-mobile).

| Repository | Role | Description |
| :--- | :--- | :--- |
| [`moor-program`](https://github.com/moor-protocol/moor-program) | **Protocol Hub** | Anchor program, math libraries, TypeScript SDK and protocol docs |
| [`moor-mobile`](https://github.com/moor-protocol/moor-mobile) | **Mobile App** | Native Android app (Expo / React Native) |
| [`moor-frontend`](https://github.com/moor-protocol/moor-frontend) | **Web App** | Trading app ([app.moor.fund](https://app.moor.fund)) and landing page ([moor.fund](https://moor.fund)) |
| [`whitepaper`](https://github.com/moor-protocol/whitepaper) | **Whitepaper** | Formal spec, math and proofs |

## 2. Download

**[⬇ Download the latest APK](https://github.com/moor-protocol/moor-android/releases/latest/download/moor.apk)**

All versions and release notes are on the [Releases](https://github.com/moor-protocol/moor-android/releases) page.

## 3. Install

1. Open the download link on your Android phone (Android 7 or newer, 64-bit).
2. Allow your browser to install apps when asked, then tap **Install**.
3. Set up a Solana wallet. On a Solana Seeker phone, the built-in Seed Vault wallet works. On other phones, install
   **Solflare** (or Phantom) and switch it to **devnet**.
4. Open Moor, tap **Connect wallet**, sign the free sign-in message, and tap **Get test tokens**.

Updates install over the previous version and keep your connection.

## 4. Verify the download

Every APK is signed with the Moor key, and Android refuses an update signed by any other key. To check the signature
yourself (needs the Android SDK build-tools):

```bash
apksigner verify --print-certs moor.apk
# Signer #1 certificate SHA-256 digest:
# d067b1a37eca7dd126f9f638f3073ba20fbba4d01e6658f6f15d8e277d6a5a00
```

Each release also lists its APK's SHA-256 checksum.

## 5. Package

The same APKs are published as the public package `ghcr.io/moor-protocol/moor-android`, with one tag per version.

## 6. License

The app bundles `@moor-protocol/sdk`, licensed under BUSL-1.1.
