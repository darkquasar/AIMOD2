---
weight: 4
title: "Threat Hunt Mission Outcomes"
---

# Mission Findings & Outcomes

Here is the single most important thing people get wrong about threat hunting: thinking it is merely about "finding signs of compromise". If you haven't found suspicious activity, then the threat hunting effort has failed. But hunting is much more than that, threat hunting is about creating positive risk impact through discovery activities applied to attack vector disruption. It is about improving your organization's risk exposure by reducing its attack surface. The truth is, depending on the maturity of the target environment, 80% to 90% of the time you won't find "evil". But this doesn't mean you don't find "risk vectors". What security control issues you uncovered? Which visibility gaps you identified? What detection opportunities have you come across? What threat intel observables have you found? How did you expand the knowledge graph around an area or topic of relevance to your organisation? What new analytics have you created for the SOC or IR teams?

AIMOD2 defines 6 initial findings categories that cyber threat hunting teams can uncover during threat hunt missions. It is extremely rare that a threat hunt team would not be able to populate at least one of these finding categories.

- **visibility gaps**: are there data collection or parsing gaps that are preventing your organization from identifying potential threats?
- **security control issues**: have you found deficiencies in any of the security control layers that are meant to prevent cyber threats?
- **detection opportunities**: have you uncovered new ways of detecting cyber threats that should be turned into detectors, signatures or that might be useful for feature engineering in anomaly ML models?
- **hunt opportunities**: during the course of your hunt mission, have you discovered relevant hunt topics that have not been identified thus far?
- **suspicious security events**: this is the classic finding most threat hunt teams aim to identify, data patterns that point to suspicious activity which should be reported to SOC and IR teams for further investigation.
- **threat intelligence events of interest**: your hunt efforts may lead to expanding the knowledge graph around a tactic, technique or procedure, these new nodes could be observables or interesting information that can be passed on to threat intelligence teams or automation pipelines.