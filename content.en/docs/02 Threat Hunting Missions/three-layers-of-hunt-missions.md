---
weight: 2
title: "The Three Layers of Threat Hunt Missions"
---

## The Three Layers of Threat Hunt Missions

Threat hunt missions can be described as three different layers that are interconnected. Each of these layers can be developed in parallel or in sequence but the three of them are necessary for the successful execution of hunting missions. As a threat hunt mission progresses, each layer generates artefacts of particular types which capture the evolution of the hunt's activities.

![mission-functional-levels.excalidraw](/diagrams/mission-functional-levels.excalidraw.svg)

<!--more-->

### Operational Layer

In this layer, we monitor the progress of a hunting mission, the who, what, why and how. A hunt mission is represented here in terms of components that help schedule and monitor the evolution of it. This level helps us organize the hunt mission by breaking it down into phases and tasks within them. The framework employed by AIMOD2 to run the operational level is Agile, in its SCRUM implementation. The types of activities that we track in this level are:

- Layout of the hunt mission as phases and tasks
- Task accountabilities and overall hunt progress
- Response or disruption actions: escalation of suspicious events (potential security incidents), Threat Intelligence Observables (TIO) or security control risks, etc.

**Associated Artifacts**: Epics, Stories or Tasks.

### Recursive Layer

At this layer, we capture the contextual information and data insights from our hunt and encapsulate them in artifacts that are capable of being reproduced and repeated. Threat Hunting is an iterative process, the results of our hunting and research efforts need to be recorded in a reproducible format that enables continuous improvement. The way we improve our hunt missions is by iterating through them in a manual or automated way.

**Associated Artifacts**: threat hunt playbook, iterative analytics (dashboards, stored queries and alerts, automation scripts)

### Analytical Layer

At this level we capture the measurable results of an iteration of a hunt mission. The results of this particular iteration of a hunt are unique to this instance of it and represent a snapshot in time. In this layer, we want to produce an artifact that captures high level metrics and documents observed risks, this is usually delivered as a report. There are other artefacts that are useful to understand the hunting mission's outcomes too: metadata such as sprint velocity and size, comparative impact of hunt outcomes, etc. provide an indication of the quality and value-add of our cyber hunting efforts.

**Associated Artifacts**: reports (a snapshot of a hunt), metrics, comms.