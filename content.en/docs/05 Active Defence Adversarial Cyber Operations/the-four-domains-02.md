---
weight: 3
bookFlatSection: true
title: "Tactical Domains: Design & Defence"
---

{{% resizeimage src="/diagrams/ADACOP-Des&Def.png" width="400" height="400" position="center" %}}

# Defend

> *Warlords who have mastered defence, attack from hidden places and assure their own success. They know when, where, and how to make an attack while defending their positions at the same time. These men of high perception rely on obstacles they have set up for the enemy. In understanding the attack mentality, they never permit the enemy to know where the attack is coming from*. (Sun Tzu, The Art of War, Book IV)

The Defence domain is focused on a set of tactics aimed at protecting the most valuable assets and resources of the defender. A strong defence can deter an attack, as the potential costs and risks of an attack may outweigh the potential benefits. Our defences should seek to exploit any weaknesses or vulnerabilities of the attacker, and use them to our own advantage, while maintaining a strong and cohesive unit with good communication and coordination among members.

## Protect

> *The different measures suited to the nine varieties of ground; the expediency of aggressive or defensive tactics; and the fundamental laws of human nature: these are things that must most certainly be studied.* (Sun Tzu, The Art of War, Book XI)

System protection is one of the classic and fundamental concepts in cybersecurity. It refers to ways of making systems and networks more resistant to digital attacks. Protection is based on implementing measures that ensure our systems safeguard all the components of the CIA triad (confidentiality, integrity and availability).

At the heart of the protection tactic, there are two main activities: attack **prevention** and **system hardening**.

*Attack prevention* involves implementing measures to prevent unauthorized access to a system or network, and to protect against attacks that may exploit vulnerabilities in the system. This can include installing and maintaining firewalls, IDS/IPS, EDR, AV, encryption, etc. 

*System hardening*, on the other hand, refers to the process of making it more secure by reducing its vulnerability surface. This is typically done by reducing the number of functions the system performs, as a system that performs fewer functions has a smaller attack surface. To harden a system, several controls are applied like changing default passwords, removing unnecessary software, disabling unnecessary services and protocols, applying security patches, etc. A classic hardening framework is provided by the Center for Internet Security (CIS)[^1]. Essentially, the goal of hardening is to reduce the number of potential ways an attacker could compromise the system.

## Detect

> *In the midst of chaos, there is also opportunity.* (Sun Tzu, The Art of War, Book IV)

Detection refers to the process of identifying the presence of a security threat or breach in computer networks. This typically involves using various tools and techniques to monitor systems by collecting remote data (telemetry), analyzing this data, and looking for signs of unusual activity that might indicate an attempted attack or compromise. The goal of detection is to identify threats as quickly as possible, so that appropriate countermeasures can be taken to prevent or mitigate the potential damage.

Detection is comprised of three main components:

- **Sensor**: the device or system that is used to collect data locally or remotely (telemetry) on target devices. The term "sensor" designates an abstract device that can take any shape like an EDR (a local system sensor that hooks on to system calls and gathers multiple types of data), IDS (sensing and collecting data from network communications), etc. Detection leverages tactics from the Discovery domain to achieve this goal. E.g. tactics like Exploration, to survey the internal infrastructure and understand data collection coverage and gaps; Collection, to effectively gather required data and centralize it in data lakes or SIEMs.
- **Signal (Data)**: the information that is gathered by the sensor and used to identify the presence of threats. This information is usually pre-processed and refined before it arrives at the next stage.
- **Algorithm**: the process that is used to analyze the signal and determine whether it meets the threshold for detection. The algorithm might be a simple rule-based system, or a more complex statistical, behavioural or risk-based model. Machine Learning algorithms that utilize UEBA and anomaly detection to find suspicious signals are an example of the latter.

When combined, these components produce a **detector**. A detector is an artifact that implements some type of logic (algorithm) based on data collected by sensors that aims to detect a specific type of suspicious activity. Detectors define different thresholds (trigger conditions) depending on the type of threat and telemetry available. 

## Respond

Entities in the _cybersphere_ require constant vigilance and protection to build a layer of resilience against potential attacks in order to mitigate damage and reduce their future exposure. As such, **Cyber Incident Response provides tactical and operational capabilities** to defend against cyber attacks in the most effective manner.

In the context of the digital _cybersphere_, we can define Response as

> a series of organized actions that are triggered due to a disruption that poses a threat to business operations.

This disruption does not need to cause an immediate damage to the business’ continuity but _it carries the potential to do so_. Cyber Response is the process of **coordinating effort** towards the identification, containment, eviction and remediation of a cyber threat, with the goal to minimize organizational damage and reduce its future occurrence. The purpose of Response is the same as any other Cybersecurity tactic: to manage risk.

Response usually takes the shape of "Incident Response" as a function, but since our framework does not define functions, teams or departments per se, response tactical activities refer to any type of reaction to a disruption in the connective tissue of our digital assets or services. In this sense any planned activity that can be used in a defensive context qualifies as a response tactic: disaster recovery plans, business continuity plans, emergency response plans, risk management plans, etc.

# Design

> *Now the general who wins a battle makes many calculations in his temple ere the battle is fought. The general who loses a battle makes but few calculations beforehand*. (Sun Tzu, Book I)

The Design domain implements tactics to aid in the process of creating a plan or solution to a problem or need. It involves identifying the needs or requirements for a product, service, or system, and developing an approach for how to meet those needs.

In order to design something effectively, we need to have a clear understanding of the problem or need that we are trying to address, as well as the materials, resources, and constraints that we have to work with. Designing usually requires the ability to think creatively and come up with innovative ideas for how to solve the problem or meet the need.

Effective communication and dissemination are important components of the design process. Communication is necessary in order to clearly articulate the problem or need that you are trying to address, as well as to gather input and feedback from others who may be involved in the design process. Thus dissemination is a necessary part of the design process, in order to share prospective or final outcomes with relevant stakeholders.

## Analyse

Analysis is the process of breaking something down into its component parts in order to gain a better understanding of it. It often involves examining and evaluating data or information in order to identify patterns, trends, and relationships. The word comes from the Ancient Greek ἀνάλυσις (_analysis_, "breaking-up", "untying;" from _ana-_ "up, throughout" and _lysis_ "loosening").

Analysis can be qualitative, in which the focus is on understanding and interpreting the meaning of data or information, or quantitative, in which the focus is on measuring and evaluating data or information using statistical or mathematical techniques. 

Analytical tactics don't make distinctions between "analysis" and "synthesis" as opposite activities but rather it comprises both as complementary activities.

In the context of this framework, analysis is any activity performed to identify, reason and solve for a given problem.

## Plan

> *... a power of estimating the adversary, of controlling the forces of victory, and of shrewdly calculating difficulties, dangers and distances, constitutes the test of a great general.* (Sun Tzu, Book X)

Planning involves considering the actions needed to achieve a particular goal and anticipating potential outcomes. It relies on the ability to imagine and formulate alternative futures (a capability otherwise known as foresight, the fundamental capacity for mental time travel), and is thought to have played a key role in human evolution.

From a neurological perspective, planning involves a number of brain functions including goal setting, decision making, and problem solving. It requires the activation of certain areas of the brain such as the prefrontal cortex, which is involved in higher cognitive functions such as planning and decision making, and the basal ganglia, which is involved in the selection and initiation of actions.

Planning also involves the coordination of various brain regions and cognitive processes, such as attention, memory, and language, to generate and evaluate potential courses of action.

## Model

Design is also the process of analysing gathered data and developing models, schemas, frameworks and diagrams that help us make sense of the data that has been collected via exploration. In this phase, we must transition from data to information.

Data is raw, unprocessed facts and figures, while information is data that has been processed and organized in a way that is meaningful and useful. In order to go from data to information, you typically need to perform some kind of modelling and analysis. The process of going from data to information is not just about finding answers, but about creating new questions and possibilities.

Modelling allows us to identify patterns and relationships within the data that might not be immediately obvious. It can also help us make predictions and forecasts. By building a model of how a system is likely to behave, we can make educated guesses about what might happen in the future. Modelling information can be a powerful tool for gaining insights and understanding complex systems.

In the cyber security world, some examples of modelling activity are: 

- Analysing threat intel data to uncover patterns that can be ascribed to a particular threat actor
- Threat Modelling of new systems or apps, to understand how they could be compromised
- Attack Path Modelling, using tools like [MITRE Attack Flow](https://ctid.mitre-engenuity.org/our-work/attack-flow/), to understand sets of combined attacker behaviours.

[^1]: As per [Microsoft Learn](https://learn.microsoft.com/en-us/compliance/regulatory/offering-cis-benchmark): "[CIS benchmarks](https://www.cisecurity.org/cis-benchmarks/) are configuration baselines and best practices for securely configuring a system. Each of the guidance recommendations references one or more [CIS controls](https://www.cisecurity.org/controls/) that were developed to help organizations improve their cyberdefense capabilities. CIS controls map to many established standards and regulatory frameworks, including the NIST Cybersecurity Framework (CSF) and NIST SP 800-53, the ISO 27000 series of standards, PCI DSS, HIPAA, and others."