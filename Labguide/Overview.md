# Threat Protection with XDR

## Overview

Extended Detection and Response (XDR) is a comprehensive cybersecurity solution that offers advanced threat protection by integrating and correlating security data across various sources and security layers within an organization's infrastructure. XDR is designed to detect, investigate, respond to, and remediate cyber threats more effectively than traditional security solutions.

### Key features of Threat Protection with XDR

- Integration of Security Tools: XDR integrates multiple security tools and technologies such as endpoint security (EPP/EDR), network security, email security, cloud security, and more into a unified platform.
- Centralized Visibility and Analytics: XDR collects and aggregates data from diverse security sources, creating a comprehensive and unified view of the organization's security posture.
- Automated Threat Detection: XDR leverages its analytical capabilities to detect sophisticated threats, including zero-day exploits, malware, ransomware, phishing attacks, and other advanced threats that might evade traditional security measures.
- Contextualized Insights: XDR provides contextualized insights into detected threats, offering detailed information about the attack chain, affected systems, and the severity of the threat.
- Response and Remediation: When a threat is identified, XDR facilitates a swift response by automating threat containment, isolation, and remediation actions.

## Sandbox Scenario
Contoso is a global organization with a complex IT infrastructure that includes a combination of on-premises data centers and cloud-based resources. They are looking to enhance their security posture by deploying Azure Sentinel, Microsoft's cloud-native security information and event management (SIEM) and security orchestration automation and response (SOAR) solution. Additionally, Contoso aims to onboard its cloud resources and servers to Azure Sentinel to gain better visibility and proactive threat detection and response capabilities.

By implementing a robust log analytics and threat detection program, Contoso aims to proactively identify and mitigate threats, reduce the risk of security breaches, and maintain a strong security posture in an ever-evolving threat landscape. This approach will enable Contoso to stay ahead of potential threats and protect its digital assets effectively.

## Using this Sandbox

In this sandbox environment, You'll have access to a predeployed environment with an active Azure subscription, a tenant, and a Microsoft 365 E5 license assigned to the user. 

Using this environment, You'll be able to explore complete features and offerings offered by Microsoft Sentinel including XDR protection.

The lab scenarios are given as reference material to assist you in getting started with the exploration. You are encouraged to explore Microsoft Purview further based on your interests and preferences.

## Contents:

### Threat Protection using XDR

- Prerequisites
- Lab 01 - Review and explore sentinel workspace
- Lab 02 - Create queries for Microsoft Sentinel using Kusto Query Language (KQL)
- Lab 03 - Conduct attacks
- Lab 04 - Create workbooks
- Lab 05 - Use Repositories in Microsoft Sentinel
- Lab 06 - Understand Detection Modeling
- Lab 07 - Create Detections
- Lab 08 - Investigate an Incident
- Lab 09 - Threat Hunting using Notebooks with Microsoft Sentinel
- Lab 10 - Mitigate threats using Microsoft Defender for Cloud
- Lab 11 - Integrate Logic App with Threat Protection and XDR

### Azure services and related products

- Log Analytics Workspace
- Microsoft Defender for Cloud
- Microsoft Defender for Endpoint
- Microsoft Entra ID
- Microsoft Sentinel
