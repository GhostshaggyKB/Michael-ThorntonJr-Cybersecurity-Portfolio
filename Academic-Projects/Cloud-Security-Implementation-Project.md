# Azure Cloud Security Implementation and Compliance Plan

`Academic Project — Sanitized Portfolio Summary`

## Project Overview

I completed this cloud-security project as part of my graduate cybersecurity studies at Western Governors University.

The project required me to evaluate an existing Microsoft Azure environment, identify security and governance gaps, implement security improvements in an authorized lab, and develop recommendations that aligned cloud resources with business, security, and compliance requirements.

This public portfolio page is intentionally limited to a high-level professional summary. Assessment materials, scenario details, account information, resource identifiers, screenshots, exact configurations, and submitted work are not published.

---

## Areas of Focus

The project involved practical application of:

- Microsoft Azure security
- Infrastructure as a Service (IaaS)
- Identity and access management
- Azure role-based access control (RBAC)
- Least privilege
- Azure resource organization
- Azure Key Vault
- Encryption at rest
- Encryption in transit
- Azure Backup
- Recovery planning
- Cloud shared-responsibility concepts
- Vulnerability management
- Cloud risk analysis
- Regulatory and compliance considerations
- Threat mitigation
- Security documentation

---

## Security Assessment

I evaluated the cloud environment for security weaknesses involving access control, resource organization, data protection, backup readiness, and security governance.

The assessment required me to consider whether cloud resources and permissions were aligned with organizational responsibilities and whether existing controls adequately supported least privilege and separation of duties.

I also evaluated risks associated with:

- Excessive access permissions
- Improperly scoped cloud resources
- Weak separation between organizational functions
- Inadequate backup verification
- Unmonitored or unpatched cloud systems
- Privileged-access misuse
- Cloud configuration errors
- Third-party and software supply-chain risk

---

## Identity and Access Management

A major portion of the project focused on improving access control using Azure RBAC.

I evaluated existing role assignments and resource scopes and then implemented changes intended to reduce unnecessary access.

My approach emphasized:

- Assigning permissions according to job requirements
- Limiting role assignments to the narrowest practical scope
- Avoiding unnecessarily broad administrative permissions
- Separating resources according to organizational responsibility
- Applying the principle of least privilege

This work strengthened my understanding of how Azure RBAC combines roles and scopes to control access to cloud resources.

---

## Azure Key Vault

I evaluated the use of Azure Key Vault as part of the organization's data-protection strategy.

The design emphasized separating access to sensitive cryptographic resources and limiting management permissions to authorized users.

I also evaluated how Key Vault can support:

- Secure key management
- Secret management
- Certificate management
- Customer-managed encryption keys
- Encryption of stored data
- Protection of data transmitted using encrypted connections
- Key and certificate lifecycle management

The project reinforced the importance of separating management-plane permissions from access to the sensitive data stored inside a vault.

---

## Encryption and Data Protection

I developed recommendations for protecting cloud information both at rest and in transit.

For data at rest, I evaluated the use of centrally managed encryption keys for supported Azure services.

For data in transit, I evaluated centralized certificate and key management to support encrypted communications between applications and services.

The goal was to ensure that cryptographic controls were paired with tightly scoped access rather than relying on encryption alone.

---

## Backup and Recovery

I evaluated the existing Azure backup environment and implemented an updated backup policy in the authorized lab.

The configuration was designed around business recovery requirements, including:

- Consistent scheduled backups
- Recovery-point retention
- Rapid-recovery capability
- Centralized backup management
- Recovery objectives
- Backup verification

This portion of the project reinforced that simply configuring a backup job is not enough.

A mature backup strategy also requires monitoring backup success, validating recovery points, and periodically confirming that systems can actually be restored.

---

## Shared Responsibility

I analyzed cloud security using the shared-responsibility model for an IaaS environment.

The project reinforced that moving infrastructure to Azure does not transfer all security responsibilities to Microsoft.

The cloud provider is responsible for protecting the underlying physical cloud infrastructure, while the customer remains responsible for areas such as:

- Identities
- Access permissions
- Data
- Guest operating systems
- Applications
- Cloud-resource configuration
- Network-security configuration
- Vulnerability management
- Backup and recovery
- Compliance implementation

Understanding this division of responsibility was important when evaluating which risks remained under organizational control.

---

## Risk and Compliance Analysis

I evaluated how cloud-security controls could support organizational compliance and risk-management requirements.

Rather than treating compliance as a checklist, I considered how controls such as:

- Least privilege
- Access reviews
- Vulnerability scanning
- Patch management
- Backup verification
- Logging and monitoring
- Strong authentication
- Secure configuration

could provide both security value and evidence that cloud resources were being actively governed.

The project also included consideration of established security frameworks and regulatory requirements relevant to cloud environments.

---

## Threat Analysis

I evaluated several categories of threats that could affect an Azure environment.

These included:

- Privileged-access abuse
- Compromised identities
- Exploitation of unpatched systems
- Long-term unauthorized access
- Software supply-chain compromise
- Excessive permissions
- Cloud-resource misconfiguration

For each area, I considered preventive and detective controls such as least privilege, access reviews, vulnerability management, endpoint protection, network restrictions, logging, monitoring, and secure software practices.

---

## Security Recommendations

My recommendations emphasized maintaining cloud security as an ongoing operational process.

Key themes included:

### Regular Access Reviews

Cloud permissions should be reviewed periodically and whenever users change responsibilities or leave an organization.

### Vulnerability Management

Cloud systems should be formally included within vulnerability-scanning, patch-management, and remediation programs.

### Backup Verification

Backup jobs should be monitored and recovery testing should be performed periodically rather than assuming that a configured backup policy guarantees recoverability.

### Least Privilege

Administrative permissions should be limited to the minimum role and scope necessary for each function.

### Continuous Monitoring

Security-relevant identity, administrative, endpoint, and cloud activity should be monitored so abnormal behavior can be identified and investigated.

---

## Skills Demonstrated

This project demonstrates experience with:

- Microsoft Azure security
- Azure RBAC
- IAM
- Least privilege
- Azure resource organization
- Azure Key Vault
- Key and certificate management concepts
- Encryption at rest
- Encryption in transit
- Azure Backup
- Recovery planning
- Cloud shared responsibility
- Cloud risk analysis
- Vulnerability-management planning
- Compliance considerations
- Threat modeling
- Security-control recommendations
- Cloud-security documentation

---

## What I Learned

This project strengthened my understanding that cloud security depends heavily on configuration and governance.

A secure cloud provider does not automatically make an organization's workloads secure.

Identity permissions, operating systems, applications, backup policies, network controls, data protection, and monitoring still require deliberate security decisions.

I also gained a better understanding of how several Azure security capabilities work together.

RBAC controls who can manage resources, Key Vault protects sensitive cryptographic material, encryption protects stored and transmitted information, and backup controls improve resilience and recoverability.

The project reinforced that these controls are most effective when they are implemented as part of a broader least-privilege, risk-management, and continuous-monitoring strategy.

---

## Academic Integrity and Publication Notice

This public portfolio summary intentionally excludes:

- The WGU assessment prompt
- Grading rubrics
- Course instructions
- Skillable lab instructions
- The original scenario organization
- Usernames or account information
- Resource identifiers
- Exact role assignments
- Exact configuration values
- Exact backup schedules or retention values
- Protected screenshots
- Credentials
- Complete or partial submitted assessment content
- Step-by-step instructions for completing the assessment

The content presented here is an original, high-level professional summary of the cloud-security skills and decisions demonstrated during the project.

---

## Portfolio Classification

School: Western Governors University (WGU)  
Course: D485 — Cloud Security  
Status: Completed  
Type: Academic Project — Sanitized Portfolio Summary  
Primary Areas: Azure Security, IAM, RBAC, Least Privilege, Key Vault, Encryption, Backup and Recovery, Cloud Risk, Compliance
