# Security Posture Monitor for Microsoft 365

PowerShell-based security posture monitoring and device correlation platform for Microsoft 365 environments.

# Operational Use Cases

- Identify unmanaged or partially visible devices
- Detect Defender inactive endpoints
- Improve endpoint visibility across platforms
- Support helpdesk investigations
- Prioritize risky operational cases
- Improve Microsoft 365 security posture visibility

Correlates security and management data from:
- Microsoft Entra ID
- Microsoft Intune
- Microsoft Defender
- Trend Micro

Designed to improve:
- endpoint visibility
- BYOD detection
- compliance monitoring
- Defender operational visibility
- missing KB detection
- operational security reporting

# Sample Outputs

<img width="942" height="1337" alt="Capture d&#39;écran 2026-04-17 091045" src="https://github.com/user-attachments/assets/c9d645d7-5822-45a2-974d-eacb17f93f05" />

# Why I Built This

Modern Microsoft 365 environments often suffer from fragmented endpoint visibility across multiple management and security platforms.

This project was designed to:
- centralize device visibility
- correlate security signals
- identify unmanaged or partially visible endpoints
- improve operational reporting
- support security and helpdesk workflows

# Operational Focus

This project was designed with a practical operational mindset:
- security visibility
- endpoint monitoring
- Defender operational analysis
- helpdesk reporting
- device correlation
- compliance visibility

# Architecture

```text
+-------------------+
|   Microsoft Entra |
+-------------------+
           |
+-------------------+
|   Microsoft Intune|
+-------------------+
           |
+-------------------+
| Microsoft Defender|
+-------------------+
           |
+-------------------+
|    Trend Micro    |
+-------------------+
           |
           v
+-------------------+
| Correlation Engine|
+-------------------+
           |
           v
+-------------------+
|    Risk Engine    |
+-------------------+
           |
           v
+-------------------+
| Reports / Outputs |
+-------------------+

Outputs:
- HTML Reports
- JSON Reports
- CSV Exports
```

# Correlation Engine

The core of this project is the correlation engine.

It normalizes and matches device data across Microsoft 365 and endpoint security sources in order to identify visibility gaps, unmanaged devices, compliance issues, and Defender-related risks.

The correlation logic compares signals from:
- Microsoft Entra ID
- Microsoft Intune
- Microsoft Defender
- Trend Micro

It helps detect:
- devices visible in one source but missing from others
- potential unmanaged or BYOD endpoints
- duplicate or inconsistent device identities
- inactive Defender machines
- partially monitored endpoints
- devices requiring operational review

# Example Workflow

1. Collect device inventories
2. Normalize device identities
3. Correlate devices across platforms
4. Detect visibility gaps
5. Analyze Defender activity
6. Detect missing KBs
7. Apply risk scoring
8. Generate operational reports

# Risk Classification Logic

<img width="932" height="589" alt="Capture d&#39;écran 2026-04-17 091059" src="https://github.com/user-attachments/assets/7d850b3d-f1f4-40dc-be55-662905ef4c8c" />

The platform classifies devices based on:
- compliance status
- Defender activity
- visibility gaps
- missing KBs
- correlation signals

# Technical Challenges

- Cross-platform device identity correlation
- Duplicate hostname normalization
- Partial visibility handling
- Microsoft Defender API throttling
- Missing KB optimization
- Active vs inactive Defender classification
- Large dataset processing

# Skills Demonstrated

- PowerShell scripting
- Microsoft Graph API
- Microsoft Defender API
- JSON processing
- Security reporting
- Endpoint visibility analysis
- Risk analysis
- Security operations logic
- API troubleshooting
- Modular scripting architecture

![PowerShell](https://img.shields.io/badge/PowerShell-5.1+-blue)
![Microsoft Graph](https://img.shields.io/badge/Microsoft-Graph-blue)
![Microsoft Defender](https://img.shields.io/badge/Microsoft-Defender-green)

# Project Status

Current state:
- Core platform completed
- Defender integration operational
- Risk scoring implemented
- Reporting operational
- Demo/public version available

Current focus:
- dashboard integration
- operational reliability
- reporting improvements

# Planned Improvements

- Web dashboard integration
- Historical trend analysis
- Microsoft Sentinel integration
- Scheduled reporting
- Real-time alerting
- Multi-tenant support
---
# Demo Mode

A public demo mode is available using anonymized sample datasets.

The demo mode simulates:
- Entra ID devices
- Intune devices
- Defender signals
- Trend Micro visibility
- Risk scoring
- HTML reporting

## Important Security Note

This repository does not publish:

credentials
secrets
customer data
production identifiers
internal SMTP values
private tenant structure
sensitive reporting content

Any resemblance to real environments in the public sample data is purely illustrative.

# Status
Public repository status

Active and evolving.

Current public direction
strong PowerShell foundation
multi-source unified model
public Defender enrichment model
dashboard-ready JSON outputs
frontend-ready evolution path
Author

Built as a practical PowerShell security project focused on:

clean structure
real-world usefulness
Microsoft ecosystem relevance
portfolio credibility
progression toward security / automation / cloud-oriented roles

# Author

Cybersecurity Analyst focused on:
- Microsoft Security
- Endpoint Visibility
- Entra ID / Intune
- Security Operations
- PowerShell Automation
