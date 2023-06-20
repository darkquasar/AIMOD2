---
weight: 3
title: "CAPEO: Threat Hunt Mission Structure"
---

# CAPEO: Collect - Analyize - Plan - Execute - Outcomes

AIMOD2 defines a set of phases for all its mission operations called CAPEO: Collection, Analysis, Planning, Execution and Outcomes.

## Collect

Ensure that threat Intel is collected into a Threat Intelligence Platform (TIP) and that proper communication channels exist to make it available and highlight important or relevant cyber threats to stakeholders.

## Analyze

The analysis phase involves a series of tasks required to perform a pre-assessment and high level examination of the hunt mission. It is not meant to perform a complete investigation on the topic.

### Initial Research

Conduct initial Research In the future Cyber Threat Hunt will formulate a systematic approach to conduct initial research on a particular topic, however for the time being the process will be based on security analysis experience, OSINT, and acquired research techniques.

At a bare minimum, the research process should capture what the current literature says about a particular tactic, technique or procedure. This involves reference material like online articles, existing documentation, code repositories, etc.

### Perform Feasibility Assessment

Evaluating the practicality and viability of a proposed threat hunt topic.  This involves considering different factors like data availability, quality of available information, skillsets, resource constraints and timelines, etc. In the initial stages of threat hunt maturity, the process will be more based in heuristics and relevancy of threats to an organization as determined by impacted Crown Jewels, major vulnerabilities or emergent threats. There is no systematic approach in the early stages of threat hunt maturity.

> **Define Process**. Threat Hunting Teams should develop threat hunt prioritization model that formulates a systematic approach for feasibility assessment to determine whether a topic qualifies for a hunt mission

### Business and Technical Owner identification

During the analysis phase, it is important to identify documentation related to the asset, service, or application's business and technical points of contact. This information could prove useful if there are questions regarding those areas which are pertinent to the hunt scoping and qualification process.

### Identify requirements to engage other teams

During certain threat hunt missions, it may be necessary to collaborate with other teams, both within and outside the cyber security vertical, to achieve the desired goals. To ensure successful collaboration, it is important to identify and assess these requirements early in the threat hunt phase, determining the level of involvement needed from other teams and the deliverables expected. If engaging other teams is necessary to achieve mission objectives, the analysis phase should carefully evaluate and document these requirements.

## Plan

### Designate Mission Lead

The threat hunt team will designate a Mission Lead which will be in charge of the end to end delivery of the hunt mission. 

### Evaluate and define Scope

Based on the results of the Analysis phase, a scope for the hunt operation must be determined:

- *Determine Tactical Objectives*. Objectives represent the targets of our mission that must be accomplished to achieve our goals. These tactical objectives will serve as high-level topics whose understanding the hunt party will develop through further research, investigation, or scouting.
- *Allocate expected time for hunt duration end-to-end*. This serves as a basis to understand sprint requirements for the completion of the hunt. Additionally, it will be captured later as two different metrics *"Total Hunt Duration"*, which represents the total duration from initial research to releasing reports, and, *"Execution Phase Duration"* (usually no more than 75% of Total Hunt Duration, so that a quarter of the total hunt duration can be allocated to report writing).

### Determine Hunting Squad Composition

- It is the task of the Mission Lead to bring in the required resources to accomplish mission objectives, in this case, to designate one or more threat hunters that will become part of the hunting squad.
- Members should be contacted and express their willingness to participate.
- Once the above is completed, a Threat Hunting Squad would have formed.

### Setup Squad Communication Channels

- The Mission Lead should stand up the appropriate comms channels according to organizational best practice. These channels should serve the purpose of quick day-to-day information sharing and should be recognized as central channels for mission coordination.
- The hunt operation can be given a code name to make things a bit more fun or interesting, but it still needs to fit within a nomenclature rule. Example: *"EAVD01 - Barracuda Muffin" or "EAVD01 - Phishing Campaign Interception"* (where EAVD stands for External Attack Vector Discovery).
- Comms regarding specifics of the hunt operation should happen within this chat channel. Other members can be invited on a need to know basis. 

### Formalize Action Plan in Agile/Scrum

- Layout the action plan based on the tactical objectives
- Structure the plan according to your Agile or sprint management software

## Execute

### Discovery

Exploration is an essential activity of Cyber Defence that is linked to the Discovery Tactical Domain. During our exploratory phase we aim to perform the following activities: 

- *data source discovery*: developing an understanding of the data sources relevant to the hunt operation that can yield the best results, where is the data, what are the data types and models, etc. Knowledge about this can be further developed throughout the duration of the whole hunt. 
- *identify relevant stakeholders*: people that can provide important information or support regarding our hunt topic: business owners, technical support teams, etc.
- *find available infrastructure knowledge*: architecture maps, knowledge base articles, policies, procedures, etc. that help provide insight into the people, process and technology that are relevant to our hunt efforts.
- *investigate previous security data*: any relevant incident tickets, Pentests/Red Team reports, Risks or related information that may provide insight into previous security incidents, vulnerabilities or overall risks.
- *interrogate data*: run systematic queries that help you advance in the achievement of mission objectives.
- *data collection*. Data Collection is another essential activity of the [Discovery Tactical Domain](https://threathunterz.com/posts/threat-hunting/the-way-of-the-intercepting-fist-part-3/#discover). Data collection is an ongoing activity that informs all our hunt efforts. Some activities to consider are:
	- document temporary findings on the go in your CRM or ticketing system
	- gather available evidence from insightful data queries and be sure to flag them for Playbook development and Battlefield Intel.

### Disruption

Disruption activities are an essential part of the [Disruption Tactical Domain](https://threathunterz.com/posts/threat-hunting/the-way-of-the-intercepting-fist-part-3/#disruption). The term *"disruption"* refers to intentionally intercepting cyber adversaries, with two primary tactical purposes: *interception and coercion*.

- intercept anomalous behaviour by applying data analytic techniques to distinguish signal from noise
- escalate suspicious activity (SEOI) so that it can be quickly actioned by downstream teams as per our Incident Response Plan, follow escalation process.
- raise urgent visibility gaps: if there is a log outage affecting our ability to hunt or detect adversarial operations, these need to be raised as per visibility gap process.
- isolate endpoints or accounts: in case active threat activity is observed unfolding and assets are identified, liaise immediately with your DFIR team to evaluate threat containment techniques
 
## Outcomes

Once a threat hunt is completed, there are some outcomes that are produced by the hunt. During the post-hunt phase, these outcomes are captured in *three different artifacts*:

1. **Threat Hunt Playbook**: a combination of a research document and a code recipe. The Playbook is a data analytics story. The best model for this are Jupyter Notebooks applied to data science research. The Threat Hunt Playbook is an iterative artefact that is improved with each iteration of the same hunt mission. The playbook does not care about metrics.
2. **Threat Hunt Report**: the report is a snapshot in time of the results in an iteration of a hunt mission. The report is the container for metrics, here is where we should capture the different operational metrics for the mission.
3. **Comms**: once the report and the playbook have been created, the threat hunt mission needs to be communicated as a story to the target audience. Comms are normally distributed as an email or newsletter. They should at a bare minimum convey the background of the hunt mission, i.e., what motivated it, and a summary of the findings. The more we tell a story with our findings, the more memorable they become, even when there are no security incidents uncovered as a result of the hunt.

In the **Mission Findings & Outcomes** section we cover what are the actual findings that should be captured and communicated as a result of a threat hunt mission.

> **AUDIENCE**: it is important to identify the stakeholders that should become your target audience. They will be the main recipients of your hunt discoveries. Aim to identify stakeholders that can convert your findings into actionable information, so that your findings will help improve the overall security posture of your organization.
