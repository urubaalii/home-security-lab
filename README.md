# Home Enterprise Security Lab

This project demonstrates a hands-on vulnerability assessment performed using Nessus Essentials in a simulated home lab environment. The goal of the lab was to gain practical experience with vulnerability scanning, risk identification, and remediation analysis.

## Objective

The objective of this project was to understand how vulnerability scanning tools identify security weaknesses within a system and how those findings are analyzed using industry-standard risk scoring such as CVSS.

The lab simulates both:

- An **unauthenticated scan** (external attacker perspective)
- An **attempted authenticated scan** (internal vulnerability assessment)

## Tools Used

- Nessus Essentials
- Windows 11
- CVSS Vulnerability Scoring

## Lab Workflow

1. Configured Nessus Essentials vulnerability scanner.
2. Performed an unauthenticated vulnerability scan on a Windows host.
3. Analyzed vulnerabilities identified by the scanner.
4. Investigated severity ratings using CVSS scoring.
5. Attempted an authenticated scan using Windows credentials to simulate an internal security assessment.
6. Documented findings and remediation strategies.

## Key Findings

The scan identified several informational and medium-severity vulnerabilities including certificate trust issues and configuration weaknesses. These findings demonstrate how vulnerability scanners detect exposed services and misconfigurations that could increase system risk.

## Authenticated Scan Attempt

An authenticated scan was attempted using Windows credentials to allow Nessus deeper visibility into system configurations. The authentication attempt was unsuccessful, which highlights a common challenge in real-world vulnerability management where credential permissions, firewall rules, or system services may prevent successful authentication.

## Lessons Learned

This project demonstrated the difference between unauthenticated and authenticated vulnerability scans.

- Unauthenticated scans identify vulnerabilities visible from an external perspective.
- Authenticated scans allow deeper system inspection but require proper credential configuration and system permissions.
- Vulnerability management requires both accurate scanning and proper system configuration to be effective.

## Repository Structure
home-security-lab
│
├─ vulnerability-assessment
│ ├─ report.md
│ └─ screenshots
│ ├─ unauthenticated-scan-results.png
│ ├─ ssl-certificate-vulnerability.png
│ ├─ authenticated-scan-running.png
│ └─ authenticated-scan-failed.png

## Future Improvements

- Configure successful authenticated scanning
- Expand lab to include SIEM log monitoring
- Perform vulnerability remediation testing
