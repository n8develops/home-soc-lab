# Home SOC Lab (Splunk)

Hands-on SOC environment to practice ingestion → detection → response using:
- Splunk on Ubuntu
- Windows endpoint (Win10/Server) with Sysmon/Winlogbeat
- Linux endpoint (Ubuntu) shipping auth logs
- Kali attacker box for simulations

## Why this repo
- End-to-end: build, ingest, detect, respond
- Resume-ready evidence: screenshots, detections, dashboards, playbooks
- Reproducible configs and docs

## Architecture (VirtualBox)
Internal network `lab-net`:
- Splunk: `192.168.56.10`
- Windows: `192.168.56.11`
- Linux: `192.168.56.12`
- Kali: `192.168.56.13`

## Quick Start
1) Read `docs/01-architecture.md`
2) Build VMs (Host-only or Internal Network) → `docs/02-virtualbox-setup.md`
3) Configure data inputs → `docs/03-splunk-setup.md`
4) Ship logs from endpoints → `docs/04-endpoints-config.md`
5) Run attack playbooks → `playbooks/` and validate detections → `detections/`

## Detections
See `detections/savedsearches/` for SPL and descriptions in `docs/05-attacks-and-detections.md`.

## Screenshots
Put triage screenshots in `docs/` (alerts → investigation → containment).

## License
MIT (see LICENSE).
