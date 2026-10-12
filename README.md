# Moor for Android

> The official Android release for Moor: trade autonomous leveraged funds on Solana with zero margin calls and continuous Net Asset Value (NAV) pricing.

[![Latest Release](https://img.shields.io/github/v/release/moor-protocol/moor-android)](https://github.com/moor-protocol/moor-android/releases/latest)
[![Solana: Devnet](https://img.shields.io/badge/Solana-Devnet-blue)](https://explorer.solana.com/?cluster=devnet)
[![Platform: Android 7+](https://img.shields.io/badge/Android-7%2B-3DDC84)](#2-installation--setup)

---

## 1. Overview

Moor for Android brings fixed-leverage DeFi funds (2× / 3× Long, −1× / −2× Short) directly to mobile. The app connects to Solana via Mobile Wallet Adapter, lets users mint and redeem fund shares at NAV, tracks portfolio performance, and delivers background notifications for rebalance events and band alerts.

> **Environment:** Deployed on **Solana Devnet** using test tokens.

### Key Protocol Repositories

| Repository | Role | Description |
| :--- | :--- | :--- |
| [`moor-program`](https://github.com/moor-protocol/moor-program) | **Protocol Hub** | Core Anchor contracts, math libraries, and TypeScript SDK |
| [`moor-mobile`](https://github.com/moor-protocol/moor-mobile) | **App Source** | React Native / Expo source code for this Android app |
| [`moor-frontend`](https://github.com/moor-protocol/moor-frontend) | **Web Interface** | Trading app ([app.moor.fund](https://app.moor.fund)) and landing page |
| [`whitepaper`](https://github.com/moor-protocol/whitepaper) | **Specification** | Mathematical formulations, NAV invariance proofs, and sizing |

---

## 2. Download & Installation

### Step 1: Download the APK
Direct download for the latest verified release:

📥 **[Download Latest Release (moor.apk)](https://github.com/moor-protocol/moor-android/releases/latest/download/moor.apk)**

*All historical releases and release notes are available on the [Releases](https://github.com/moor-protocol/moor-android/releases) page.*

### Step 2: Install on Device
1. Open the downloaded `.apk` file on your Android device (Android 7.0 or higher required).
2. If prompted, allow installations from your browser or file manager.
3. Tap **Install**. Future releases install directly over existing versions while preserving local app data.

### Step 3: Wallet Configuration (Devnet)
- **Solana Seeker:** Connects seamlessly through the built-in default Seed Vault wallet.
- **Other Android Devices:** Install **Solflare** or **Phantom**, navigate to Developer Settings, and switch the network to **Devnet**.
- **Devnet Test Tokens:** Once connected, tap **Get test tokens** to receive an initial allocation of mock USDC and devnet SOL.

---

## 3. Cryptographic Verification

All release APKs are signed with Moor's official release key. To verify package authenticity and integrity using Android SDK build tools:

```bash
apksigner verify --print-certs moor.apk
```

**Expected Signer Certificate Fingerprint (SHA-256):**
```text
d067b1a37eca7dd126f9f638f3073ba20fbba4d01e6658f6f15d8e277d6a5a00
```

Each GitHub release also provides the direct SHA-256 checksum of the committed APK.

---

## 4. Package Distribution

APKs are mirrored as container packages on GitHub Container Registry:
```text
ghcr.io/moor-protocol/moor-android:<version>
```
