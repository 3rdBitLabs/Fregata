# Security Policy

Fregata is a network video recorder. It handles camera credentials, RTSP streams, recordings, and runs on machines that are often part of a home or small-business network. We take security reports seriously.

## Reporting a vulnerability

**Do not file a public GitHub issue for security bugs.** Public disclosure before a fix is available puts other Fregata users at risk.

Please report vulnerabilities through:

1. **GitHub private security advisory**:
   [Open a draft advisory](https://github.com/3rdBitLabs/Fregata/security/advisories/new)

We will acknowledge receipt within 3 business days and aim to provide an initial assessment within 7 days.

## What to include

A useful report contains:

- A clear description of the issue and its impact.
- Affected Fregata version(s) and macOS version.
- Steps to reproduce, or a proof of concept.
- Any logs, network captures, or screenshots that help us reproduce.
- Whether you've shared this with anyone else.

## Scope

In scope:

- The signed Fregata `.app` bundle (process supervisor, native CoreML detector, macOS runtime, menu bar app).
- Fregata's local web UI and HTTP API as exposed by the bundled app.
- Fregata's handling of camera credentials, stored recordings, and configuration files on disk.
- Fregata-specific CoreML / VideoToolbox / ANE integration code.

Out of scope (please report upstream):

- Bugs in the upstream open-source [Frigate](https://github.com/blakeblackshear/frigate) Python core that are not Fregata-specific. Report those at the Frigate project.
- General macOS, FFmpeg, or third-party library vulnerabilities not introduced by Fregata.
- Issues that require physical access to an unlocked Mac.
- Social engineering, phishing, or attacks against Fregata users outside the app itself.

## Disclosure policy

- We follow coordinated disclosure. We'll work with you on a timeline to fix and release before public disclosure.
- Once a fix ships, we'll credit reporters in the release notes unless you'd prefer to remain anonymous.
- We do not currently run a paid bug bounty program.

## Hardening tips for users

A few defaults worth keeping in mind, regardless of Fregata bugs:

- Put cameras on an isolated VLAN or guest network when possible. Cameras themselves are frequently the weakest link.
- Use unique, strong passwords for each camera. Rotate the defaults.
- Don't expose Fregata's web UI to the public internet. Use a VPN or Tailscale-style tunnel for remote access.
- Keep macOS and Fregata updated. Security fixes ship in updates.
