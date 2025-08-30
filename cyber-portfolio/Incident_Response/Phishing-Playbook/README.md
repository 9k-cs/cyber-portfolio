# 🧭 Phishing Incident Response Playbook (Lab)

## Objective
Document and automate steps to triage, contain, and remediate phishing attempts in Microsoft 365.

## Scope & Tools
- **Environment:** M365 dev tenant
- **Tools:** Exchange Admin Center, Defender for Office 365, Python for header parsing
- **Frameworks:** NIST CSF – Respond/Recover; MITRE – Initial Access (T1566)

## Workflow (High-Level)
1. Intake & triage (user report, automated detections)
2. Header analysis (SPF/DKIM/DMARC, Received chain)
3. Containment (message trace, purge, block sender/domains)
4. User comms & awareness
5. Root cause & prevention (rules, transport policies)

## Evidence
- Placeholder for redacted screenshots / synthetic headers
