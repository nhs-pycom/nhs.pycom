---
layout:     post
title:      Process Mining in Python
date:       2022-06-30 12:00:00
summary:    Process Mining in Python
categories: python, process mining, NHS
author:     Craig Shenton
author-bio: Medical Directorate, NHS England
author-link: https://github.com/craig-shenton
---

## NHS Pycom at Confed Expo

At the Confed Expo in Liverpool, the NHS pycom team met up with Qian Huang - Chief Impact Officer & Co-Founder @ Logan Todd & Co. 

The analytical tools used can be complex for non-analysts and the analysis generated provides oversight rather than relevant actionable insights [[1](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining)].

Process mining as a proven technique to analyse any process flow, with widespread adoption outside the NHS [[1](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining)].

We have demonstrated that with any patient flow data, analysts will be able to provide actionable operational insights to business users in days, sometimes within hours, not weeks or months that many NHS business users would expect. 

<div class="nhsuk-action-link">
    <a class="nhsuk-action-link__link" href="https://olobiotokoni.medium.com/write-or-die-fc8a081508b1">
        <svg class="nhsuk-icon nhsuk-icon__arrow-right-circle" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
            <path d="M0 0h24v24H0z" fill="none"></path>
            <path d="M12 2a10 10 0 0 0-9.95 9h11.64L9.74 7.05a1 1 0 0 1 1.41-1.41l5.66 5.65a1 1 0 0 1 0 1.42l-5.66 5.65a1 1 0 0 1-1.41 0 1 1 0 0 1 0-1.41L13.69 13H2.05A10 10 0 1 0 12 2z"></path>
        </svg>
        <span class="nhsuk-action-link__text">Read: Using Process Mining to accelerate eletive recovery in the NHS</span>
    </a>
</div>

## What is Process Mining

Process mining is a technique to analyse and monitor processes. By process we mean a collection of discrete activities or events. A patient journey can be viewed as a series of activities or events e.g. in elective care, patients start their journey from a referral, flowing through a series of processes before completing their journey with a discharge [[1](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining)]. 

The end goal of process mining is to discover, model, monitor, and optimize the underlying processes [[2](https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5)]. This can include:
- Process discovery: analysing event data to identify hidden nodes and bottlenecks in business processes.
- Conformance checking: comparing mined process to the reference model
- Prediction: predicting e.g the state or point of time a future event has/occurs

## PM in a healthcare setting

Basic output is to visualise the real patient journey so that

> "All teams involved can easily understand what they are looking at, get value from their own data, and start identifying appropriate actions"

Once everybody can see the reality of the patient journey it is much easier to collaborate and deliver real improvement.

### Figure: Exaple patient flow visualisation
<div class="nhsuk-card">
    <img alt="code" class="nhsuk-card__img" src="../assets/img/posts/proc-mining.png" />
</div>

### Advanced Analysies

- Understand where patient flows are disrupted, stuck, or having processes duplicated.
- Spot bottlenecks and show policy makers where to invest - i.e., clinical, admin or diagnostic capacity
- Release capacity by reconfigureing patient pathways
- Measure the impact of non-conformance to best practice

### Data Preperation
The key element of any successful analysis is data preparation - in process mining, this relates to the preparation of Event logs where a single entry is an unique event ID, an associated activity and the timestamp of the activity.  All other information about an event are considered optional attributes that can be easily linked to the Event log using the unique event ID to create an incredibly rich and relevant analysis.
Examples of optional attributes include:

- Patient attribute: age, gender, disability
- Workforce attributes: specialism, staff group, working hours
- Outcome attributes: referral accepted, discharged, follow-up appointment required
- Pathway attributes: RTT, Cancer 2-weeks wait, Urgent, Routine, Admitted, Non-Admitted

Both the Event log and optional attributes data typically resides in existing systems within the NHS e.g. PTL, PAS, EPR which means process mining can be applied to any NHS organisation today.

## Process Mining in Python

## References

Qian Huang. 2021. "Using Process Mining to accelerate elective recovery in the NHS." [Online] Avaialbe at: [https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining). Logan Todd & Co.

Awesome Process Mining. 2019. [Online] Avaialbe at: [https://github.com/TheWoops/awesome-processmining](https://github.com/TheWoops/awesome-processmining)

Fluxcon. 2020. "Process Mining in Practice." [Online] Avaialbe at: [https://fluxicon.com/book/read/#](https://fluxicon.com/book/read/#)

Eryk Lewinson. 2020. "Introduction to Process Mining" [Online] Avaialbe at: [https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5](https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5). 

c3d3. 2020. "Process Mining with Python tutorial: A healthcare application — Part 1." [Online] Avaialbe at: [https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-1-ae02027a050](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-1-ae02027a050). Four part series [Part 2](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-2-4cf57053421f), [Part 3](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-3-cc9af986c122), [Part 4](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-4-912286ee51b).

[Fraunhofer Institute for Applied Information Technology (FIT)](http://fit.fraunhofer.de/). 2022. "PM4PY: State-of-the-art-process mining in Python". Application. [Online] Avaialbe at: [https://pm4py.fit.fraunhofer.de/](https://pm4py.fit.fraunhofer.de/).