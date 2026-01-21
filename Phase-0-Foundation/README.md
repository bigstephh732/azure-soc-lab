## Phase 0 – Foundation Setup

## Objective

Establish a secure Microsoft cloud foundation to support a Security Operations Center (SOC) lab environment. This phase focuses on identity setup, tenant validation, and confirming administrative access before enabling security tooling.



## Environment
	•	Platform: Microsoft Azure + Microsoft Entra ID
	•	Tenant: SOC Lab (custom tenant)
	•	Role: Global Administrator
	•	Endpoint: macOS (primary lab device)
	•	Browser Access: Azure Portal, Microsoft Defender Portal



## Tasks Completed

## 1. Microsoft Entra ID Tenant Setup
	•	Confirmed active Entra tenant
	•	Verified tenant ID and primary domain
	•	Confirmed global administrator role assignment
	•	Validated user account access

Purpose:
Identity is the control plane of cloud security. All SOC tools depend on proper Entra configuration.



## 2. Azure Portal Access Verification
	•	Logged into Azure Portal successfully
	•	Confirmed access to:
	•	Azure services dashboard
	•	Resource creation options
	•	Subscription onboarding page

Purpose:
Ensures readiness for future SOC components such as Sentinel, Log Analytics, and VM-based telemetry.



## 3. Microsoft Defender Portal Access
	•	Accessed security.microsoft.com
	•	Verified visibility of:
	•	Defender settings
	•	Endpoint configuration
	•	XDR navigation options

Purpose:
Confirms tenant is recognized by Microsoft security stack and ready for endpoint onboarding.



## 4. Role & Permissions Validation
	•	Confirmed Global Administrator privileges
	•	Verified permissions across:
	•	Entra ID
	•	Defender portal
	•	Security settings pages

Purpose:
SOC analysts must understand role-based access control (RBAC) and privilege boundaries.



## Security Concepts Practiced
	•	Identity as the security perimeter
	•	Role-based access control (RBAC)
	•	Tenant-level security governance
	•	Cloud control plane validation
	•	SOC environment preparation



## Outcome

The cloud identity foundation is fully operational.
The tenant is ready for endpoint onboarding, telemetry ingestion, and security detection activities in Phase 1.



## Key Takeaway

Before detection and response can occur, a SOC must ensure:
	•	Identity is secure
	•	Roles are correct
	•	Management portals are accessible
	•	Logging paths can be enabled

This phase mirrors real-world SOC onboarding procedures.





### Screenshot 1: Microsoft Entra Tenant Overview
- Confirms successful tenant creation
- Shows Global Administrator role assignment
- Verifies identity platform readiness

### Screenshot 2: Azure Portal Access
- Confirms Azure portal access
- Validates tenant-to-Azure linkage
- Confirms readiness for SOC tooling

### Screenshot 3: Microsoft Defender Settings
- Confirms Defender portal availability
- Shows Defender XDR and Endpoint services
- Validates security platform initialization## PHASE 0 — FOUNDATION LAB




