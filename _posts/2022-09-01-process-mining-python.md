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

The NHS Python Community team met up with Qian Huang - Chief Impact Officer & Co-Founder @ [Logan Todd & Co.](https://www.logantod.net/) at the Confed Expo in Liverpool earlier this year to discuss the use of 'process mining', a well proven analytical technique and has seen widespread adoption in industry [[1](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining)].

## What is Process Mining

Process mining is a technique to analyse and monitor processes. A 'process' can be thought of as a collection of discrete activities or events. The end goal of process mining is to provide actionable operational insights and ultimately help optimise the whole process [[2](https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5)]. This can involve identifying hidden nodes and bottlenecks in business processes. Checking the conformance of a process to a reference model or making predictions about the future state of the process [[2](https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5)].

### Process Mining in a Healthcare Setting

In a healthcare setting, process mining can be used to analyse patient pathways. For example, in elective care, patients start a pathway with a referral, moving them between different appointments and procedures, before completing their journey with a discharge [[1](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining)]. 

<figure class="nhsuk-image">
  <img class="nhsuk-image__img" src="../assets/img/posts/proc-mining.png" alt="Example patient flow visualisation">
  <center>
    <figcaption class="nhsuk-image__caption">
        Figure 1. Example patient flow visualisation
    </figcaption>
  </center>
</figure>

Figure 1. show a visualisation of an example patient pathway developed using process mining. Qian and her team have found that once everybody can see the reality of the patient journey it is much easier to collaborate, identify appropriate actions, and deliver real improvement [[1](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining)].

<div class="nhsuk-action-link">
    <a class="nhsuk-action-link__link" href="https://olobiotokoni.medium.com/write-or-die-fc8a081508b1">
        <svg class="nhsuk-icon nhsuk-icon__arrow-right-circle" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
            <path d="M0 0h24v24H0z" fill="none"></path>
            <path d="M12 2a10 10 0 0 0-9.95 9h11.64L9.74 7.05a1 1 0 0 1 1.41-1.41l5.66 5.65a1 1 0 0 1 0 1.42l-5.66 5.65a1 1 0 0 1-1.41 0 1 1 0 0 1 0-1.41L13.69 13H2.05A10 10 0 1 0 12 2z"></path>
        </svg>
        <span class="nhsuk-action-link__text">Read: Using Process Mining to accelerate eletive recovery in the NHS (Logan Todd & Co.)</span>
    </a>
</div>

## Process Mining in Python

## References

Qian Huang. 2021. "Using Process Mining to accelerate elective recovery in the NHS." [Online] Avaialbe at: [https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining](https://www.logantod.net/resources/accelerate-nhs-recovery-with-process-mining). Logan Todd & Co.

Awesome Process Mining. 2019. [Online] Avaialbe at: [https://github.com/TheWoops/awesome-processmining](https://github.com/TheWoops/awesome-processmining)

Fluxcon. 2020. "Process Mining in Practice." [Online] Avaialbe at: [https://fluxicon.com/book/read/#](https://fluxicon.com/book/read/#)

Eryk Lewinson. 2020. "Introduction to Process Mining" [Online] Avaialbe at: [https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5](https://towardsdatascience.com/introduction-to-process-mining-5f4ce985b7e5). 

c3d3. 2020. "Process Mining with Python tutorial: A healthcare application — Part 1." [Online] Avaialbe at: [https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-1-ae02027a050](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-1-ae02027a050). Four part series [Part 2](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-2-4cf57053421f), [Part 3](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-3-cc9af986c122), [Part 4](https://medium.com/@c3_62722/process-mining-with-python-tutorial-a-healthcare-application-part-4-912286ee51b).

[Fraunhofer Institute for Applied Information Technology (FIT)](http://fit.fraunhofer.de/). 2022. "PM4PY: State-of-the-art-process mining in Python". Application. [Online] Avaialbe at: [https://pm4py.fit.fraunhofer.de/](https://pm4py.fit.fraunhofer.de/).