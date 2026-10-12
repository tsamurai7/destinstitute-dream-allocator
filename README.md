# dest.institute Dream Allocator

A device that records your dreams into video. Allegedly.

**Dream Allocator** is the first device from **Dest Institute**, a merchandise-first production company. Record your dreams on video, clock in on-chain, and your dream gets a number: one of **1111 Dream Drops**, a limited series. 

Users buy a physical device based on a PAY WHAT YOU WANT structure, from 1 to 100 euros, which will allocate from 1 to 1000 tokens, respectively. The number users hold is their voice in creative decisions - a bottom-up platform for onchain cinematic brands, where each project grows from podcast to game engine to film or series, validated by the audience before the money arrives.

## What this prototype does today

- Runs on a real Android phone with a real Solana wallet (Mobile Wallet Adapter)
- Connect wallet, tap **Clock In**, approve the transaction - your dream is assigned a tier number
- Every clock-in is a **signed on-chain transaction** (Solana **devnet**), with the transaction signature shown in-app and verifiable on Solscan

This is an honest prototype: numbers are per-device rehearsal numbers on devnet. It does not yet mint tokens, record video, or run on mainnet.

## Stack

- Kotlin + Jetpack Compose
- Solana Mobile Wallet Adapter (MWA)
- Solana **devnet**

## Build

Open in Android Studio, then `Build &gt; Generate App Bundles or APKs &gt; Generate APKs`, or:

```
./gradlew assembleDebug
```

The debug APK lands in `app/build/outputs/apk/debug/app-debug.apk`, and a ready APK is attached to this repo's Releases.

## Roadmap

- Video capture inside the app (the dream recording itself)
- Mainnet deployment
- The other 1110 drops

---

Built for the Solana Mobile **Clock In** hackathon, October 2026.
