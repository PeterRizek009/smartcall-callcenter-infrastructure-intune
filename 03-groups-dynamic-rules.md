# Groups & Dynamic Rules

## User Groups (Dynamic)
### Call Center Users
Rule:
(user.department -eq "Call Center")

### Non-Call Center Users
Rule:
(user.department -ne "Call Center")

## Device Groups (Dynamic) – Autopilot Group Tags
### Call Center Autopilot Devices
Rule:
(device.devicePhysicalIDs -any (_ -contains "[ZTDId]:Callcenter"))

### Admin Autopilot Devices
Rule:
(device.devicePhysicalIDs -any (_ -contains "[ZTDId]:Admin"))

## Why Group Tags?
- Works BEFORE device enrollment
- Allows different Autopilot profiles (Self-Deploying vs User-Driven)
- Minimizes manual device assignment
