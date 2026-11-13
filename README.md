# Handsy 1.0.6 — unsigned iPhone build

Based on [ESP32 iPhone Agent](https://github.com/onehumanbeing/esp32-iphone-agent) by Henry Yuan.

This repository builds the unmodified public iOS source at commit `39aa23e17de957bc01529fbd8f22f4deef0e08ca` (tag `v1.0.6`) with a standard GitHub-hosted macOS runner.

The resulting unsigned IPA, SHA-256 checksum, original MIT license and NOTICE, and source/build information appear under **Releases** after a successful build.

## Installation

Download `Handsy-ESP32-Agent-1.0.6-original-unsigned.ipa` and sign it with your own iOS signing tool and profile. It contains a physical-device arm64 app and its Live Activity extension.

The public source reports version 1.0.6, build 1. The upstream tag describes official TestFlight build 16; this source build is not claimed to reproduce the official TestFlight binary.

Configure your own model after installation. The author's private/free model service and signing certificates are not included. Device operation, App Groups, Live Activity, and automatic Wi-Fi joining depend on the signing profile and require device verification.

## Build

The workflow runs on changes to its own file on main or by manual dispatch. It is restricted to public repositories, uses standard `macos-26`, has a 20-minute limit, and does not use Actions artifact or cache storage. Only the public-source app and provenance files are published.

Public demos, videos and posts should credit Henry Yuan and the original project.
