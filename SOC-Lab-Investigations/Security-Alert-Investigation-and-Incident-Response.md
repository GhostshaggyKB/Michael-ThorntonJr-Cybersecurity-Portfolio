# Security Alert Investigation and Incident Response Analysis

`Academic/Simulated Security Operations Project`

## Publication Notice

This project is an original portfolio summary based on work I completed in an authorized cybersecurity academic environment.

The scenario, identifiers, technical values, screenshots, challenge content, and step-by-step assessment procedures have intentionally been removed or generalized.

This page is intended to demonstrate my security operations skills without reproducing protected academic material or providing an answer key.

---

## Project Summary

I completed a simulated security operations investigation involving a potentially compromised Windows-based server that was affecting the availability and performance of an important business application.

The investigation required me to distinguish a routine technical-performance problem from a security incident by reviewing multiple sources of evidence and evaluating the broader context surrounding the affected system.

I followed a structured incident-response process that included:

- Detection
- Investigation
- Risk assessment
- Containment
- Remediation
- Documentation
- Preventative recommendations

---

## Initial Situation

Multiple simulated users reported similar performance problems involving a shared business application.

Because the issue affected several users and continued after standard troubleshooting, I determined that the problem was more likely associated with the shared server environment than with a single workstation or file.

Additional information suggested that an unverified software change had recently occurred.

This increased the possibility that the performance issue could have a security-related cause.

---

## Detection and Triage

I reviewed the available security monitoring data to determine whether the affected system showed indicators consistent with malicious activity.

The available telemetry showed abnormal system-resource utilization and suspicious outbound network communication.

I correlated those observations with the reported business impact and the recent unverified software activity.

Based on the combined evidence, I treated the system as potentially compromised and continued with a security-focused investigation.

---

## Investigation

I used a SIEM platform to review security events and network-related metadata associated with the affected environment.

I identified outbound communication that did not match the expected behavior of the system.

I then examined activity on the affected Windows server and identified a suspicious process consuming unusually high system resources.

Further investigation indicated that the process was associated with unauthorized malware activity.

I also discovered that endpoint-protection functionality was not operating as expected.

These findings helped explain both the system-performance problems and the suspicious network activity.

---

## Key Findings

The investigation identified several security concerns:

- Abnormal resource consumption on a shared server
- Suspicious outbound network communication
- Unauthorized malware activity
- Reduced endpoint-protection effectiveness
- A recent software change that had not been sufficiently verified
- Security controls that allowed the malicious activity to continue longer than necessary

The combination of these findings supported treating the system as compromised.

---

## Containment and Remediation

I performed remediation within the authorized lab environment.

My response included:

- Restoring endpoint-protection functionality
- Scanning the affected system
- Allowing the endpoint-security platform to remediate the detected threat
- Implementing a firewall control to block the identified unauthorized outbound communication
- Verifying that the network-control change was applied correctly

These actions addressed both the endpoint and network components of the incident.

---

## Risk Assessment

I treated the incident as high priority because it involved:

- A compromised shared system
- Malware execution
- Business-service disruption
- Multiple affected users
- Suspicious external communication
- Security-control failure
- A social-engineering-related entry point

The incident demonstrated how a seemingly ordinary performance problem can represent a larger security event when multiple indicators are correlated.

---

## Root Cause

The investigation indicated that inadequate verification of a software update contributed to the compromise.

The scenario demonstrated the risk of trusting software-update communications without independently confirming their legitimacy.

It also showed how disabled or ineffective security controls can increase the impact of a successful compromise.

---

## Preventative Recommendations

### Verify Software Updates

Administrators should independently verify software updates using trusted vendor channels rather than relying solely on links delivered through email or other unsolicited communications.

### Monitor Endpoint Protection

Security teams should monitor the operational status of endpoint-protection systems and alert when critical protections are unexpectedly disabled or changed.

### Restrict Outbound Communication

Servers should be limited to the outbound network destinations and services required for their business function.

Unexpected outbound activity should be logged and investigated.

### Strengthen Change Management

Changes to important systems should follow a documented process that includes verification, review, testing, and rollback planning.

### Improve Security Awareness

Users and administrators should remain cautious when receiving unexpected technical requests or software-update instructions, even when the communication appears to come from a familiar source.

---

## Skills Demonstrated

This project demonstrates experience with:

- Security incident triage
- SIEM investigation
- Security-event analysis
- Network-traffic analysis
- Malware identification
- Windows process investigation
- Endpoint-security remediation
- Firewall-based containment
- Incident prioritization
- Root-cause analysis
- Risk assessment
- Security-control recommendations
- Incident documentation
- Preventative security planning

---

## What I Learned

This project reinforced the importance of looking beyond the initial symptom of a technical problem.

A slow or unstable application does not automatically indicate a cybersecurity incident. However, when that behavior is combined with abnormal resource usage, suspicious network activity, security-control issues, and an unverified system change, the overall risk picture changes significantly.

I also learned the importance of addressing multiple layers of an incident.

Removing a malicious process alone is not sufficient if unauthorized network communication remains possible or endpoint protections remain disabled.

Effective incident response requires identifying the immediate threat, containing its communication, restoring defensive controls, documenting the incident, and identifying improvements that can reduce the likelihood of recurrence.

---

## Academic Integrity

This repository does not contain:

- Assessment questions
- Challenge answers
- Grading rubrics
- Course instructions
- Exact lab identifiers
- Exact IP addresses or ports
- Hostnames or account information
- Credentials
- Protected screenshots
- Complete submitted assessment content
- Step-by-step instructions for completing the academic exercise

The content presented here is an original professional summary of the cybersecurity skills and decision-making demonstrated during the project.

---

## Portfolio Classification

Source: WGU Security Operations coursework  
Environment: Authorized simulated cybersecurity lab  
Type: Academic / Simulated Security Operations Project  
Primary Areas: Incident Response, SIEM Analysis, Malware Response, Endpoint Security, Network Containment, Risk Assessment, Security Documentation
