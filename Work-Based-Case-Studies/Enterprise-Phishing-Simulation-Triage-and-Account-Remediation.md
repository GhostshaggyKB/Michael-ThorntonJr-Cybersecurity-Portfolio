# Enterprise Phishing Simulation Triage and Account Remediation

**Work-Based Case Study — Sanitized Security Simulation**

## Overview

Participated in an authorized internal phishing simulation designed to evaluate phishing recognition, user reporting, incident triage, documentation, escalation, and account-remediation procedures.

The simulation was not disclosed to the support team in advance. I therefore handled each report as a potentially legitimate security incident until the organization’s security team confirmed that the activity was part of an authorized exercise.

This case study has been intentionally generalized to protect confidential organizational information.

## Initial Reports

A user contacted support regarding a suspicious account-security message.

I initially escalated the report to the organization’s security team for review.

When a second user reported a message with similar characteristics, I requested that the suspicious message be forwarded for examination and used an approved remote-support session to inspect the message and surrounding context directly.

The similarity between the reports indicated that the activity could be part of a broader phishing campaign, so I contacted the security team to validate the pattern.

## Phishing Indicators Identified

During examination of the message, I identified several indicators consistent with credential-harvesting phishing:

- An unusual sender address that did not match commonly used organizational communication patterns
- A subtly malformed domain using `.corn` instead of `.com`
- Urgent language warning recipients that their account could be deleted
- A request directing recipients to authenticate using organizational credentials

After identifying the malformed domain and credential-harvesting behavior, I did not interact with the embedded link or attempt to access the destination.

The available indicators were sufficient to treat the message as malicious and continue escalation through the established security workflow.

## Incident Triage and Documentation

Each reported message was handled as an individual security case.

Using the organization’s established phishing-triage process, I documented the user’s level of interaction with the message, including whether the user:

- Interacted with the message
- Followed the embedded link
- Disclosed credentials
- Required account remediation

Each case was documented separately and routed to the organization’s security team for review.

After additional reports were received, the security team confirmed that the activity was part of an authorized internal phishing simulation.

## Account Containment and Remediation

Users who reported credential exposure required additional account-security actions.

My team and I supported containment by temporarily restricting affected accounts and MFA access until remediation could be completed.

When affected users contacted support following notification from the security team, I personally performed remediation activities that included:

- Verifying user identity through approved organizational verification methods
- Resetting affected credentials
- Restoring Active Directory account access after verification and remediation
- Re-enabling MFA access after account security requirements were satisfied

The organization’s internal security team handled notification to affected users, while my team supported the account-remediation and restoration process.

## Security Approach

I treated each reported security concern as potentially legitimate until sufficient evidence established otherwise.

Although the activity was ultimately confirmed as an authorized simulation, the reports were initially handled using the same cautious approach appropriate for a real phishing incident.

This helped ensure that suspicious activity was investigated, documented, and escalated rather than dismissed based on appearance or apparent source.

## Skills Demonstrated

- Phishing analysis
- Social-engineering recognition
- Lookalike-domain identification
- Credential-exposure triage
- Security incident documentation
- Pattern recognition across related reports
- Security-team escalation
- Active Directory account remediation
- MFA access management
- Identity verification
- Credential reset procedures
- Secure account restoration
- Incident-response coordination

## Key Takeaway

This exercise reinforced the importance of treating suspicious communications as potentially malicious until validated, recognizing patterns across separate user reports, avoiding unnecessary interaction with suspicious links, documenting exposure levels carefully, and coordinating account containment and recovery with the broader security team.

## Confidentiality Notice

This case study is a sanitized summary of professional work performed during an authorized internal security simulation.

Employer names, user identities, email addresses, ticket numbers, internal systems, exact campaign metrics, internal procedures, verification methods, screenshots, URLs, and other potentially sensitive information have intentionally been omitted or generalized.
