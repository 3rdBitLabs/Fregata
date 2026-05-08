<p align="center">
  <a href="https://fregata.app">
    <img src="https://fregata.app/assets/fregata-icon.png" alt="Fregata" width="128" height="128" />
  </a>
</p>

<h1 align="center">Fregata</h1>

<p align="center">
  <strong>Native NVR for Apple Silicon.</strong><br/>
  Your cameras. Your Mac. No cloud.
</p>

<p align="center">
  <a href="https://fregata.app">Website</a> ·
  <a href="https://docs.fregata.app">Documentation</a> ·
  <a href="https://fregata.app/#download">Download</a> ·
  <a href="https://github.com/3rdBitLabs/Fregata/discussions">Discussions</a>
</p>

<p align="center">
  <img alt="Platform" src="https://img.shields.io/badge/platform-macOS%2013%2B-000?style=flat-square&logo=apple&logoColor=white" />
  <img alt="Architecture" src="https://img.shields.io/badge/arch-Apple%20Silicon-000?style=flat-square" />
  <a href="https://github.com/3rdBitLabs/Fregata/discussions"><img alt="Discussions" src="https://img.shields.io/github/discussions/3rdBitLabs/Fregata?style=flat-square" /></a>
  <a href="https://github.com/3rdBitLabs/Fregata/issues"><img alt="Issues" src="https://img.shields.io/github/issues/3rdBitLabs/Fregata?style=flat-square" /></a>
</p>

---

## What is Fregata?

Fregata is a private, local-first network video recorder for macOS, built on the open-source [Frigate NVR](https://frigate.video) engine. Object detection runs on the Apple Neural Engine, video decode and encode go through VideoToolbox, and the whole thing ships as a single signed `.app` - drag to Applications, done.

No Docker. No VMs. No terminal setup. No cloud.

## Highlights

- **Apple Silicon native** - built for M-series Macs. Detection on the Apple Neural Engine.
- **Hardware accelerated video** - H.264 / H.265 decode and encode through VideoToolbox.
- **Local-first** - recordings, video, and detections never leave your Mac. No Fregata account.
- **One app** - signed, notarized `.app` bundle. Drag, launch, configure in your browser.
- **Built on Frigate** - the same detection pipeline thousands already trust, repackaged for Apple Silicon.

## Requirements

- macOS 13 (Ventura) or later
- Apple Silicon (M1 or newer)

## Get Fregata

[**Download the latest release**](https://releases.fregata.app/Fregata-latest.dmg)

---

## About this repository

This is the **community repository** for Fregata.

### Where to do what

| Need | Go here |
|---|---|
| Report a bug | [Open an issue](https://github.com/3rdBitLabs/Fregata/issues/new/choose) |
| Request a feature | [Open an issue](https://github.com/3rdBitLabs/Fregata/issues/new/choose) |
| Ask for help, share tips, chat | [Discussions](https://github.com/3rdBitLabs/Fregata/discussions) |
| Submit a community benchmark | [Discussions](https://github.com/3rdBitLabs/Fregata/discussions) - *Benchmarks* category |
| Read the docs | [docs.fregata.app](https://docs.fregata.app) |
| Press, media, or review coverage | [Press kit](press-kit/) |

### Filing a useful bug report

A few things help us reproduce quickly:

- Fregata version - menu bar → **About Fregata**
- macOS version and chip - e.g. *macOS 14.5 on M2 Pro*
- What you were doing when it happened
- Logs from **Open Logs Folder** in the menu bar, if relevant
- Steps to reproduce, if you have them

### Sharing a community benchmark

If you've stress-tested Fregata on your hardware, post your numbers in the [Benchmarks discussion category](https://github.com/3rdBitLabs/Fregata/discussions). Helpful details:

- Mac model and chip (e.g. *M1 Mac mini, 16 GB*)
- Camera count, resolution, FPS, codec
- Detector settings (model, input size, FPS)
- CPU / GPU / ANE load and thermal behavior over time

The more apples-to-apples your setup, the more useful your post is for the next person sizing their hardware.

---

## Built on Frigate

Fregata is a native-macOS port of the open-source [Frigate NVR](https://frigate.video) by [Blake Blackshear](https://github.com/blakeblackshear) and contributors. The Frigate Python core stays open source. Fregata's macOS runtime, Apple Silicon optimizations, native CoreML detector, process supervisor, and the Fregata brand are proprietary.

If you don't need the Apple Silicon work or the `.app` bundle, you can run [Frigate](https://github.com/blakeblackshear/frigate) directly with Docker - it's an excellent project and we owe it everything.

---

<p align="center">
  <a href="https://fregata.app">fregata.app</a> ·
  <a href="https://docs.fregata.app">docs</a> ·
  <a href="https://github.com/3rdBitLabs/Fregata/discussions">discuss</a> ·
  <a href="https://github.com/3rdBitLabs/Fregata/issues">issues</a>
</p>
