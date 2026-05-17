# Mobile APK Static Analysis using MobSF

## Project Overview

This project demonstrates the process of performing static security analysis on an Android APK using MobSF (Mobile Security Framework).

The objective of this lab is to:

* Perform Android APK static analysis
* Analyze AndroidManifest configurations
* Identify dangerous permissions
* Detect insecure network configurations
* Map vulnerabilities to OWASP MASVS
* Generate a professional security report

---

# Project Structure

```text
lab-6/
│
├── README.md
└── images/
    ├── 1.png
    ├── 2.png
    ├── 3.png
    ├── 4.png
    ├── 5.png
    ├── 6.png
    ├── 7.png
    ├── 8.png
    ├── 9.png
    ├── 10.png
    ├── 11.png
    ├── 12.png
    ├── 13.png
    ├── 14.png
    ├── 15.png
    ├── 16.png
    ├── 17.png
    ├── 18.png
    ├── 19.png
    ├── 20.png
    └── 21.png
```

---

# Step 1 — Preparing the Workspace

The first step consisted of creating a dedicated working directory and moving the APK file into the analysis environment.

![Step 1](images/1.png)

This screenshot shows:

* Creation of the analysis folder
* Navigation into the workspace
* Moving the APK file
* Verification of the APK using terminal commands

---

# Step 2 — Starting MobSF

MobSF was launched successfully inside the analysis environment.

![Step 2](images/2.png)

The terminal displays:

* MobSF initialization
* Gunicorn startup
* Environment information
* Framework version details

---

# Step 3 — MobSF Web Dashboard

The MobSF dashboard became accessible through the web browser.

![Step 3](images/3.png)

The interface allows:

* APK upload
* Static analysis
* Dynamic analysis
* Access to previous scans

---

# Step 4 — APK Upload Interface

The APK file can be uploaded directly into MobSF.

![Step 4](images/4.png)

The interface supports:

* Drag and drop upload
* APK scanning
* Analysis automation

---

# Step 5 — Static Analysis Overview

MobSF generated a complete overview of the analyzed application.

![Step 5](images/5.png)

The analysis includes:

* File information
* Application metadata
* Security score
* Package details
* SDK versions

---

# Step 6 — Manifest Analysis

The AndroidManifest.xml file was analyzed for insecure configurations.

![Step 6](images/6.png)

The report identified:

* Cleartext traffic enabled
* Backup configuration enabled
* Exported services
* Exported activities

---

# Step 7 — Permission Analysis

The Android permissions requested by the application were inspected.

![Step 7](images/7.png)

The analysis revealed:

* Dangerous permissions
* Access to sensitive resources
* Potential overprivileged behavior

---

# Step 8 — Advanced Manifest Findings

MobSF identified additional manifest-related vulnerabilities.

![Step 8](images/8.png)

The findings include:

* Exported activities
* Unprotected services
* Insecure intent filters

---

# Step 9 — Binary Security Analysis

The binary security protections of the application were inspected.

![Step 9](images/9.png)

The binary analysis verified:

* NX protection
* PIE support
* Stack canary usage
* Symbol stripping
* Binary encryption

---

# Step 10 — Security Findings Summary

MobSF generated a global summary of detected vulnerabilities.

![Step 10](images/10.png)

The report displays:

* High severity vulnerabilities
* Warning-level issues
* Informational findings
* Security score distribution

---

# Step 11 — Manifest Security Findings

The manifest security configuration was analyzed in detail.

![Step 11](images/11.png)

The report highlights:

* Android version weaknesses
* Backup exposure risks
* App link verification issues
* Exported activities

---

# Step 12 — Network Security Analysis

The network security configuration was inspected.

![Step 12](images/12.png)

The analysis detected:

* Cleartext traffic allowed
* Weak TLS configurations
* Insecure network scopes

---

# Step 13 — Additional Manifest Configuration Review

Another review of the manifest security configuration was performed.

![Step 13](images/13.png)

This analysis confirmed:

* Insecure transport configurations
* Network security configuration usage
* Security warnings related to communication

---

# Step 14 — MobSF Analysis on macOS

MobSF was also accessed from a macOS environment.

![Step 14](images/14.png)

This screenshot demonstrates:

* MobSF web interface
* Static analyzer dashboard
* Manifest analysis section

---

# Step 15 — OWASP MASVS Documentation

The vulnerabilities were correlated with OWASP MASVS requirements.

![Step 15](images/15.png)

The MASVS framework provides:

* Mobile security verification standards
* Security domains
* Best practices for Android security

---

# Step 16 — MASVS Requirement Mapping

Specific MASVS controls were reviewed.

![Step 16](images/16.png)

The screenshot presents:

* Storage security requirements
* Verification mappings
* Security testing references

---

# Step 17 — Detailed Security Findings

MobSF displayed a detailed vulnerability report.

![Step 17](images/17.png)

The report includes:

* High-risk vulnerabilities
* Warning-level findings
* Exported component risks
* Cleartext traffic issues

---

# Step 18 — Security Scorecard

The overall application security score was generated.

![Step 18](images/18.png)

The scorecard summarizes:

* Security score
* Risk level
* Severity distribution
* Privacy risk
* Findings categories

---

# Step 19 — Signing Certificate Analysis

The APK signing certificate was analyzed.

![Step 19](images/19.png)

The report detected:

* Debug certificate usage
* Weak SHA1 signature algorithm
* Signed application information

---

# Step 20 — Vulnerability Dashboard

An additional vulnerability management dashboard was reviewed.

![Step 20](images/20.png)

The dashboard visualizes:

* Vulnerability severity distribution
* Device exposure statistics
* Vulnerability trends
* Risk metrics

---

# Step 21 — Compliance Report

A compliance report was generated to verify security controls.

![Step 21](images/21.png)

The report contains:

* Passed controls
* Failed controls
* Audit rules
* Compliance results

---

# Main Vulnerabilities Identified

The analysis revealed multiple security weaknesses:

* Cleartext traffic enabled
* Exported Android components
* Dangerous permissions
* Backup exposure
* Weak signing certificate
* Insecure network communication
* Debug configurations enabled

---

# Recommendations

1. Disable cleartext traffic and enforce HTTPS.
2. Remove debug configurations before production release.
3. Restrict exported components.
4. Reduce unnecessary dangerous permissions.
5. Use strong signing certificates.
6. Disable application backups for sensitive applications.
7. Apply OWASP MASVS security recommendations.

---

# Conclusion

This lab demonstrated how MobSF can be used to perform Android static application security analysis.

The analysis process helped identify:

* Manifest vulnerabilities
* Dangerous permissions
* Weak network configurations
* Insecure binary protections
* Exported Android components

The use of OWASP MASVS improved the understanding of mobile application security standards and vulnerability management.
