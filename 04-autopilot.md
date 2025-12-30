# Windows Autopilot

## Register Devices
Option A) Vendor registers devices (recommended in enterprise)
Option B) Manual hardware hash collection and import

## Import hardware hash
Intune -> Devices -> Windows -> Windows enrollment -> Windows Autopilot devices -> Import

## Group Tag
Set Group Tag during import:
- Callcenter -> Call Center shared devices
- Admin     -> Admin/user devices

## Profiles
1) Self-Deploying (Call Center shared)
2) User-Driven (Admin laptops)

Assign profiles to the matching dynamic device groups.
