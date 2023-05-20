---
weight: 1
bookFlatSection: true
title: "External Attack Vector Discovery"
---

> **NOTE**: We will define all hunt mission subtypes mentioned above under "DAIKI Applied to Threat Hunt Missions" in future versions of AIMOD2, for the moment, we provide the definition for External Attack Vector Discovery, which is one way to interpret Attack Vector Discovery hunts, a subtype of Threat Informed Operations (TIO).

# External Attack Vector Discovery

Standard threat hunting activities focus usually on internal attack vectors, coming from a stance of "assumed breach", and look for threat indicators (atomic, behavioural o anomaly based) within the organization's systems. Contrary to this, External Attack Vector Discovery are threat hunt missions that attempt to discover external threats before they produce significant impact in our organization. Instead of assuming breach, we start by assuming intention on behalf of the threat actors, which means we assume threat actors will first mount operational infrastructure to carry on their targeted campaigns, as well as actively performing reconnaissance on our perimeter. This service has three goals:

The standard approach to threat hunting typically focuses on internal attack vectors, adopting an "assumed breach" stance to identify threat indicators (atomic, behavioural, or anomaly-based) within an organization's systems. Contrary to this, External Attack Vector Discovery represents a proactive approach that aims to uncover external threats before they cause perceivable harm to an organization. Rather than *assuming breach*, this approach **assumes intention** on behalf of threat actors and centers efforts around two important aspects of adversarial operations:

1. cyber criminals do make OpSec mistakes, their operators are not always equally skilled and the operational procedures they follow might also contain issues, we aim to exploit these OpSec mistakes.
2. we assume threat actors will first mount operational infrastructure to carry on their targeted campaigns, as well as to actively perform reconnaissance on our perimeter.

It's in the early stages of adversarial operation development that we aim to **intercept and disrupt** their efforts.

The primary objectives of these hunt missions are:

- seek to proactively identify threats outside our perimeter network, that are highly likely targeting the organization's clients and employees
- attempt to intercept phishing campaigns and malware strains that are building momentum, with the aim of targeting the organization's clients and employees
- exploit threat actor operational security (OpSec) mistakes that expose adversarial intention and infrastructure

To accomplish these goals, we will leverage tools and services that provide insight into what is happening outside of the trusted digital surface, as well as traditional SIEM and EDR telemetry.
