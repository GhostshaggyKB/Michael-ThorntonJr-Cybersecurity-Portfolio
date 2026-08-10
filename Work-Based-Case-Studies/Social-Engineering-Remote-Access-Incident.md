# Social Engineering and Unauthorized Remote Access Incident

`Work-Based Case Study — Sanitized Incident Reconstruction`

## Confidentiality Statement

This case study is a sanitized reconstruction of a real security-related incident I supported in a professional enterprise environment.

Company names, user identities, account information, ticket numbers, internal systems, vendor names, geographic details, and other potentially confidential information have been removed or generalized.

The purpose of this report is to demonstrate my investigation, containment, documentation, and escalation process without exposing employer or customer information.

---

## Executive Summary

A user contacted support after unexpectedly losing access to their workstation. The normal Windows password field was no longer visible, and the behavior did not match the organization's standard workstation configuration.

During troubleshooting, I learned that an individual claiming to be an IT technician had previously contacted the user through an enterprise collaboration platform. The caller had guided the user through installing remote-access software under the pretext of performing a quick software update.

As the investigation progressed, I identified additional indicators of compromise, including abnormal authentication activity and continued unexplained workstation activity.

After observing mouse movement without user interaction and the appearance of a PowerShell window, I instructed the user to immediately disconnect the workstation from all network connectivity and power it down.

I directly notified the Information Security team, classified the incident as a compromised-account case, assigned high urgency, and documented the incident timeline in the organization's ticketing system while events were occurring.

Information Security later confirmed malicious remote access, credential exposure, attempted credential-hash extraction, and malicious PowerShell activity. The affected workstation was subsequently reimaged and affected credentials were reset by the appropriate teams.

---

## General Environment

The incident occurred in a remote enterprise environment using:

* Windows workstations
* Centralized directory services
* Single sign-on
* Multi-factor authentication
* Cloud-based productivity applications
* Enterprise collaboration software
* Remote-support tools
* Centralized service-management ticketing
* Dedicated Information Security escalation procedures

My role was Tier 2 technical support with authorized access to account-management and MFA administration tools.

---

## Initial Report

The user contacted me after returning to their workstation and discovering that they had been logged out.

The normal Windows password-entry field was no longer visible.

The user also encountered an authentication-related server message.

This behavior was unusual because it did not match the organization's normal workstation configuration or expected lock-screen behavior.

The abnormal lockout was my first major indication that the issue might involve more than routine authentication troubleshooting.

---

## Discovery of Prior Activity

While investigating the lockout, I learned that another individual had contacted the user earlier through an enterprise collaboration platform while presenting themselves as an IT technician.

The caller told the user that they needed to perform a quick software update.

The caller then walked the user through installing remote-access software and establishing a remote session.

During that session, the user reported receiving a prompt from the remote-access software requesting permission for a data transfer.

The user denied the transfer request.

This information significantly increased my concern that the earlier support interaction may have been fraudulent.

---

## Indicators Observed

During the incident, I identified or documented the following indicators:

* Unexpected workstation logout
* Missing Windows password-entry field
* Authentication behavior inconsistent with normal workstation configuration
* Prior unsolicited contact from an individual claiming to be IT support
* Installation of remote-access software at the caller's direction
* User-reported data-transfer request
* Loss of access to cloud productivity applications
* Suspicious authentication activity
* Continued workstation activity without user input
* Unexpected mouse movement
* Appearance of a PowerShell window
* Repeated disruption of workstation access

---

## Information Reviewed

My investigation was limited to the systems and evidence available within my authorized Tier 2 support role.

I reviewed:

* The user's description of the earlier support interaction
* The user's description of the remote-access session
* Current workstation behavior
* Authentication failures
* MFA activity through the organization's MFA administration console
* Account status within authorized account-management systems

I did not perform forensic analysis, malware analysis, SIEM correlation, or endpoint forensics.

Those activities were outside my role and were escalated to Information Security.

---

## MFA Investigation

Using my authorized access to the organization's MFA administration console, I reviewed recent authentication activity associated with the affected account.

I identified three denied MFA attempts occurring during the incident.

The attempts originated from a foreign location and were automatically denied by location-based security controls.

This provided additional evidence that the account was experiencing suspicious authentication activity while the unauthorized remote-access incident was ongoing.

---

## Investigation Process

I initially approached the issue as an authentication and workstation-access problem.

The missing password field and abnormal logout behavior did not match normal workstation behavior, so I treated the issue cautiously.

After a power cycle, the workstation displayed a system configuration screen. After proceeding through the required setup process, the normal Windows login screen returned.

The user was able to regain access to the workstation, but cloud productivity and SSO-connected applications remained inaccessible.

At that point, I reset the affected account through the organization's directory service.

I:

* Assigned a temporary password
* Required a password change at the next login
* Terminated active cloud-account sessions
* Did not provide the temporary password to the user

I then instructed the user not to interact with the workstation so we could determine whether activity continued without user input.

While the user remained hands-off, the mouse began moving unexpectedly.

A PowerShell window also appeared.

These observations indicated that unauthorized remote access could still be active.

---

## Containment Actions

Once continued unauthorized activity was observed, I immediately shifted from troubleshooting to containment.

I instructed the user to:

1. Stop interacting with the workstation.
2. Remove all network connectivity.
3. Disconnect the laptop from the docking station.
4. Power the laptop completely off.

I remained on the call throughout the isolation and shutdown process to ensure the device was disconnected and powered down.

I initiated these containment actions before waiting for further direction because the workstation appeared to still be under unauthorized remote control.

---

## Escalation Decision

I determined that the issue required immediate Information Security involvement.

I directly contacted members of the Information Security team through the organization's collaboration platform to alert them to the active incident.

I then created a high-urgency ticket in the organization's service-management platform.

I personally:

* Categorized the incident as a compromised-account case
* Set the urgency to high
* Documented the incident timeline
* Recorded the user's reported activity
* Recorded authentication issues
* Documented my troubleshooting actions
* Documented containment actions
* Routed the incident to Information Security

The detailed ticket served as my incident report.

I documented the case while the incident was actively unfolding rather than reconstructing the timeline only afterward.

---

## Information Security Findings

After escalation, Information Security performed the deeper investigation.

The Information Security team confirmed that:

* The malicious actor initially contacted the user while impersonating IT support.
* The actor used a screen-sharing session to guide the user through installing remote-access software.
* The actor accessed the user's password-management application.
* Credentials stored within the password manager were exposed.
* The actor used that access to change the password associated with the user's cloud productivity account.
* The password change contributed to the user's loss of access to collaboration and productivity applications.
* The actor attempted to extract Windows credential hashes.
* The credential-hash extraction attempt was unsuccessful.
* PowerShell scripts were used in an attempt to disrupt legitimate access to the workstation.
* No additional malicious persistence or tooling was identified beyond the remote-access software.
* No additional data exfiltration was confirmed beyond the credential exposure identified during the investigation.

These findings were made by Information Security and were not conclusions I independently reached through forensic analysis.

---

## Remediation and Outcome

Post-incident remediation was performed by the appropriate technical and security teams.

Remediation included:

* Reimaging the affected workstation
* Resetting affected passwords
* Removing unauthorized remote-access software
* Restricting administrative privileges for standard users
* Limiting elevated administrative access to authorized IT and Information Security personnel

I did not personally perform the workstation reimage or organization-wide privilege changes.

My responsibility was incident recognition, initial investigation, account-containment actions within my authorized role, workstation isolation, documentation, and escalation.

Information Security provided positive feedback regarding the speed of the containment and escalation actions.

---

## Skills Demonstrated

This incident demonstrates practical experience with:

* Security incident triage
* Social-engineering recognition
* Account-compromise response
* Authentication troubleshooting
* MFA investigation
* Active Directory account administration
* Cloud-session termination
* Remote-access incident recognition
* Endpoint containment
* Security escalation
* Incident severity assessment
* Real-time incident documentation
* Service-management ticketing
* Communication with Information Security
* Distinguishing observed evidence from confirmed forensic findings

---

## Lessons Learned

One of my most important takeaways from this incident was the value of listening carefully when a user describes what happened before the technical problem began.

The issue initially presented as an unusual workstation lockout.

Learning that another supposed IT technician had recently contacted the user changed the context of the investigation and helped connect the authentication problems with a potential social-engineering incident.

The abnormal lockout behavior itself was an important warning sign because it did not match the organization's normal workstation configuration.

The incident reinforced several principles:

* Unexpected IT contact should be treated cautiously.
* Small details provided by the user can change the direction of an investigation.
* Abnormal authentication behavior should not automatically be treated as a routine password problem.
* Observing a system without user interaction can help identify continued unauthorized activity.
* MFA activity can provide valuable supporting evidence during an account-security investigation.
* Active unauthorized access requires rapid containment.
* Accurate real-time documentation improves escalation quality.
* Security incidents should be escalated when investigation requirements exceed the responder's authorized role.
* Existing least-privilege and security-awareness controls remain important even when formal policies are already in place.

---

## Portfolio Classification

**Source:** Professional work experience
**Type:** Sanitized incident reconstruction
**Primary Areas:** Incident Response, Account Security, Social Engineering, MFA, Endpoint Containment, Security Escalation
**Confidentiality:** All identifying and potentially NDA-covered information has been removed or generalized.
