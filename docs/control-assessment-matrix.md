# Control Assessment Matrix – NIST Cybersecurity Framework (CSF)

## Purpose
This document records the evaluation of selected NIST Cybersecurity Framework (CSF) subcategories against a Windows 11 endpoint. Each control is assessed based on evidence gathered from system configuration, vulnerability scanning, and observable behavior.

The objective is to determine whether controls are implemented, partially implemented, or not implemented, and to identify associated risk and remediation actions.

## Assessment Summary
- **Framework:** NIST Cybersecurity Framework (CSF)
- **Assessment Scope:** Single Windows 11 endpoint (VMware)
- **Assessment Type:** Technical control assessment
- **Method:** Evidence-based evaluation
- **Outcome:** Control gaps identified, risks documented, remediation recommended

## Control Assessment Matrix

| NIST CSF Function | Subcategory ID | Control Description | Control Status | Evidence Reviewed | Risk Level | Notes |
|------------------|---------------|---------------------|----------------|-------------------|------------|-------|
| Identify | ID.AM-1 | Physical devices and systems within the organization are inventoried | Implemented | Windows system information, VM inventory | Low | Endpoint identified and documented |
| Identify | ID.AM-2 | Software platforms and applications within the organization are inventoried | Partially Implemented | Nessus authenticated scan, installed software list | Medium | Inventory exists but not centrally managed |
| Protect | PR.AC-1 | Identities and credentials are issued, managed, verified, revoked | Implemented | Local user accounts, credentialed scan access | Low | Standard authentication mechanisms in place |
| Protect | PR.AC-4 | Access permissions are managed | Implemented | Local group membership review | Low | Least-privilege model applied |
| Protect | PR.IP-1 | A baseline configuration is established and maintained | Partially Implemented | Default OS configuration, vulnerability findings | Medium | No formal baseline documented |
| Detect | DE.CM-1 | Network is monitored to detect potential cybersecurity events | Not Implemented | No centralized monitoring present | High | No SIEM or endpoint monitoring configured |
| Detect | DE.CM-7 | Monitoring for unauthorized personnel or activity | Partially Implemented | Windows Event Logs | Medium | Logging exists but lacks alerting |
| Respond | RS.AN-1 | Notifications from detection systems are investigated | Not Implemented | No alerting workflow defined | High | No formal response procedures |
| Respond | RS.MI-1 | Incidents are contained | Not Implemented | No response tooling configured | High | Response capability not established |
| Recover | RC.IM-1 | Recovery plans incorporate lessons learned | Not Implemented | No recovery documentation | Medium | Improvement process informal |

## Control Status Definitions

- **Implemented:** Control is present and functioning as intended
- **Partially Implemented:** Control exists but lacks completeness or consistency
- **Not Implemented:** Control is absent or ineffective

## Key Observations
- Technical visibility exists but is not centralized
- Preventive controls are stronger than detective and response controls
- Lack of monitoring and response capabilities increases residual risk
- Documentation gaps elevate compliance and audit risk

## Next Steps
- Document findings in the risk register
- Prioritize high-risk gaps for remediation
- Define compensating controls where full implementation is not feasible
- Reassess controls after remediation activities

## Analyst Notes
This assessment highlights that compliance is not binary. Controls must be evaluated based on real-world effectiveness, evidence, and operational context rather than checklist completion.
