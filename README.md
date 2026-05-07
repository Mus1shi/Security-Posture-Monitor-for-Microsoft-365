# Security Posture Monitor for Microsoft 365

PowerShell-based security posture monitoring and device correlation platform for Microsoft 365 environments.

## Correlates data from:
- Microsoft Entra ID
- Microsoft Intune
- Microsoft Defender
- Trend Micro

## Designed to improve:
- endpoint visibility
- BYOD detection
- compliance monitoring
- Defender operational analysis
- missing KB visibility
- security reporting

## Automated HTML security report generated after device correlation and risk analysis.

<img width="942" height="1337" alt="Capture d&#39;écran 2026-04-17 091045" src="https://github.com/user-attachments/assets/c9d645d7-5822-45a2-974d-eacb17f93f05" />

The platform classifies devices based on:
- compliance status
- Defender activity
- visibility gaps
- missing KBs
- correlation signals

<img width="932" height="589" alt="Capture d&#39;écran 2026-04-17 091059" src="https://github.com/user-attachments/assets/7d850b3d-f1f4-40dc-be55-662905ef4c8c" />


# Why I Built This

Modern Microsoft 365 environments often suffer from fragmented endpoint visibility across multiple management and security platforms.

This project was designed to:
- centralize device visibility
- correlate security signals
- identify unmanaged or partially visible endpoints
- improve operational reporting
- support security and helpdesk workflows

# Features

- Multi-source device correlation
- Microsoft Defender integration
- Entra ID visibility analysis
- Intune compliance analysis
- Potential BYOD detection
- Missing KB analysis
- Active vs inactive Defender classification
- Automated HTML reporting
- JSON and CSV exports
- Risk scoring engine
- Modular PowerShell architecture

# Architecture

Entra ID
   │
Intune
   │
Trend Micro
   │
Microsoft Defender
   ▼
Correlation Engine
   ▼
Risk Engine
   ▼
Reports / JSON / HTML Mail

# Example Workflow

1. Collect device inventories
2. Normalize identities across platforms
3. Correlate devices between sources
4. Detect visibility gaps
5. Analyze Defender activity
6. Detect missing KBs
7. Apply risk scoring
8. Generate operational reports

# Technical Challenges

- Cross-platform device identity correlation
- Duplicate hostname normalization
- Partial visibility handling
- Microsoft Defender API throttling
- Large dataset processing
- Missing KB optimization logic
- Active vs inactive Defender classification

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

---


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
