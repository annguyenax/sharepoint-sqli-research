# SharePoint SQL Injection Research

Analysis of SQL injection vulnerabilities affecting Microsoft SharePoint Server on-premises deployments — covering vulnerability mechanics, exploitation patterns, threat actor behavior, and enterprise detection and remediation.

---

## Reports

| Report | CVE | Severity | Published |
|---|---|---|---|
| [Critical SQL Injection in SharePoint Web Part Configuration Service](reports/CVE-202X-XXXXX-SharePoint-SQLi.md) | CVE-202X-XXXXX | CRITICAL (CVSS 9.8) | 2024-11-15 |

---

## Scope

This research covers:

- **Root cause analysis** — unsafe string concatenation in `ConfigurationService.dll`, absence of parameterized queries
- **Exploitation chain** — pre-authentication UNION-based injection through OS command execution via `xp_cmdshell`
- **Threat actor behavior** — historical exploitation patterns, post-exploitation tooling (web shells, C2 frameworks)
- **MITRE ATT&CK mapping** — T1190 through T1041 across the full kill chain
- **Detection engineering** — IIS log analysis, Splunk SPL queries, WAF signature development
- **Remediation** — tiered patching guidance, SQL Server hardening, network segmentation

---

## Frameworks & Standards

![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red?style=flat-square)
![CVSS](https://img.shields.io/badge/CVSS-v3.1-orange?style=flat-square)
![TLP](https://img.shields.io/badge/TLP-WHITE-white?style=flat-square&labelColor=black)
![OWASP](https://img.shields.io/badge/OWASP-Top%2010-blue?style=flat-square)
![CWE](https://img.shields.io/badge/CWE-89-lightgrey?style=flat-square)

---

## Disclaimer

> CVE identifiers marked `CVE-202X-XXXXX` are fictional placeholders. No working exploit code is published here. Research follows responsible disclosure principles and is intended for defensive security purposes.
