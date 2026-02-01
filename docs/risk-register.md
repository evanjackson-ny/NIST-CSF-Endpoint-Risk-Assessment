# Risk Register – NIST CSF Control Assessment

## Purpose
This document records identified cybersecurity risks resulting from gaps observed during the NIST Cybersecurity Framework (CSF) control assessment of a Windows 11 endpoint.

The risk register translates technical control deficiencies into business-relevant risk statements, supporting prioritization, remediation planning, and management decision-making.

## Risk Register Summary
- **Assessment Scope:** Single Windows 11 endpoint (VMware)
- **Risk Identification Method:** Control assessment and evidence review
- **Risk Rating Method:** Qualitative (Low / Medium / High)
- **Status:** Initial risk identification completed

## Risk Register

| Risk ID | Risk Description | Associated CSF Control | Likelihood | Impact | Risk Level | Current Controls | Recommended Treatment | Risk Owner | Status |
|--------|------------------|------------------------|------------|--------|------------|------------------|------------------------|------------|--------|
| R-01 | Lack of centralized monitoring may delay detection of malicious activity | DE.CM-1 | Medium | High | High | Local Windows Event Logs | Implement centralized logging and monitoring | IT / Security | Open |
| R-02 | Absence of formal incident response process may lead to unmanaged incidents | RS.AN-1 | Medium | High | High | Informal manual investigation | Develop incident response procedures and escalation paths | Security | Open |
| R-03 | No defined containment capability increases impact of security events | RS.MI-1 | Medium | High | High | Manual intervention only | Establish containment and response playbooks | Security | Open |
| R-04 | Incomplete asset and software inventory increases exposure to unpatched vulnerabilities | ID.AM-2 | Medium | Medium | Medium | Nessus authenticated scans | Implement centralized asset inventory process | IT | Open |
| R-05 | Lack of documented configuration baseline increases configuration drift risk | PR.IP-1 | Medium | Medium | Medium | Default OS configuration | Establish and document secure baseline configurations | IT | Open |
| R-06 | Limited recovery planning may slow restoration after security incidents | RC.IM-1 | Low | Medium | Medium | Informal recovery knowledge | Develop recovery documentation and lessons-learned process | IT | Open |

## Risk Rating Definitions

- **Likelihood**
  - Low: Unlikely to occur
  - Medium: Possible under normal conditions
  - High: Likely to occur

- **Impact**
  - Low: Minimal operational or security impact
  - Medium: Noticeable disruption or increased risk
  - High: Significant security, operational, or compliance impact

- **Risk Level**
  - Derived from Likelihood × Impact

## Key Observations
- Highest risks stem from gaps in detection and response capabilities
- Preventive controls are stronger than monitoring and response controls
- Most identified risks can be reduced through procedural and tooling improvements rather than major infrastructure changes

## Risk Treatment Strategy
The following treatment approaches are recommended:

- **Mitigate:** Implement missing controls where feasible
- **Accept:** Document and accept low-impact risks
- **Transfer:** Not applicable for current scope
- **Avoid:** Not applicable for current scope

Risk treatment decisions should be approved by appropriate stakeholders.

## Next Steps
- Align remediation actions with organizational priorities
- Track remediation progress and reassess risk levels
- Update risk register after control improvements
- Use this register to support audit and compliance reporting

## Analyst Notes
This risk register demonstrates how technical security findings are translated into business-relevant risk. It reflects real-world GRC practice where prioritization, documentation, and accountability are as important as technical controls themselves.
