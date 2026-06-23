# SharePoint SQL Injection Research

Portfolio threat intelligence project analyzing a fictional critical SQL injection vulnerability affecting on-premises Microsoft SharePoint Server deployments. The project is written as a CVE-focused intelligence product for enterprise security leadership, vulnerability management, and SOC teams.

---

## Reports

| Report | CVE | Severity | Published |
|---|---|---|---|
| [Critical SQL Injection in Microsoft SharePoint Server](reports/CVE-202X-XXXXX-SharePoint-SQLi.md) | CVE-202X-XXXXX | Critical, CVSS 9.8 | 2024-11-15 |

---

## Scope

This research covers:

- **Executive risk framing**: business impact, affected environments, and leadership action required
- **Root cause analysis**: unsafe SQL query construction and missing parameterized database access
- **Attack path modeling**: pre-authentication network exploitation, database access, and conditional post-exploitation paths
- **Threat actor context**: likely exploitation patterns based on historical targeting of enterprise collaboration platforms
- **MITRE ATT&CK mapping**: initial access, collection, exfiltration, persistence, and impact techniques
- **Detection engineering**: IIS, WAF, SQL Server, EDR, and network telemetry opportunities
- **Remediation planning**: prioritized patching, compensating controls, hardening, and post-patch validation

---

## Frameworks and Standards

![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red?style=flat-square)
![CVSS](https://img.shields.io/badge/CVSS-v3.1-orange?style=flat-square)
![TLP](https://img.shields.io/badge/TLP-CLEAR-white?style=flat-square&labelColor=black)
![OWASP](https://img.shields.io/badge/OWASP-Top%2010-blue?style=flat-square)
![CWE](https://img.shields.io/badge/CWE-89-lightgrey?style=flat-square)

---

## Disclaimer

> CVE identifiers marked `CVE-202X-XXXXX` are fictional placeholders. This project does not publish working exploit code. The report is intended to demonstrate defensive CVE analysis, enterprise risk communication, detection logic, and remediation planning.
