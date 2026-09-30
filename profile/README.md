<div align="center">

# Code Pause, Inc.

### Secure, real-time infrastructure for healthcare, live media, and the open web

*What happens outside the visit belongs inside the record.*

[![Website](https://img.shields.io/badge/codepause.com-1F2937?style=for-the-badge)](https://codepause.com)
[![OutsideINsights](https://img.shields.io/badge/OutsideINsights-0E7C86?style=for-the-badge)](https://outsideinsights.health)
[![Voxi.Live](https://img.shields.io/badge/Voxi.Live-173BFF?style=for-the-badge)](https://voxi.live)
[![QuackXide](https://img.shields.io/badge/QuackXide-open_source-4B5563?style=for-the-badge)](https://github.com/Code-Pause-Inc/QuackXide)
[![Press](https://img.shields.io/badge/Press-Newsroom-B45309?style=for-the-badge)](https://codepause.com/press/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/codepause)

</div>

---

## Latest news

**September 30, 2026 — [QuackXide v0.1.0: open-source secure data processing](https://github.com/Code-Pause-Inc/QuackXide/releases/tag/v0.1.0)**

Code Pause, Inc. has released **[QuackXide](https://github.com/Code-Pause-Inc/QuackXide)** as open source under the MIT and Apache-2.0 licenses. QuackXide is a secure database and data-processing system for sensitive and protected data: it is encrypted on the way in, at rest, and on the way out; plaintext exists only in attested enclave memory; and every query passes a disclosure gate that returns aggregates, never rows. *Data goes in. Analysis comes out. The dataset doesn't.*

Development continues with the **USF core contribution team** from the University of San Francisco: Jake Abendroth, William Shenker, Angelina Tam, and Gabriel Zubovsky. Release binaries carry signed build provenance, verifiable with `gh attestation verify`.

**September 8, 2026 — [Code Pause, Inc. Advances Real-Time Communications with Voxi.live and Telehealth over QUIC](https://codepause.com/press/voxi-live-telehealth-over-quic/)**

A live, browser-based Voxi.Live avatar session measured approximately **93 ms** of edge-clock-calibrated capture-to-render video latency over Media over QUIC. The same communications foundation is being applied to **Telehealth over QUIC (ToQ)**, the healthcare initiative for OutsideINsights, where live conversation and multiplexed medical telemetry share one secure, encrypted channel.

| Metric | Value |
| --- | --- |
| Capture-to-render latency | ≈93 ms |
| Frame rate / codec | ≈30 fps, VP8 over MOQT draft 16 |
| Video payload | ≈1.42 Mbps |
| Decoder rejections / backlog | 0 / 0 |

Also published on [voxi.live](https://voxi.live/press/voxi-live-telehealth-over-quic) and [outsideinsights.health](https://outsideinsights.health/press/voxi-live-telehealth-over-quic). All releases: [codepause.com/press](https://codepause.com/press/).

---

## What we build

Code Pause, Inc. develops advanced communications, software, and data technologies. We own the secure rails for care between visits and the products that run on them, and we apply the same real-time foundation to live media on the open web.

| | Product | What it is |
| --- | --- | --- |
| <img src="https://api.iconify.design/lucide/stethoscope.svg?color=%236b7280" width="48" height="48" alt="Health"> | **[OutsideINsights](https://outsideinsights.health)** | Contextual remote patient monitoring and telehealth. Connected-device data and caregiver observations delivered into the EHR care teams already use: Epic, Oracle Health, and athenahealth. |
| <img src="https://api.iconify.design/lucide/mic.svg?color=%236b7280" width="48" height="48" alt="Live audio"> | **[Voxi.Live](https://voxi.live)** | Browser-based live communications and entertainment platform built on Media over QUIC, with real-time avatars, voice processing, and interactive audience features. *Be live. Be anything.* |
| <img src="https://api.iconify.design/lucide/radio-tower.svg?color=%236b7280" width="48" height="48" alt="Telehealth"> | **Telehealth over QUIC (ToQ)** | Real-time telehealth over Media over QUIC: live visits, multiplexed medical telemetry, adaptive resolution from low-bandwidth audio to HD video, and post-quantum end-to-end encryption. |
| <img src="https://api.iconify.design/lucide/satellite.svg?color=%236b7280" width="48" height="48" alt="Edge gateway"> | **OUTsights Gateway** | Tri-band connected edge hardware (Wi-Fi, cellular, satellite failover) with delay-tolerant networking for homes and field sites beyond ordinary coverage. |
| <img src="https://api.iconify.design/lucide/database.svg?color=%236b7280" width="48" height="48" alt="Secure data"> | **[QuackXide](https://github.com/Code-Pause-Inc/QuackXide)** | Open-source secure database and data-processing system for sensitive and protected data. Client-side encryption, HPKE-encrypted storage, analytics inside attested enclaves, and a disclosure gate so results leave as aggregates, never rows. MIT or Apache-2.0. |
| <img src="https://api.iconify.design/lucide/shield-check.svg?color=%236b7280" width="48" height="48" alt="Secure transport"> | **Century Service Protocol** | The secure, multi-tenant transport and storage foundation beneath everything: database-enforced tenant isolation, append-only audit ledger, and encrypted PHI at rest, in flight, and at ingest. |

**In development:** TREK watcher (consumer-direct off-grid health monitoring) · MarineINsights (maritime crew health and safety).

---

## How we build

- **Rust where the trust boundaries live.** Gateways, relays, media pipelines, and the WebAssembly browser player.
- **TypeScript where the people do.** React 19 frontends, Bun and Hono services, Drizzle and PostgreSQL.
- **Standards first.** Media over QUIC, WebTransport, WHIP, LL-HLS, FHIR, DTN and Bundle Protocol v7 through the [Pale Blue Systems Foundation](https://github.com/Pale-Blue-Systems).
- **Security past today's requirements.** Hybrid X25519 + ML-KEM post-quantum key exchange, hardware-attested confidential computing, HIPAA-grade architecture by construction.
- **Edge-native delivery.** Cloudflare Workers and the Cloudflare MoQ relay network, Google Cloud Run, and satellite-backed ingestion.
- **Disciplined agentic engineering.** Strict roadmaps, local validation gates, and a human in the loop on every shipped system.

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![WebAssembly](https://img.shields.io/badge/WebAssembly-654FF0?style=flat-square&logo=webassembly&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black)
![Bun](https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white)
![Hono](https://img.shields.io/badge/Hono-E36002?style=flat-square&logo=hono&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white)

---

## Why it matters

- Over 70% of patients use connected health devices, yet only about 6% of providers see that data in their workflow. OutsideINsights closes that gap without a new login or a new dashboard.
- Devices show *what* changed; the people around the patient explain *why*. The Care Circle Protocol gives families a structured, HIPAA-compliant path into the record.
- Real-time communication is more valuable when the technology carries the full experience without interrupting the conversation. Voxi.Live proves the foundation; ToQ brings it to care.

---

## Leadership

**Jeremy L. D. Ryan** — Founder & CEO · [@AxolDad](https://github.com/AxolDad)

Twenty-five years as an EMT and crisis responder, an active 988 crisis-line volunteer, and a Rust and TypeScript systems engineer. Creator of OutsideINsights, Voxi.Live, and the Pale Blue Systems open standards for delay-tolerant space communication.

---

## Connect

| | |
| --- | --- |
| Company | [codepause.com](https://codepause.com) · [Mission](https://codepause.com/mission/) · [Ecosystem](https://codepause.com/ecosystem/) · [R&D](https://codepause.com/rd/) |
| Investors | [codepause.com/investors](https://codepause.com/investors/) |
| Press | [codepause.com/press](https://codepause.com/press/) · [Jeremy.Ryan@Codepause.com](mailto:Jeremy.Ryan@Codepause.com) |
| General | [info@codepause.com](mailto:info@codepause.com) · +1-202-459-9156 |
| Security | [codepause.com/security](https://codepause.com/security/) · [security.txt](https://codepause.com/.well-known/security.txt) |
| Machine readers | [llms.txt](https://codepause.com/llms.txt) · [llms-full.txt](https://codepause.com/llms-full.txt) |

<div align="center">

**Code Pause, Inc.** · Long Island, N.Y.

© 2026 Code Pause, Inc. All rights reserved. OutsideINsights and Voxi.Live are products of Code Pause, Inc.

</div>
