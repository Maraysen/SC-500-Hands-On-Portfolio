# Lab 08 – Microsoft Defender for Cloud Security Posture

## Objective

Review Microsoft Defender for Cloud posture-management capabilities and confirm that Foundational CSPM is active for the Azure subscription.

## Resources Used

- Microsoft Defender for Cloud
- Foundational CSPM
- Secure Score
- Security recommendations
- Azure subscription

## What I Reviewed

1. Opened Microsoft Defender for Cloud.
2. Reviewed the Defender plans for the `SC-500 Lab` subscription.
3. Confirmed that Foundational CSPM was active.
4. Confirmed free pricing and full monitoring coverage.
5. Kept Defender CSPM and all paid workload-protection plans disabled.
6. Opened the Recommendations page.
7. Confirmed that all recommendation-status filters were selected.

## Defender for Cloud Configuration

- **Subscription:** `SC-500 Lab`
- **Foundational CSPM:** Active
- **Pricing:** Free
- **Monitoring coverage:** Full
- **Defender CSPM:** Disabled
- **Paid workload-protection plans:** Disabled

## Security Posture Concept

Microsoft Defender for Cloud evaluates Azure resources against security controls and can provide:

- Secure Score
- Security recommendations
- Resource health findings
- Cloud security posture insights

Foundational CSPM provides the basic posture-management capabilities without requiring the paid Defender CSPM plan.

## Current Assessment Status

At the time of this lab, Defender for Cloud had not yet produced recommendations for the newly created Azure resources.

The Recommendations page showed no findings even though all status filters were selected.

Because no recommendation was available, no remediation was performed during this lab.

## Screenshots

### 1. Foundational CSPM Enabled

![Foundational CSPM Enabled](screenshots/01-foundational-cspm-enabled.png)

### 2. No Recommendations Yet

![No Recommendations Yet](screenshots/02-no-recommendations-yet.png)

## Outcome

Foundational CSPM was confirmed as active with free full monitoring coverage.

The subscription was onboarded to Microsoft Defender for Cloud, but no security recommendations were available at the time of documentation.
