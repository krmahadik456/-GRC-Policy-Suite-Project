# Access Control Policy

| **Document Information** | |
|--------------------------|---|
| **Document Owner:** | IT Director |
| **Version:** | 1.0 |
| **Effective Date:** | June 24, 2026 |
| **Review Date:** | June 24, 2027 |
| **Approved By:** | CISO |
| **Classification:** | Internal |

---

## 1. Purpose

The purpose of this policy is to define the rules and procedures for controlling access to SecurePay Technologies' information assets. This policy ensures that only authorized individuals have access to the resources they need to perform their job functions, in accordance with the principle of least privilege.

---

## 2. Scope

This policy applies to:
- All users accessing SecurePay Technologies' systems, applications, and data
- All systems, applications, and networks owned or operated by SecurePay Technologies
- All devices used to access SecurePay Technologies' resources, including personal devices
- All third parties accessing SecurePay Technologies' resources

---

## 3. Policy Statements

### 3.1 User Account Management

**3.1.1 Account Creation**
- Accounts shall only be created upon approved request
- Requests shall include justification and required access level
- Accounts shall be created with minimum privileges necessary
- Default passwords shall be changed upon first login

**3.1.2 Account Types**

| Account Type | Description | Examples |
|--------------|-------------|----------|
| **Standard User** | Regular employee access | Email, applications, shared drives |
| **Privileged User** | Administrative or elevated access | System administrators, database admins |
| **Service Account** | Automated processes | Application-to-application communication |
| **Guest Account** | External users | Contractors, visitors, auditors |

**3.1.3 Account Review**
- All user accounts shall be reviewed quarterly
- Inactive accounts (45+ days) shall be disabled
- Privileged accounts shall be reviewed monthly
- Account reviews shall be documented

**3.1.4 Account Termination**
- Accounts shall be disabled immediately upon:
  - Employment termination
  - Contract expiration
  - Role change requiring different access
  - Suspicion of compromise

### 3.2 Password Requirements

**3.2.1 Password Complexity**
- Minimum length: 12 characters
- Must include: uppercase letters, lowercase letters, numbers, special characters
- Passwords shall not contain:
  - Dictionary words
  - Personal information (name, birthday)
  - Common patterns (123456, password, qwerty)

**3.2.2 Password Management**
- Password change frequency: Every 90 days
- Password reuse: No reuse of last 5 passwords
- Account lockout: After 5 failed attempts
- Lockout duration: 15 minutes

**3.2.3 Password Storage**
- Passwords shall be stored using secure hashing algorithms
- Passwords shall not be stored in clear text
- Password managers are recommended for personal use

### 3.3 Multi-Factor Authentication (MFA)

MFA shall be required for:

| Access Type | Requirement |
|-------------|-------------|
| Remote access (VPN, web portal) | ✅ Required |
| Administrative access | ✅ Required |
| Access to critical systems | ✅ Required |
| Financial systems | ✅ Required |
| Customer data (PII, KYC) | ✅ Required |
| Standard user access (email, applications) | Recommended |

**MFA Methods:**
- Authenticator apps (Google Authenticator, Microsoft Authenticator)
- Hardware tokens (YubiKey)
- Biometric verification
- SMS-based OTP (if no other option available)

### 3.4 Privileged Access Management

**3.4.1 Privileged Account Management**
- Privileged accounts shall be uniquely assigned (no shared accounts)
- Privileged access shall be logged and monitored
- Privileged sessions shall be limited to minimum required duration
- Privileged accounts shall use MFA

**3.4.2 Just-in-Time Access**
- Privileged access shall be granted on a just-in-time basis
- Access requests shall require approval
- Access shall expire after the specified duration

### 3.5 Remote Access

**3.5.1 Remote Access Requirements**
- Remote access shall only be permitted through approved VPN or secure gateway
- MFA is required for all remote access
- Remote sessions shall be encrypted
- Remote access shall be logged and monitored

**3.5.2 BYOD (Bring Your Own Device)**
- Personal devices used for work must:
  - Have up-to-date anti-virus software
  - Be encrypted
  - Have screen lock (timeout ≤ 5 minutes)
  - Be enrolled in MDM (Mobile Device Management)
- Company data shall be separated from personal data
- Devices shall be subject to remote wipe if lost or compromised

### 3.6 Access Control Models

| Model | Description | Application |
|-------|-------------|-------------|
| **Role-Based Access Control (RBAC)** | Access based on job role | Primary model for SecurePay Technologies |
| **Rule-Based Access Control** | Access based on rules | Firewall rules, time-based access |
| **Attribute-Based Access Control** | Access based on attributes | Contextual access decisions |

### 3.7 Monitoring and Logging

All access events shall be logged, including:
- Successful and failed login attempts
- Access to sensitive data
- Privileged account usage
- Changes to access controls
- Account creation and termination

Logs shall be:
- Retained for at least 1 year
- Monitored for suspicious activity
- Accessible to auditors upon request

---

## 4. Roles and Responsibilities

| Role | Responsibility |
|------|----------------|
| **System Administrators** | Manage user accounts, implement access controls, review accounts |
| **Data Owners** | Approve access to their data, review access quarterly |
| **All Users** | Protect their credentials, report suspicious activity |
| **Security Team** | Monitor access logs, investigate suspicious activity |
| **HR Department** | Notify IT of employee terminations |

---

## 5. Compliance and Enforcement

### 5.1 Compliance Monitoring
- Access reviews shall be conducted quarterly
- Access logs shall be reviewed for suspicious activity
- Auditors shall have access to access control records

### 5.2 Enforcement
- Violations of this policy may result in disciplinary action
- Unauthorized access may result in legal action

---

## 6. Review and Update Schedule

This policy shall be reviewed:
- At least annually
- When significant changes occur in:
  - Technology infrastructure
  - Regulatory requirements
  - Threat landscape

---

## 7. References

- ISO/IEC 27001:2022 (Section 9.1)
- NIST SP 800-53 (AC-2, AC-3, AC-6)
- PCI DSS (Section 7)
- SecurePay Technologies' Information Security Policy

---

## 8. Definitions

| Term | Definition |
|------|------------|
| **Least Privilege** | Users should have the minimum access necessary to perform their job |
| **MFA** | Multi-Factor Authentication |
| **RBAC** | Role-Based Access Control |
| **BYOD** | Bring Your Own Device |
| **MDM** | Mobile Device Management |
| **OTP** | One-Time Password |

---

## 9. Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | June 24, 2026 | Kaustubh Mahadik | Initial creation |
