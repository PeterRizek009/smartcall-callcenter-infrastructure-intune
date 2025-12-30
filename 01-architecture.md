# Architecture

## Identity Layer (Microsoft Entra ID)
- Users created with Department & JobTitle (bulk CSV)
- Dynamic User Groups:
  - CallCenter-Users (department = Call Center)
  - NonCallCenter-Users (department != Call Center)

## Device Provisioning (Windows Autopilot)
- Devices registered via Hardware Hash
- Group Tag used to classify devices before enrollment:
  - Group Tag = Callcenter  -> Call Center Self-Deploying profile
  - Group Tag = Admin       -> Admin User-Driven profile

## Endpoint Management (Intune)
- Device-based policies for shared devices
- User-based assignments for user-targeted apps and MAM

## Security & Access Control
- Endpoint Security Baseline + BitLocker
- Compliance policy checks required settings
- Conditional Access blocks access unless compliant + MFA

## Data Protection (MAM)
- App protection policies for Outlook/Teams on BYOD/mobile
- Selective wipe for corporate data

## Operations
- Offboarding: Retire (BYOD) vs Wipe (Corporate)
- Lost device: Wipe + cleanup
- Monitoring: compliance + app install status + security reports
