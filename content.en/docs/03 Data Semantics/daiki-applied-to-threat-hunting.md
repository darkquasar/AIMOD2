---
weight: 3
bookFlatSection: true
title: "Threat Hunt Mission Categories"
---

# Threat Hunt Mission Categories

## DAIKI applied to Threat Hunt Missions

If we keep in mind that cyber threat hunting is all about data science applied to the discovery and disruption of cyber threats, it makes sense that we can employ DAIKI to bring clarity to data analytic approaches during threat hunting. DAIKI can be used to differentiate between threat hunting mission types depending on the stage of the semantic chain where they operate. As such, there are four main hunt approaches based on the level of informational connectedness we are working with:

![daiki-hunt-types.excalidraw](/diagrams/daiki-hunt-types.excalidraw.png)

### Exploratory Data Analysis (EDA)

These mission types start at the very bottom of our data semantics chain, their purpose is to help us understand the "**what**": what data we are dealing with, is it structured or unstructured, what is the shape of the data, what are the basic components of it, what are the circumstances under which it was collected, what processes were involved in collecting the data, etc. Most hunt missions have some sort of exploratory data analysis phase. In this sense, threat hunting teams operate in a very similar way to data science teams.

*Example: imagine you want to understand whether an organization has logs that provide evidence for data exfiltration using Microsoft O365 Exchange suite*.

You would first need to understand how that organization is logging data overall (is there a SIEM, is there a data lake, are there any log retention policies, is logging enabled at the O365 tenancy level, etc.), then explore where that data could be, how is it being parsed and stored, what level of granularity is provided. Doing your research you may stumble upon the O365 Unified Audit Log. The UAL is a complex set of deeply nested log structures, you will have to figure out what each log type means, and how user activity is logged, what are the most prominent activity types vs the ones observed less often, etc. 

Depending on the complexity of the data at hand, and the techniques employed to analyze it, this endeavour could easily become a whole hunt mission in itself, in preparation for a second iteration of the mission where you will have a higher understanding of the data structures that will help you achieve mission objectives.

Once you've performed a first pass on your data, you will come out of it with more than just data, you will now start to build **knowledge** from that initial work and will be in a better position to transition your hunt mission to a **hypothesis based operation**.

There are many ways to explore your data. Initially, AIMOD2 considers that the two subtypes of EDA are: **baselining** and **machine learning assisted modelling** (e.g. unsupervised clustering algorithms like k-means). We will define these subtypes in later versions of AIMOD2.

> **Define Process**: threat hunting teams should define a process for the statistical, visual, machine learning assisted and generic manual examination of data for EDA hunt missions. This process shouldn't be exhaustive and extremely detailed, but it should at a bare minimum outline the different approaches that are most useful during data baselining and the best ways to achieve that according to the available technologies in the organization.

### Hypothesis based Operations (HBO)

When we possess some level of context around the data we are working with, but we lack enough situational awareness to integrate this data into threat actor profiles and threat likelihood, we need to focus our hunting efforts based on low to medium confidence hypothetical scenarios.

To drive a hypothesis based scenario, we should have already answered the "what" of data. We have now a more holistic understanding of the data at hand. Baseline, statistical, clustering and manual examination techniques have given us a more consistent idea of the data.

At this point, we are better positioned to formulate a hypothesis that we have good chances at answering since we have some basic level understanding of the underlying data structures.

These hunt missions involve formulating and testing hypotheses or theories based on adversarial tradecraft information collected from  various data sources. Central to the success of hypothesis based hunts is the concept *situational awareness*:

- industry knowledge to understand which threats are most likely to target your business
- infrastructure awareness, to understand your own strengths and weaknesses, e.g. are there unpatched servers in some network segments? which systems have control exceptions? what is the status of cloud and container telemetry?
- security control's awareness: what technologies have been deployed in our environment, who owns the different control stacks?
- risk management knowledge: what is the risk framework in the organization? which teams manage it? how is risk reported and how does the risk matrix look like?
- threat intelligence, to understand the threat landscape and which threat actors are relevant to your business depending on geopolitical and tradecraft factors
- technological landscape, to understand which new or emerging technologies can challenge your cyber defense paradigm

The data above feeds these hunt types, and can be collated at different levels by the same or different teams in the organization. This data needs to be synthesized by the threat hunting team following either heuristic or explicit qualifying rules that help highlight the most relevant topics to focus on.

There are many ways to execute hypothesis based operations. Initially, AIMOD2 considers that the two subtypes of HBO are: **hypothesis driven hunts** and **attack vector discovery**. We will define these subtypes in more detail in later versions of AIMOD2. However, at a high level we can say that:

- **Hypothesis Driven Hunts**. They employ heuristics and basic knowledge of the threat landscape to craft credible attack scenarios that are worth hunting for. We are not yet at the stage of knowledge and as such we lack the informational processing power that a threat intelligence team or specialized third party can provide.
- **Attack Vector Discovery**. Closely linked to attack path modelling and controlled attack paths (which I have touched on [here](https://threathunterz.com/posts/threat-hunting/the-way-of-the-intercepting-fist-part-1/) and [here](https://threathunterz.com/posts/threat-hunting/the-way-of-the-intercepting-fist-part-1/#fn:4)), attack vector discovery is a hypothesis driven mission where our goal is to identify early signs of offensive operations that could impact an organization. An example of this is hunting for phishing campaigns before they are launched (via new domain registration analysis, cloned site identification, DOM hash similarities, etc.) or malware strains that have been inadvertently leaked by cyber criminals which can tip us off on new malware designed to target our business. AVD missions capitalize heavily on the concept that cyber criminals also make OpSec mistakes. It is our job to exploit those OpSec mistakes to our advantage.

> **Define Process**: threat hunting teams should define a process for information collection, prioritization and synthesis, so that it can be turned into contextualized knowledge and actionable insight.

> **NOTE**: to be clear, all threat hunt missions are one way or another subtypes of hypothesis based operations. There is a primordial underlying hypothesis to any hunt operation which is *assuming breach*. But beyond this, threat hunting is about finding the unknown, with the presumption that it is *knowable* by leveraging data analysis and other techniques like deception.

### Threat Informed Operations (TIO)

This is the domain where actionable threat intelligence is essential. Threat intel usually represents higher level data that has been processed into knowledge or insight. When in this stage, our threat hunting efforts can take a higher ROI approach since a lot of the relevancy of the information at hand has been already established by threat intel functions (which can be the same or a different team to that where threat hunters sit).

AIMOD2 defines three basic subtypes of TIO:

- **Threat Intelligence Hunts**. Also known as "Tactical Intel Hunts", these are agile missions carried out by the threat hunting team to break down threat reports (whether from CTI team or other sources like red team engagements) and drive an active assessment of threat indicators in our digital landscape. This is achieved by obtaining relevant threat indicators (both behavioural and atomic), performing searches in our digital infrastructure for any matches and finally enriching our Threat Intel Platform with any expanded knowledge obtained through this assessment.
- **Attack Modelling**. A subset of threat modelling, what we are interested in here is understanding the attack chains and relationships between TTPs. Attack modelling can only happen in the semantic level of knowledge, since we require distilled threat intel and practical knowledge of plausible attack paths (for example, via red team engagements or pentest reports)
- **Deceptive Ops**. Threat Hunting is the driver for cyber deception. As part of a thoughtful cyber deception strategy, these missions will help plan the engagement aspects of the strategy, following industry best practices like [MITRE ENGAGE](https://engage.mitre.org/). These missions will also aim at deploying decoys and lures, as well as crafting specialized decoy systems based off available threat intelligence and attack path models.

### Disruptive Purple Operations (DPO)

It is extremely difficult to truthfully commence a threat hunt effort at the epistemological level of insight. Insight implies embodied knowledge that has been put to practice and internalized into behaviours (these behaviours in turn inform our security controls and risk profile).

However, joint purple operations achieve this goal by combining the insight from red teams, who can craft real attack paths into the organization's crown jewels, with the defensive knowledge from blue teams.