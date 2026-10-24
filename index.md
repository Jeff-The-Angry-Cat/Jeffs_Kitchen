---
layout: default
title: "Sensing and Responding: Security as One Network"
description: "How a cybersecurity mesh, CTEM, the OODA loop, UK ISR doctrine and Ukraine's Delta system point to a security department that works as one team."
date: 2026-10-24
---

# Sensing and Responding: Security as One Network

*October 2026*

## Introduction

Most security departments are organised as a set of separate teams: one for identity, one for networks, one for monitoring, one for vulnerabilities, one for policy and compliance. Each has its own tools, its own data and its own manager. People often call these teams "stovepipes" or "silos", because information travels up and down inside each one but rarely across.

That structure is too slow for modern attacks. An attacker does not care which team owns which system. They move from a phishing email to a stolen password to a cloud server in hours. If each team only sees its own slice, nobody sees the whole attack until it is too late.

This paper argues that the fix has two parts:

- **A shared technology fabric** that joins the tools together, so that everyone sees the same picture. The industry name for this is a "cybersecurity mesh".
- **A way of working** that lets many teams act as one. For this, the best guide is not from the security industry at all. It comes from the armed forces, which have spent decades learning how to turn many separate sensors and units into one team that is always watching and always ready to act.

Neither part works alone. Joining up the tools without changing how people work just recreates the silos in software. Changing how people work without a shared picture leaves them nothing to work from.

The paper explains each idea in plain terms: the mesh and its continuous checking for weaknesses, a decision model called the OODA loop, a recent piece of UK military guidance, and a system Ukraine has built to share battlefield information. It then describes the way of working they point to, and where the military comparison stops being useful in a bank.

It runs alongside two earlier papers, *Designing the Whole* and *Security Within the Business's Risk Appetite*. It shares their starting point: the business owns the risk, and security works within the level of risk the business is willing to accept.

## The mesh: joining up the tools

Ten years ago, most of a bank's systems sat inside its own buildings and data centres, and security was largely about guarding the edge. Today systems sit in the cloud, on staff laptops at home, and with dozens of suppliers. There is no single edge left to guard.

The research firm Gartner coined the term **Cybersecurity Mesh Architecture (CSMA)** in 2021 for its answer to this. It is not a product you can buy. It is a design approach: keep the many security tools a firm already has, but connect them so they share information and follow the same rules ([Check Point summary](https://www.checkpoint.com/cyber-hub/cyber-security/what-is-cybersecurity-mesh-architecture-csma)). Gartner describes four shared layers that sit across all the tools:

| Gartner's layer | What it means in plain terms | The military equivalent |
| --- | --- | --- |
| Security analytics and intelligence | One place where warning signs from every tool are collected and compared | A network of sensors feeding one intelligence cell |
| Distributed identity | Every person, device and system has one identity that all tools recognise | A shared map grid, so everyone describes locations the same way |
| Consolidated policy and posture | One set of security rules, applied wherever the system lives | The commander's instructions, which every unit follows |
| Consolidated dashboards | One view of what is happening, for everyone who needs to decide | A shared battle map |

The right-hand column is why the mesh feels so close to military thinking. Both are about turning many separate eyes into one picture.

There is a catch. A well-known rule in technology, Conway's law, says that systems end up mirroring the structure of the organisation that builds them. If the identity team, the network team and the monitoring team each keep their own tools, budgets and managers, they will build three separate meshes that do not talk to each other. Each will guard its own data. The "shared" layers will be shared only on the architecture diagram. So the way the department is organised has to change along with the technology, or the technology will quietly drift back to match the old silos.

## Addendum: CTEM, checking for weaknesses all the time

The mesh joins the tools up. **Continuous Threat Exposure Management (CTEM)** is the habit of constantly asking: "If someone attacked us today, where could they get in, and would it matter?" Gartner introduced the idea in 2022. Like the mesh, it is a way of working rather than a product. It has five stages ([Vectra summary](https://www.vectra.ai/topics/ctem)):

1. **Scoping**: agree with the business which services, data and people matter most. Start there, not with a list of every system.
2. **Discovery**: look for weaknesses in that scope. These include software flaws, but also badly set-up systems, weak passwords and people with more access than they need.
3. **Prioritisation**: rank what was found by how much harm it could do to the business and how easily an attacker could reach it, not by a generic severity score.
4. **Validation**: test whether an attacker could really use the weakness, for example by hiring people to try ("red teaming").
5. **Mobilisation**: get the right people, often outside security, to fix it by an agreed date. Then feed what was learned back into step 1.

Gartner predicted that organisations working this way would be three times less likely to suffer a breach by 2026. That is a forecast, not a proven result: no published study has yet measured it.

CTEM deserves its own mention for three reasons.

- **It starts and ends with the business.** The business decides what matters, and fixes are ranked by business harm. This is the same starting point as the risk appetite paper.
- **It makes the mesh look ahead, not just react.** Spotting and stopping an attack in progress is a fast, short loop. CTEM is a slower loop that runs all the time, before any attack. Both feed the same shared picture. Without CTEM, the mesh only ever responds to things that have already happened.
- **Its hardest step is about people, not technology.** Most CTEM programmes stall at mobilisation, because the people who must make the fix sit in technology teams, operations or the business, not in security. That only works if the department and its colleagues behave as one team, rather than security sending tickets over a wall.

So CTEM is best seen as part of the mesh rather than separate from it. The mesh supplies the eyes and the rules. CTEM supplies the discipline of deciding what to look for, what matters most, and who acts.

## The OODA loop: shared understanding beats raw speed

**What it is.** The OODA loop was developed by John Boyd, a US Air Force fighter pilot and strategist, in the 1970s and 1980s. It describes how any person or organisation makes decisions under pressure, in four steps:

1. **Observe**: notice what is happening.
2. **Orient**: make sense of it, using experience, knowledge and culture.
3. **Decide**: choose what to do.
4. **Act**: do it, then observe the result and go round again.

An everyday example is a driver who sees brake lights ahead (observe), recognises a traffic jam forming (orient), chooses to change lanes (decide) and steers (act).

**What people often miss.** OODA is usually summed up as "go round the loop faster than your opponent". Boyd's own later work (*The Essence of Winning and Losing*, 1995) says something more useful. The most important step is **orient**, the sense-making. When a group of people share the same understanding of the situation and the same idea of what matters, they can act without stopping to ask permission, because they already know what their leader would want. Boyd called this "implicit guidance and control". Speed follows from shared understanding; it is not a goal on its own. Frans Osinga's study of Boyd, *Science, Strategy and War* (2007), makes the same case.

**Why it matters here.** This is the heart of the silo problem. A siloed security department does not lack tools or data. It lacks a shared understanding. So every warning sign has to travel up one team's chain of command and down another's before anyone acts. The department moves at the speed of its organisation chart.

Shared understanding comes from three things, and each is something a leader can design:

- **A common picture**: everyone sees the same information, described in the same way. This is what the mesh provides.
- **Shared intent**: everyone knows what matters and how much risk is acceptable. In a bank, this comes from the business's risk appetite.
- **Trust to act**: people are allowed to act within that intent without asking first. The armed forces call this "mission command": leaders say what needs to be achieved and why, and leave the how to the people on the ground. Stanley McChrystal's book *Team of Teams* (2015) describes how the same idea transformed US special forces in Iraq, summed up as "shared consciousness and empowered execution".

The first is technology. The second is governance. The third is how the organisation is designed.

## What the military calls ISR, and what it teaches us

**What it is.** Armed forces need to know what is happening around them: where the other side is, what it is doing, and what it might do next. Gathering and making sense of that information is called **ISR**, short for intelligence, surveillance and reconnaissance:

- **Surveillance** is watching an area continuously, like a CCTV camera.
- **Reconnaissance** is going to look at something specific for a purpose, like sending a drone to check a particular road.
- **Intelligence** is the end product: what all that watching means, and what to do about it.

You will also hear **ISTAR**, which adds "target acquisition": pinning down exactly where something is so that action can be taken against it. Security has a direct equivalent: finding exactly which account or server an attacker is using so it can be shut off.

In 2023 the UK Ministry of Defence published a short guide on how British forces should do this: [Joint Doctrine Note 1/23, Intelligence, Surveillance and Reconnaissance](https://assets.publishing.service.gov.uk/media/641c27e15155a200136ad4df/JDN_1_23_ISR_web.pdf). ("Joint" means across the Army, Navy and Air Force; "doctrine" means the agreed way of doing things.) Read with a security department in mind, it is almost a manual for working as one team. Five of its ideas carry straight across.

**1. Information gathering serves operations, not just analysts.** The guide describes ISR as "an integrated intelligence and operations set of capabilities" (p. 3). The people who gather information and the people who act on it are one system. In security terms, threat intelligence, monitoring, vulnerability management and incident response are one capability, not four separate teams.

**2. One effort, not divided up.** The guide says ISR should not be "artificially divided" between land, sea, air or levels of command, and that equipment should be used wherever it is needed, regardless of who owns it (paras 1.14 to 1.15). Swap "land, sea and air" for "cloud, laptops and identity", and this is the case against silos in one sentence.

**3. The commander decides what to look for.** Information gathering starts with requests from the people in charge, which are checked, ranked and matched to the right sensors (paras 2.1 to 2.4). In a bank, the "commander" is the business leader who owns the risk. Their priorities, set by the business's risk appetite, decide what security watches most closely. This is the same idea as CTEM's scoping step.

**4. The data does not belong to whoever collected it.** The guide says making sense of information is "not subordinate to collection" (para 4.1), and prefers models where many teams share and analyse it together (para 4.13). In security terms, warning signs from the firewall team, the identity team and the cloud team should be pooled and analysed together, not kept and judged inside each team.

**5. Say what you need, not how to do it.** Orders state what is to be achieved, not how, and rely on "an empowered collection operations manager" to adapt on the spot (paras 2.20, 2.25). This is mission command again, and it is what lets the loop run without waiting for permission.

The guide breaks ISR into five steps (task, collect, process, exploit, disseminate), which map onto security like this:

| Military step | What it means in security | Who owns it in a one-team model |
| --- | --- | --- |
| Task | Decide what to watch for, based on business risk and known threats | The business sets priorities; security turns them into a watch list |
| Collect | Gather logs, scan for weaknesses, take reports from staff and suppliers | Every team and tool, including the business |
| Process and exploit | Pull the signals together and work out what they mean | One shared analysis function, fed by all |
| Disseminate | Get the picture and the actions to whoever must act | Whoever owns the fix, inside or outside security |

The guide is also frank that the main challenge is the sheer amount and variety of data, and asks that all collected data be treated as potentially valuable when it is gathered (paras 1.17d, 1.19). That is a strong argument for one shared pool of security data rather than each tool keeping its own.

## Ukraine's Delta: one live map that everyone adds to

**What it is.** [Delta](<https://en.wikipedia.org/wiki/Delta_(situational_awareness_system)>) is a computer system used by Ukraine's armed forces since Russia's full-scale invasion in 2022. Think of it as a shared live map of the battlefield, a little like a navigation app that shows traffic reported by other drivers. Units, drones, satellites, radar, allied countries and even vetted members of the public add what they see: a tank in a field, a supply truck on a road. Everyone with access can see the result, plan missions on it and coordinate with neighbouring units.

**What it replaced.** Before systems like Delta, information moved by radio, phone and paper map. A drone operator who spotted a target reported it up their own chain of command, someone passed it across to another unit, and that unit decided whether to act. Ukrainian officials say this could take up to 72 hours, by which time the target had often moved. With Delta, they say, the time from spotting a target to acting on it is now about two minutes, and about 90% of combat units use the system ([Business Insider via AOL](https://www.aol.com/articles/ukraines-digital-war-tool-cut-151256172.html)). These are the officials' own figures and have not been independently checked, but the scale of change they describe is the point.

**What made it work.** The technology matters less than how it came about.

- **It was designed to share, not hoard.** Delta began in 2017 as part of a NATO exercise on getting units to share information instead of each keeping its own.
- **It was built by insiders and outsiders together.** The Ministry of Defence built it with Aerorozvidka, a volunteer group of drone enthusiasts, and kept improving it based on soldiers' feedback.
- **Everyone gives and everyone gets.** A unit that reports a sighting can also see everyone else's. Contributing is how you benefit.
- **Computers take the first look.** An add-on called Avengers scans drone and camera video and flags enemy vehicles automatically, reportedly about 12,000 a week, so people spend their time judging what to do rather than staring at screens.
- **It is protected as a prime target.** Because it holds so much valuable information, it has been attacked itself, including a phishing campaign in December 2022. In early 2026 it passed an independent security assessment against more than 160 requirements.

**What a bank can learn.** A shared security picture should be fed not only by the security operations team, but by the business, technology teams, suppliers and ordinary staff, and each contributor should get something useful back. Automation should do the first sift so that people can concentrate on judgement. And the picture, which by its nature shows every weakness the firm has, needs the strongest protection of all.

## The operating model: two loops, one picture

Put together, these ideas describe one way of working. The business says what matters. Everyone works from one shared picture, so they understand the situation the same way. Two loops run off that picture: a slow loop (CTEM) that checks for weaknesses all the time, and a fast loop (OODA) that spots and stops attacks as they happen. Both loops draw information from, and hand actions to, one team that reaches well beyond the security department.

![Two loops share one picture and one intent: business intent at the top sets requirements for an exposure loop (CTEM), a common security picture, and a response loop (OODA); all draw signals from and send actions to one team of security, technology, business, suppliers and staff.](two-loops-one-picture.svg)

Reading the diagram from top to bottom: the top band is the "commander's" priorities from the military guide, and CTEM's scoping step. The centre is the joined-up mesh, and Delta shows it should be fed by everyone. The bottom band is where the silos are removed.

Four practical choices follow.

1. **Organise around the shared picture, not the tools.** Each team keeps its specialist skills, but no team owns its data. One shared analysis function pulls everything together.
2. **Turn risk appetite into clear rules for action.** Write down what people may do without asking (lock a stolen account, isolate an infected laptop) and what must go to the business owner first (take a payment service offline). This is mission command in a bank.
3. **Make fixing things a shared duty.** Whoever runs a system owns its fix. Security provides the picture, the priority and the deadline.
4. **Reward people for contributing to the picture.** Teams and business units that feed it should get faster, better answers back, just as Delta's units do.

The three roles from the earlier paper fit onto the diagram. As **CISO**, the head of security writes the security part of the business's priorities and checks that both loops stay within them. As **service provider**, they run the picture and both loops as services to the business. As **head of department**, they invest in the technology and shape the one team. The diagram also makes the tension plain: the same person both runs the loops and checks them.

## Where the military comparison stops

The comparison is useful, but a bank is not an army. Four differences matter.

- **The person in charge sits outside security.** In the armed forces, the people gathering information and the commander are in the same chain of command. In a bank, priorities come from the business and the firm-wide risk framework, not from the security department. Security can run the loops but cannot set their purpose.
- **The aim is to stay within limits, not to win.** A military response aims to defeat the enemy. A security response aims to keep the business within the risk it has agreed to accept and the disruption it can tolerate, under rules such as the UK's operational resilience regime and the EU's Digital Operational Resilience Act (DORA). Sometimes the right answer is to accept a risk, not to act on it.
- **Faster is not always better.** Delta's two-minute loop works because striking the target is the expected outcome. Shutting down a payment system in two minutes could do more damage than the attacker. The firm needs to agree in advance which actions people may take on their own and which need the business owner's say.
- **Someone still has to check independently.** Armed forces do not have a separate function checking that controls work. Banks do. A security department that both runs controls and checks them must keep enough distance to do the checking honestly. This is the three-roles tension from the earlier paper.

## Open questions

- Which response actions can the department take on its own authority, and which must go back to the business risk owner? This is the boundary of mission command.
- Who owns the common picture: security, technology, or the enterprise risk function?
- How should the department be organised to run one loop: by capability (identity, network, cloud) as today, or by mission (protect payments, protect customer data) as JDN 1/23's problem-centric model suggests?
- How should success be measured: by speed of the loop, or by time spent within appetite?

## Plain-English glossary

| Term | Meaning |
| --- | --- |
| CSMA (cybersecurity mesh) | Gartner's design approach of joining separate security tools so they share data and follow one set of rules |
| CTEM | Continuous Threat Exposure Management: constantly finding, ranking, testing and fixing weaknesses, starting from what matters to the business |
| Delta | Ukraine's shared live battlefield map, fed by units, drones, satellites and allies |
| Doctrine | The armed forces' agreed way of doing something |
| ISR | Intelligence, surveillance and reconnaissance: gathering information and working out what it means |
| ISTAR | ISR plus target acquisition: pinpointing something precisely enough to act on it |
| Mission command | Leaders say what to achieve and why; the people on the ground decide how |
| OODA loop | Observe, orient, decide, act: John Boyd's model of decision-making under pressure |
| Silo or stovepipe | A team whose information flows up and down its own chain but rarely across to others |

## Sources

Opened for this paper:

- UK MOD, [JDN 1/23 Intelligence, Surveillance and Reconnaissance](https://assets.publishing.service.gov.uk/media/641c27e15155a200136ad4df/JDN_1_23_ISR_web.pdf) (January 2023)
- [Cybersecurity Mesh Architecture (CSMA)](https://www.checkpoint.com/cyber-hub/cyber-security/what-is-cybersecurity-mesh-architecture-csma), Check Point summary of Gartner's model
- [CTEM explained](https://www.vectra.ai/topics/ctem), Vectra summary of Gartner's five stages
- [Delta (situational awareness system)](<https://en.wikipedia.org/wiki/Delta_(situational_awareness_system)>), Wikipedia
- [Ukraine's digital war tool cut the time between finding and striking targets from days to minutes](https://www.aol.com/articles/ukraines-digital-war-tool-cut-151256172.html), Business Insider via AOL
- [OODA Loops in Cyberspace: A New Cyber-Defense Model](https://cps-vo.org/sites/cps-vo.org/files/cpsvo_file_nodes/OODA_Loops_in_Cyberspace_A_New_Cyber-Defense_Model.pdf)

Cited from general knowledge, worth reading in full: John Boyd, *The Essence of Winning and Losing* (1995); Frans Osinga, *Science, Strategy and War* (2007); Stanley McChrystal, *Team of Teams* (2015).
