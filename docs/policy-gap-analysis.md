# Policy Gap Analysis – NIST CSF Alignment

## Purpose
This document evaluates the presence and adequacy of security policies relative to the NIST Cybersecurity Framework (CSF). The goal is to identify policy-level gaps that increase organizational risk, even when technical controls may partially exist.

This analysis focuses on whether controls are **formally defined, documented, and enforceable**, not just whether they are technically possible.

## Assessment Scope
- **Framework:** NIST Cybersecurity Framework (CSF)
- **Environment:** Windows 11 endpoint (virtualized lab system)
- **Assessment Type:** Policy existence and coverage review
- **Out of Scope:** Enterprise-wide governance, third-party risk, cloud policy

## Summary of Findings
Several technical controls were observed to exist informally; however, **formal security policies were largely absent or undocumented**. This creates risk related to inconsistency, auditability, and accountability.

The most significant gaps were identified in the **Detect**, **Respond**, and **Recover** functions of the NIST CSF.

## Policy Coverage Assessment

### Identify (ID)

| Control Area | Policy Status | Gap Identified |
|-------------|--------------|---------------|
| Asset Inventory | Partial | No documented asset management policy |
| Risk Assessment | Missing | No formal risk assessment methodology |
| Governance | Missing | No defined roles or accountability model |

**Impact:**  
Without formal identification policies, risk decisions are informal and difficult to audit.

### Protect (PR)

| Control Area | Policy Status | Gap Identified |
|-------------|--------------|---------------|
| Configuration Management | Partial | No secure baseline documentation |
| Vulnerability Management | Partial | Process exists, policy not documented |
| Access Control | Partial | No written access control standards |

**Impact:**  
Controls may be applied inconsistently across systems and environments.

### Detect (DE)

| Control Area | Policy Status | Gap Identified |
|-------------|--------------|---------------|
| Logging & Monitoring | Missing | No centralized logging policy |
| Detection Processes | Missing | No defined detection thresholds or alerting standards |

**Impact:**  
Security incidents may go undetected or identified too late.

---

### Respond (RS)

| Control Area | Policy Status | Gap Identified |
|-------------|--------------|---------------|
| Incident Response | Missing | No formal IR policy or playbooks |
| Communication | Missing | No escalation or notification procedures |
| Analysis | Missing | No guidance on evidence handling |

**Impact:**  
Response actions rely on individual judgment, increasing operational risk.

### Recover (RC)

| Control Area | Policy Status | Gap Identified |
|-------------|--------------|---------------|
| Recovery Planning | Missing | No documented recovery procedures |
| Lessons Learned | Missing | No formal post-incident review process |

**Impact:**  
Extended downtime and limited organizational learning after incidents.

---

## Key Policy Gaps Identified

1. Absence of documented **Incident Response Policy**
2. Lack of **Logging and Monitoring Standards**
3. No formal **Risk Assessment Policy**
4. No documented **Vulnerability Management Policy**
5. Missing **Recovery and Business Continuity Guidance**

## Risk Implications
Even when technical controls exist, the absence of formal policy introduces the following risks:

- Inconsistent security implementation
- Reduced audit readiness
- Increased regulatory and compliance exposure
- Dependence on individual knowledge rather than institutional process

From a compliance perspective, **undocumented controls are functionally equivalent to nonexistent controls**.

## Recommendations
To reduce policy-related risk, the following actions are recommended:

- Develop and approve baseline security policies aligned to NIST CSF
- Define ownership and accountability for each control domain
- Establish documentation standards for detection, response, and recovery
- Integrate policy review into continuous improvement cycles

These steps prioritize governance maturity over tool deployment.

## Conclusion
This policy gap analysis demonstrates that cybersecurity risk is not solely technical. Governance, documentation, and accountability are equally critical components of a defensible security program.

The findings reinforce the importance of policy-driven security management aligned with recognized frameworks such as NIST CSF.

## Analyst Note
This analysis is intentionally scoped to policy presence rather than enforcement. Future assessments may evaluate policy effectiveness, compliance testing, and control validation.
