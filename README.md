# SmartCall Call Center Infrastructure (Microsoft Entra ID + Intune + Autopilot) – Portfolio Project

This repository documents a real-world enterprise-style deployment for a call center company using:
- Microsoft Entra ID (Identity)
- Microsoft Intune (Endpoint management)
- Windows Autopilot (Zero-touch provisioning)
- Endpoint Security (Baseline, Defender, BitLocker)
- Compliance + Conditional Access (Access control)
- MAM App Protection (Data protection inside apps)
- Operations (Offboarding, lost device, troubleshooting)

## Scenario
Company: SmartCall LLC (fictional)
Users: 120
- 80 Call Center agents (shared devices)
- 40 Admin departments (IT / HR / Quality / Finance / Operations)

Devices:
- Windows 11 corporate-owned
- Optional BYOD mobile for Outlook/Teams

Goals:
1) Zero-touch deployment for Call Center shared devices (Self-Deploying Autopilot)
2) User-driven Autopilot for Admin laptops
3) Standardized apps deployment
4) Security hardening (Defender, Firewall, BitLocker)
5) Compliance-based access control via Conditional Access
6) Data protection using App Protection (MAM)
7) Clear lifecycle procedures (Retire/Wipe/Delete)

## Key Design Decisions
- Use Autopilot Group Tags to classify devices BEFORE enrollment.
- Use Dynamic Groups (User + Device) to avoid manual membership updates.
- Use Compliance Policy + Conditional Access to block risky/non-compliant access.
- Use MAM to protect corporate data on BYOD/mobile.

## Evidence
- Implementation steps: `docs/`
- Policies and rules: `/autopilot`, `/security`, `/compliance`, `/conditional-access`, `/mam`
- Screenshots: `docs/screenshots/` (sanitized, no secrets)

## Disclaimer
This is a portfolio lab. Do NOT store real passwords, tenant IDs, secrets, or customer data in this repo.
