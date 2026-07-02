# Conditional Access Design

## Project Overview

This document outlines the Conditional Access policies that would be implemented in an enterprise environment.

> **Note:** Microsoft Entra ID Free does not support Conditional Access. These policies were designed to demonstrate knowledge of Zero Trust principles and enterprise identity security.

---

## Policy 1 – Require MFA for Administrators

**Purpose:** Protect privileged administrator accounts.

**Users:** IT-Admins

**Applications:** All cloud applications

**Grant Control:** Require Multi-Factor Authentication (MFA)

**Business Justification:** Administrator accounts are high-value targets. Requiring MFA significantly reduces the risk of unauthorized access.

---

## Policy 2 – Block Legacy Authentication

**Purpose:** Block older authentication protocols that do not support MFA.

**Business Justification:** Legacy authentication is commonly targeted in password spraying and brute-force attacks.

---

## Policy 3 – Require MFA for Remote Workers

**Purpose:** Secure remote access to Microsoft 365 resources.

**Users:** Remote Workers

**Grant Control:** Require MFA

**Business Justification:** Remote users connect from networks outside the organization's control, increasing security risks.

---

## Policy 4 – Block Sign-ins from High-Risk Locations

**Purpose:** Restrict authentication attempts from countries where the organization has no business operations.

**Business Justification:** Reduces the risk of unauthorized access and credential-based attacks.

---

## Implementation Note

These policies were designed but not implemented because Microsoft Entra ID Free does not include Conditional Access. Microsoft Entra ID Premium P1 or P2 would be required to deploy these policies.