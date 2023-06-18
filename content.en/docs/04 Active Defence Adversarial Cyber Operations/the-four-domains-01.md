---
weight: 2
bookFlatSection: true
title: "Tactical Domains: Discovery & Disruption"
---

## Discovery

> *By discovering the enemy's dispositions and remaining invisible ourselves, we can keep our forces concentrated, while the enemy's must be divided.* (Sun Tzu, The Art of War, Book VI)

Discovery is the domain where information is continuously synthesized into different layers of abstraction to help develop context awareness and insight. The discovery domain is characterized by the simultaneous scouting of known and unchartered territory. Understanding your digital infrastructure, attack surface or external threat landscape is a never ending effort that seeks to survey the technological capabilities, understand weaknesses, secret passages, avenues of exploitation, strengths, natural tendencies, and any traces of adversarial incursion. 

### Explore

> *We are not fit to lead an army on the march unless we are familiar with the face of the country—its mountains and forests, its pitfalls and precipices, its marshes and swamps.* (Sun Tzu, The Art of War, Book VII)

Exploration refers to the act of searching for and discovering new or unknown things. During exploratory activities, we may have little to no knowledge of the terrain we are venturing into. Our aim is seeking to gain a deeper understanding of the environment that surrounds us and our adversaries. From the point of view of cyber warfare, exploration involves reconnaissance and terrain mapping, the technical process of acquiring information and intelligence about the threat landscape. Exploration may or may not involve collecting data, but data collection is essential to progress to higher levels of information refinement and insight.

### Collect

Data collection is the process of gathering, classifying and measuring information on variables of interest, ideally in a systematic fashion, to enable us to answer research questions, test hypotheses, and evaluate outcomes. The data collection process may involve the collection of raw data, as well as the processing, preparation, and analysis of data, in order to make it usable for research purposes. Data collection in cyber defence may encompass activities such as placing sensors in our infrastructure, gathering raw telemetry from digital systems (servers, endpoints, OT devices, etc.), available threat intelligence, internal asset database (CMDB), etc.

The data collection phase is also applicable to GRC (Governance, Risk and Compliance) procedures, like gathering requirements from public policies or stakeholders. Ultimately, the goal of data collection is to obtain accurate and reliable data that can be turned into information and used to answer research questions and inform decision-making. In order to go from data to information, data must be collected and organized in a way that allows it to be analysed and interpreted.

### Disseminate

Dissemination refers to the act of spreading or distributing information or ideas to a wider group of people or audience. It can refer to the distribution of information through various channels, such as through the media, through communication networks, or through public speaking and presentations. Dissemination can be used to share research findings, news, cultural events, or any other type of information with a larger group of people.

> **Note**: *in a future version of the framework Disseminate may transform into Communicate as a more broad and complex activity.*

## Disruption

> *The supreme art of war is to subdue the enemy without fighting. Thus the highest form of generalship is to balk the enemy's plans; the next best is to prevent the junction of the enemy's forces. The third is to attack the enemy's army in the field before it has formed into order of battle. The fourth is to hurl your army on a single point in the enemy's line, and the fifth is to roll up his whole line from one end to the other. When he is in disarray, your victory will be complete*. (Sun Tzu, The Art of War, Book 3)

Disruption is key to cyber operations. The goal of disruption is to break the patterns that the adversary has memorized, either through purposeful training or repetition arising from environmental constraints. These patterns refer to any aspect of the adversary's cultural (e.g. the time of the day they operate based on their geographical location and usual work hours in that culture), biological, behavioural or digital (e.g. their botnet infrastructure deployment) disposition. Disruption is the act of using maneuvers to destabilize the opponent to a degree that dismembers their formation leading to imminent defeat. In cyber operations, disruption takes place when the adversary's capabilities are so impaired that they are forced into a zone of confusion which imposes a high cost of operations whilst attempting to get back into balance. This state of confusion opens a window of opportunity to achieve mission objectives.

The Tao Teh Ching offers us one of the most beautiful, powerful, enlightened and insightful teachings of all time when it says *"He who conquers others is strong; He who conquers himself is The Strength"*. You may as well re-write it by saying *He who conquers himself is The Force*. Warriors know that to achieve true mastery, we must regard ourselves as our most fearful opponent, we must become our greatest adversary and teacher! Conquering oneself means developing a growth mindset built on resiliency and constant practice, this is the way to self-mastery.

But what does this mean in the context of cyber security? To put it simply, we cannot afford to wait until cyber criminals breach our defences, we must strive to breach them ourselves first, we cannot afford to wait until nation state threats compromise our systems: we must relentlessly attempt to compromise them ourselves.

Disruption is about becoming that force able to disrupt our own defensive operations as much as adversarial ones. This requires a huge shift in mindset, from one of passive to one of active defence. This is the road to cyber self-mastery, a transition from simply reacting to and defending against external challenges, to proactively seeking out opportunities to improve and grow: internal motivation instead of merely external. The required shift involves taking a proactive approach to cyber defence development and actively working to identify and address areas of weakness or imbalance. It calls for a willingness to engage with difficult situations, rather than avoiding or denying them.

Some of the ways these weaknesses are uncovered is via emulation of cyber threats: vulnerability scans simulating exploits, tabletop exercises, cyber readiness programs, penetration tests that attempt to find exploitable avenues to existing apps and services, red and purple teaming that mimic real world threat actor behaviours, etc.

### Deceive

> *All warfare is based on deception. Hence, when we are able to attack, we must seem unable; when using our forces, we must appear inactive; when we are near, we must make the enemy believe we are far away; when far away, we must make him believe we are near.* (Sun Tzu, The Art of War, Book I)

> *Deception and subterfuge are essential ingredients to a successful campaign... The warlord of consistent skill never leaves traces of where he has been. He is indistinguishable among the many.* (Sun Tzu, The Art of War, Book VI)

Everything starts with deception, a strategy as old as human conflict itself. Deception is the art of **influence**. Deception is the act of misleading or tricking someone through the use of false or misleading information, concealing one's true intentions. The goal of deception is to influence adversarial behaviour in order to gain a tactical advantage that helps either disarticulate the opponent's operations or avoid a negative consequence to our own position and assets.

Deception is an essential activity of the Disruption domain, its goal is to ultimately contribute to disruption of adversarial operations.

Cyber Deception is essential in cyberwarfare since it can mean the difference between a full breach and just an *attempted* breach. Cyber Deception takes many different shapes in security operations: 

- honey pots
- honey nets (full scale decoy networks)
- honey tokens (small targeted lures like Azure KeyVault lures, in-memory session credentials for fake accounts, etc.)
- other lures (file)

Deception is accomplished essentially by implementing four components:

- **decoy**: a fake or imitating object that is used to mislead the target.
- **lure**: unlike a decoy, a lure is meant to entice or attract the target towards the decoy.
- **persona**: an analysis of the target, captured for the purposes of running deceptive operations.
- **process**: an intel-driven process that can deploy and monitor the required infrastructure that ties together the persona, decoy and lure.

### Engage

> *By holding out advantages to him, he can cause the enemy to approach of his own accord; or, by inflicting damage, he can make it impossible for the enemy to draw near.* (Sun Tzu, The Art of War, Book VI)

> *Appear at points which the enemy must hasten to defend; march swiftly to places where you are not expected.* (Sun Tzu, The Art of War, Book VI)

The Disruption domain is characterized by any tactics that aim to actively disrupt cyber operations in the anticipation space, either to improve and strengthen your own controls, or to dislocate and thwart adversarial campaigns.

As such, disruption is also the process of intentionally applying the efforts of other domains (Discovery, Defence, etc.) in a directed way, in the form of anticipated force. The space of anticipation is what allows active defence to project hypothetical attack vectors and deploy countermeasures as if the attack vectors were effectively happening.

The goal is to inflict damage on cyber operations. This directed activity can be described as the proactive **engagement** of cyber threats before they even eventuate. The Engagement space has two main purposes that define its tactical goals: **interception** and **coercion**.

Engagement involves a small team of specialized scouts, usually threat hunters, responsible for surveying the area and providing valuable information about the environment and any potential dangers. Threat hunters should be trained in covert operations and interception tactics and use their skills to gather, distribute, and share critical intelligence about the enemy and the cyber battlefield conditions. Their expertise is crucial in helping to ensure the success of cyber operations.

Engaging adversarial operations requires processing collected data into informational signals. It requires drawing from other domains like "Design", to develop a higher understanding of the cyber landscape by analysing available data using aggregation, recombination, clustering and other inference algorithms. The goal of scouting is to intercept adversarial operations to ensure their early disruption, imposing higher operative costs on threat actor's campaigns. To do this, information needs to be contextualized and applied in a directed effort whose outcome is a higher level of insight.

#### Engagement as Interception

Interception refers to a type of interference in the trajectory or course of action of an agent or an object. It assumes that there are patterns that threat actors employ, which end up becoming tendencies that shape a specific course of action. This course of action is the result of engrained patterns that are hard to change without significant energy investment by adversaries. As such, interception aims to stop or interfere with the progress of the chain of events typically evidenced by a specific threat actor. This can be done in various contexts, such as intercepting an encrypted message being transmitted by a C2, or intercepting a phishing campaign on the build in order to frustrate its success.

#### Engagement as Coercion

Coercion is the act of imposing constraints either on the adversary or yourself. The aim of a battle is to coerce the opponent into a course of action that destabilizes their plans, defences and general stance. When directed to adversarial engagement, as opposed to used in a more generic context, coercion takes the shape of **deterrence** or **compellence**. The former aims to prevent the other from enacting a course of action, whilst the latter aims to force the other into a defined course of action, usually controlled by the cyber strategist. Both deterrence and compellence intend on influencing the adversary's behaviour.

An example of coercion in the cyber world would be to develop controlled attack paths in Active Directory and Azure Active Directory. This means, leveraging tools like Bloodhound to (a) understand the current attack paths that could be leveraged to escalate to Domain Admin or similar, (b) craft a fake attack path leveraging deception, which will aim to be the path that threat actors will take, (c) prune your weak attack paths and shape your AD forest to entice (compel) threat actors to take your fake attack path as the easiest one. In executing the above, you will have achieved coercion by compelling cyber adversaries to follow the path of least resistance, one which you control.

### Emulate

> *If you know the enemy and know yourself, you need not fear the result of a hundred battles* (Sun Tzu, The Art of War, Book III)

> *The supreme art of war is to subdue the enemy without fighting* (Sun Tzu, The Art of War, Book III)

Emulation refers to the ability of a system to imitate or replicate the functions of another system. Emulation is characterized by what the ancient Greek world called "**mimesis**" (μίμησις), the act of reproducing or imitating something. Emulation is not a characteristic of computer systems alone, but rather a type of tactic that complex systems employ to dynamically adapt to changing conditions. Think of emulation in the context of history, drama, art, biological organisms, etc. 

In the biological world, for example, emulation can occur when one organism imitates or replicates the behaviours, actions, or characteristics of another organism. This can happen for a variety of reasons, such as to gain some advantage in a particular environment or to avoid being targeted by predators.

In this context, imitation can happen when one species closely resembles another species in terms of physical appearance. For example, certain species of butterflies may mimic the appearance of toxic or unpalatable species in order to deter predators. Imitation can also occur when one species observes and copies the behaviours of another species. For example, some primates, such as chimpanzees, have been observed imitating the facial expressions and gestures of their human caregivers.

Emulation can be wide ranging, and applied in multiple contexts, when a child learns to speak from the parents, when on individual learns a behaviour or skill through observation and imitation, etc. We can even talk about "genetic emulation", when one species evolves to closely resemble another species in order to exploit similar ecological niches, like some species of cichlid fish in Africa's Lake Malawi have evolved to resemble other species in order to better compete for resources.

In the context of cyber security, emulation takes many shapes:

- Vulnerability Scans: when employing technologies that can simulate real exploitation attempts against our systems.
- Red Teaming: simulating real world threat actors in an attempt to compromise our infrastructure and demonstrate feasible attack chains.
- Penetration Testing: simulating application attacks to identify any weaknesses that could be exploited by an attacker, with the goal to determine the security of the system.