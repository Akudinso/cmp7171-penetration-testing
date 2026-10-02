# CMP7171 Advanced Ethical Hacking Assessment Part 2
## Penetration Testing Report: Network Infrastructure Security Assessment

---

## Executive Summary

This repository contains the complete penetration testing engagement report and supporting evidence from a comprehensive security assessment of a multi-host network infrastructure (DC31_01, DC31_02, DC31_03). The engagement identified and exploited three distinct vulnerability classes, demonstrating a complete exploitation chain from initial reconnaissance through post-exploitation and privilege escalation.

### Key Findings Overview

| Host | IP Address | Service | Vulnerability | OWASP Classification | Impact | Status |
|------|------------|---------|----------------|----------------------|--------|--------|
| **DC31_01** | 10.75.134.90 | Gitea v1.4.0 | Unprotected Installation (CVE-2020-14144) | A05: Security Misconfiguration | Remote Code Execution (RCE) as git user | ✅ Exploited |
| **DC31_02** | 10.75.134.92 | Redis v5.0.7 | Missing Authentication + Module Loading | A01: Broken Access Control | RCE as root via module injection | ✅ Exploited |
| **DC31_03** | 10.75.134.94 | Openfire v4.7.4 | Default Credentials + Path Traversal (CVE-2023-32315) | A07: Auth Failures | RCE as root via plugin upload | ✅ Exploited |

---

## 📂 Repository Structure