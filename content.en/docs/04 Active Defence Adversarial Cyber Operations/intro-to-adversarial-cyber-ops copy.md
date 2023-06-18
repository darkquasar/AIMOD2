---
weight: 1
bookFlatSection: true
title: "Intro to ADACOP"
---

{{% resizeimage src="./diagrams/adacop-v2.png" width="400" height="400" position="center" %}}

# 🧮 Framework Design Principles

ADACOP is meant to be used as a loosely coupled set of practical domains that help describe the tactical activities of cyber defence operations. A tactical framework for cyber defence operations should be concerned with categories of actions that help describe engagement environments that provide guidance for a practical course of action.

The design principles that I attempted to follow when constructing this framework are:

The design principles that I attempted to follow when constructing this framework are:

- **Abstraction instead of Concretion**. The framework needs not be concerned with the particularities of a concrete implementation. By doing this, it remains flexible and adaptable to multiple application approaches.

- **Descriptive instead of Prescriptive**. The framework does not aim to *prescribe* what to do, and in which order. Rather, it seeks to provide a descriptive map to help organizations, teams and individuals understand what aspects of a tactical maneuver they are defending against or leveraging to their advantage.

- **Polyvalent instead of Monofunctional**. The framework can be used to *understand defensive cyber operations as much as offensive ones*. This means that the framework can be employed to describe adversarial operations whether from the point of view of the attacker, the defender, or both at the same time. In doing this, I'm not trying to aid threat actors, I'm trying to question the naivety by which cyber defence ops merely looks at the protective side, overlooking realistic offensive security scenarios.

- **Simple instead of Complicated**. The framework aims to be as simple as possible (but not simpler, and also not "simplistic") and avoid overdetermining its potential applications by over-constraining its own structure. We want to facilitate the possibility of emergence, and for this, we need **enabling constrains**, as Cynefin would call them.

- **Tactical instead of Procedural**. The framework should describe **tactical environments** and the high level tactics that are most useful and mostly associated with those environments. It should not worry about the techniques or procedures that derive from the different tactics or how they are operationalized.

- **Fractality instead of Uniformity (or Monolith)**. The framework is not supposed to represent a whole, complete model. Instead, it follows the complexity attribute of self-similarity or fractality. Each domain in the framework can virtually replicate the same (or similar) structure at a higher or lower level. For example, when you are in the "Defence" domain, you also have a Design phase, where you configure your protection space and assets, a Disruptive aspect, whereby your defences act as a disruption of the enemy's forces, a Discovery aspect, by which your defences establish a new lookout zone and expand territorial limits, and a Defence aspect itself, where you protect again what its already been protected, **in a twofold self-reflective move that makes concepts like defence-in-depth** (multi-layer protection) possible. The same applies to domains like Discovery, whereby a threat hunting party wouldn't act recklessly without equipping themselves with the right protections and adopting defensive principles ("don't run malware on production systems", etc.) as well as disruptive practices (e.g. cyber deception for adversarial entrapment), etc.

# References

- Cynefin, a sense making framework. Cynefin is a framework for understanding what kind of problem space you are in to guide decisions-making and action. It was created by David Snowden and takes its name from the Welsh word meaning "the place of your multiple belongings.", https://cynefin.io/wiki/Cynefin
- Alex S. Wilner (2011) Deterring the Undeterrable: Coercion, Denial, and Delegitimization in Counterterrorism, The Journal of Strategic Studies, 34:1, 3-37, DOI: 10.1080/01402390.2011.541760, https://doi.org/10.1080/01402390.2011.541760
- MITRE ENGAGE, a framework for planning and discussing adversary engagement operations, https://engage.mitre.org/
- MITRE ATT&CK, a globally-accessible knowledge base of adversary tactics and techniques based on real-world observations, https://attack.mitre.org/
- MITRE ATTACK FLOW, a data model with supporting tooling and examples for describing sequences of adversary behaviours. Attack flows help defenders understand, share, and make threat-informed decisions based on the sequence of actions in a cyber-attack., https://ctid.mitre-engenuity.org/our-work/attack-flow/
- MITRE D3FEND, a knowledge graph of cybersecurity countermeasures, https://d3fend.mitre.org/
- Cyber Kill Chain, a model for identification and prevention of cyber intrusions activity, https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html
- NIST, a framework that offers a set of guidelines and best practices for managing cybersecurity risks in organizations, the framework provides a common language and a structured approach for organizations to identify, assess, and manage cybersecurity risks in a consistent and repeatable way, https://www.nist.gov/cyberframework
- Cyber Threat Framework, the Cyber Threat Framework was developed by the US Government to enable consistent characterization and categorization of cyber threat events, and to identify trends or changes in the activities of cyber adversaries, https://www.dni.gov/index.php/cyber-threat-framework