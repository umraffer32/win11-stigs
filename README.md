# Windows 11 STIG Remediation Project

Remediation of 10 failing audits from a DISA Microsoft Windows 11 STIG (v2r6) compliance scan run against a Windows 11 Pro VM using Tenable Nessus.

Each fix was applied via PowerShell, verified locally, and confirmed with a Nessus re-scan before being marked complete.

## Environment
- **OS:** Windows 11 Pro (VM)
- **Scanner:** Tenable Nessus — DISA Microsoft Windows 11 STIG v2r6 audit file
- **Tools used:** PowerShell, `auditpol.exe`, `secedit.exe`, `net accounts`

## Documentation Format
Each STIG writeup answers:
1. **What is the STIG ID?** — the finding and why it matters
2. **How we are fixing it** — registry / command details + PowerShell script
3. **Scan results verifying remediation** — Nessus PASS screenshot

## Table of Contents

| # | STIG ID | Description | Writeup |
|---|---|---|---|
| 1 | WN11-CC-000038 | WDigest Authentication must be disabled | [Link](STIG-1-WN11-CC-000038.md) |
| 2 | WN11-CC-000050 | Hardened UNC Paths must be defined | [Link](STIG-2-WN11-CC-000050.md) |
| 3 | WN11-CC-000066 | Command line data must be included in process creation events | [Link](STIG-3-WN11-CC-000066.md) |
| 4 | WN11-CC-000326 | PowerShell script block logging must be enabled | [Link](STIG-4-WN11-CC-000326.md) |
| 5 | WN11-SO-000167 | Remote SAM calls must be restricted to Administrators | [Link](STIG-5-WN11-SO-000167.md) |
| 6 | WN11-SO-000190 | Kerberos encryption types must prevent DES and RC4 | [Link](STIG-6-WN11-SO-000190.md) |
| 7 | WN11-SO-000215 | Minimum NTLM SSP client session security must be enforced | [Link](STIG-7-WN11-SO-000215.md) |
| 8 | WN11-AU-000050 | Audit Detailed Tracking — Process Creation successes | [Link](STIG-8-WN11-AU-000050.md) |
| 9 | WN11-AC-000035 | Passwords must be at least 14 characters | [Link](STIG-9-WN11-AC-000035.md) |
| 10 | WN11-UR-000030 | "Back up files and directories" right restricted to Administrators | [Link](STIG-10-WN11-UR-000030.md) |

## Original Scan Report
The initial Nessus compliance scan PDF: [`stig_win11__the-dude__hkpfq6.pdf`](stig_win11__the-dude__hkpfq6.pdf)
