# homeauto

![License: AGPL v3](https://img.shields.io/badge/Code-AGPL_v3-blue.svg)
[![License: CERN OHL-S v2](https://img.shields.io/badge/Hardware-CERN_OHL_S_v2-red.svg)](hardware/LICENSE)

Open source, full-stack home automation — from hardware to the application layer.

**Mission:** give users control of their data and their homes, without the security-ownership and privacy risks of big tech. Everything runs locally; external access is VPN-only.

## Repository Layout

| Folder | Contents |
|---|---|
| `hardware/` | KiCad hardware design files (CERN-OHL-S-2.0) |
| `docs/` | Project documentation, incl. the [CONOPS](docs/CONOPS.md) |

(Firmware, software, and infrastructure folders will be added as the project grows.)

## Concept of Operations

The overarching system design lives in [docs/CONOPS.md](docs/CONOPS.md): a "house as a supercharged LAN" — easy, secure device onboarding, local-first automation, no cloud dependency, and a two-tier UX (sane defaults for everyone, raw control for power users).

## License

- **Code:** AGPL-3.0-or-later — see . © 2026 DJ Fracking, see .
- **Hardware designs:** CERN-OHL-S-2.0 — see [hardware/LICENSE](hardware/LICENSE).

## Contributing

Contributions are welcome and licensed under AGPL-3.0-or-later (code) / CERN-OHL-S-2.0 (hardware), with copyright retained by contributors.

## Contact

Open an issue at [github.com/djfracking/homeauto](https://github.com/djfracking/homeauto).
