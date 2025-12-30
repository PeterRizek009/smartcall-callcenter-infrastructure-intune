# Microsoft Entra ID (Identity Setup)

## Create Users
- Entra ID -> Users -> Bulk create
- Use CSV templates in `/data/`

## Set Usage Location
- usageLocation = AE (United Arab Emirates)
- Required for license assignment

## Licensing (example)
- Assign Microsoft 365 (Business Premium / E5 etc.) depending on lab
- Validate service plans: Intune + Entra ID P1 features if needed

## Recommended Security
- Enable MFA (via Conditional Access)
- Block legacy authentication (via CA)
- Least privilege for admins
