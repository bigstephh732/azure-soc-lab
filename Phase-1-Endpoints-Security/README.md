## Phase 1 – Endpoint Security (Microsoft Defender for Endpoint)


## Objective

Deploy and validate endpoint detection and response (EDR) capabilities using Microsoft Defender for Endpoint (MDE). This phase focuses on onboarding a macOS device, verifying telemetry flow, and confirming detection visibility within the Defender portal.



## Environment
	•	Endpoint OS: macOS
	•	Endpoint Name: Stephens-MacBook-Pro
	•	Security Platform: Microsoft Defender for Endpoint (MDE)
	•	Portal: security.microsoft.com
	•	Tenant: SOC Lab (Microsoft Entra ID)
	•	Connectivity Method: Streamlined connectivity
	•	Deployment Method: Local onboarding script



## Tasks Completed



## 1. Microsoft Defender for Endpoint Configuration
	•	Navigated to Settings → Endpoints
	•	Confirmed Defender for Endpoint settings enabled
	•	Verified endpoint management options available

Purpose:
Ensures the tenant is capable of receiving endpoint telemetry and generating security events.



## 2. macOS Endpoint Onboarding
	•	Selected macOS as the operating system
	•	Chose Local Script deployment (1–10 devices)
	•	Downloaded onboarding package
	•	Executed onboarding script locally using Terminal
	sudo ./MicrosoftDefenderATPOnboardingMacOs.sh


Entered administrator credentials
	•	Script completed successfully and generated Defender configuration files

Purpose:
Registers the endpoint with Microsoft Defender cloud services.



## 3. Endpoint Registration Verification
	•	Confirmed device appeared in:
	•	Microsoft Defender Portal
	•	Device Inventory

Device status:
	•	No known risks
	•	Criticality: None
	•	Sense client active
	•	Defender engine reporting

Purpose:
Confirms successful EDR onboarding and cloud-to-endpoint communication.

⸻

## 4. Detection Testing (EICAR Simulation)
	•	Downloaded EICAR test file using terminal:
	curl -o ~/Downloads/eicar.com.txt https://secure.eicar.org/eicar.com.txt


File used strictly for detection validation
	•	No real malware involved

Purpose:
Simulates a benign malware signature to test detection pipelines.

⸻

## 5. Alert Validation & Monitoring
	•	Confirmed Defender agent activity
	•	Verified endpoint telemetry visibility
	•	Reviewed incident and alert sections
	•	Observed processing delay behavior (cloud correlation)

Note:
Alerts may take several minutes to correlate depending on tenant maturity and licensing state.



## Security Concepts Practiced
	•	Endpoint Detection & Response (EDR)
	•	macOS security onboarding
	•	Endpoint telemetry ingestion
	•	Cloud-based threat detection
	•	Incident generation workflow
	•	Detection testing methodology (EICAR)



## Outcome
	•	Endpoint successfully onboarded into Microsoft Defender for Endpoint
	•	Device reporting health and telemetry
	•	SOC visibility established
	•	Environment prepared for:
	•	Incident investigation
	•	Timeline analysis
	•	Advanced hunting (next phase)



## Key Takeaway

A SOC cannot investigate threats without endpoint visibility.
This phase establishes the foundation for:
	•	Alert triage
	•	Incident response
	•	Threat hunting
	•	Endpoint containment actions

This mirrors real enterprise SOC onboarding procedures.



## Analyst Reflection

Understanding endpoint onboarding is critical for SOC roles because:
	•	Misconfigured agents = blind spots
	•	Proper onboarding = reliable detections
	•	Verification ensures trust in alerts

