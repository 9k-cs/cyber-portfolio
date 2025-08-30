# 📊 SIEM Alert Tuning (Lab Recreation)

## 1. Objective
Improve detection of suspicious authentication attempts in Microsoft Sentinel while reducing false positives.

## 2. Scope & Tools
- **Environment:** Azure trial tenant, Sentinel enabled
- **Tools:** Microsoft Sentinel, KQL
- **Frameworks:** NIST CSF – Detect; MITRE ATT&CK – T1078

## 3. Methodology
1. Ingest Windows Security Logs into Sentinel  
2. Baselined normal authentication patterns  
3. Auth anomaly KQL queries (geo-impossible, impossible travel, failed login spikes)  
4. Rule tuning (thresholds, exclusions for service accounts)  
5. Validation using lab-simulated brute-force activity

## 4. Findings & Results
- Reduced noise from ~120/day → ~10/day with higher precision signals
- Created a dashboard for auth anomalies

## 5. Challenges & Fixes
- Service account noise → excluded known SIDs, added time-of-day logic

## 6. Outcome
- Actionable alerts, faster triage, better analyst focus

## 7. Evidence
- See `sample_queries.kql` for sample detections (genericised)
