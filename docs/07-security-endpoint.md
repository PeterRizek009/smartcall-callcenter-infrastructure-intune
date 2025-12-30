# Endpoint Security

## Security Baselines
Intune -> Endpoint security -> Security baselines
- Apply Windows security baseline
Assign to:
- CallCenter devices
- Admin devices

## BitLocker
Intune -> Endpoint security -> Disk encryption
- Require BitLocker on Windows devices
- Store recovery keys in Entra ID
Assign to device groups

## Microsoft Defender + Firewall
- Enabled via baseline and/or endpoint security policies
- Consider Attack Surface Reduction (ASR) rules (documented in /security)
