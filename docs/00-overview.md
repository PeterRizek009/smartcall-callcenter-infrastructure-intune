# Overview

This project simulates a complete endpoint and identity deployment for a call center company.

High-level flow:
1) Create users (bulk CSV) with department/jobTitle
2) Create dynamic user groups (Call Center vs Others)
3) Register devices in Autopilot (Hardware Hash + Group Tag)
4) Create Autopilot profiles:
   - Self-Deploying for Call Center shared devices
   - User-Driven for Admin devices
5) Deploy apps and configuration policies
6) Apply endpoint security baseline + BitLocker
7) Define compliance policies
8) Enforce access with Conditional Access:
   - Require MFA
   - Require compliant device
   - Block legacy authentication
9) Implement App Protection (MAM) for mobile/BYOD
10) Operate lifecycle:
   - employee exit
   - device lost
   - device reassignment

   - Require compliant device
   - Block legacy authentication
9) Implement App Protection (MAM) for mobile/BYOD
10) Operate lifecycle:
   - employee exit
   - device lost
   - device reassignment
