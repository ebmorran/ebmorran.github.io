---
title: "Building transparency into newcomer onboarding"
date: 2025-08-01T22:53:58+05:30
draft: false
author: "Elizabeth Morran"
image: /images/passport-photo.jpg
disableMainImg: true
description: "Reduced user drop-offs during ID verification by introducing a clear feedback framework that improved predictability and trust."
summary: "Reduced user drop-offs during ID verification by introducing a clear feedback framework that improved predictability and trust."               
socialShare: false
badges:
          - "Design thinking"
          - "Content design"    
          - "UX strategy"
          - "Onboarding flows"
          - "Stakeholder management"    
toc: true
---
**Role:** Content Designer     
**Project:** Adding manual identity verification to onboarding flow for newcomer banking product     
**Timeline:** July 2025 - August 2025

## An upload process with little feedback or guidance
When CIBC shifted from automatic to manual identity verification in a newcomer banking product, I led content design for the project that added document upload to the onboarding flow. The original requirements included almost no visible feedback:
* After upload, the user wasn't informed they'd have to wait for manual document review to continue.
* Approval and rejection were silent: users had to deduce what happened by scanning down the page.

Instead, I proposed a messaging framework to create a clear, predictable path through document verification, reducing visual searching and decision fatigue, supporting accessibility and building trust during a sensitive onboarding process. 

## Guiding users forward with clear status messages
| Flow step | Before | After |
| ----------- | ----------- | ----------- |
| **Immediately after document upload**  | <img src="/image_samples/cibc/newcomer/before-1-after-upload.png" alt="Before state 1" style="margin: auto; width: 100%; padding-bottom:10px;">| <img src="/image_samples/cibc/newcomer/message-1.png" alt="Message 1" style="margin: auto; width: 100%; padding-bottom:10px;"> |
| | *Upload is complete, but what now? The user doesn't know why they can't proceed.* | *Clear explanation and next steps.* |
| **Documents verified** | <img src="/image_samples/cibc/newcomer/before-2-upload-succeeded.png" alt="Before state 2" style="margin: auto; width: 100%; padding-bottom:10px;"> | <img src="/image_samples/cibc/newcomer/message-2.png" alt="Message 2" style="margin: auto; width: 100%; padding-bottom:10px;"> |
|The user receives a notification email with a link to view an update in the portal. | *The next step (Download wire transfer instructions) silently became available, but it's not obvious to look there.* | *The user immediately knows that their ID was verified and which action to choose next.* |
| **Documents not verified** | <img src="/image_samples/cibc/newcomer/before-3-upload-failed.png" alt="Before state 3" style="margin: auto; width: 100%; padding-bottom:10px;"> | <img src="/image_samples/cibc/newcomer/message-3.png" alt="Message 3" style="margin: auto; width: 100%; padding-bottom:10px;"> |
| The user receives a notification email with a link to view an update in the portal. | *Though the update is explicit, it's buried as a status message on a button. In the constrained space, we couldn't mention the fallback ID option, increasing potential anxiety.* | *The update is visually obvious. It reassures the user they can always provide their documents in person, reducing tension and frustration.* |
{.compare-table}

## Driving alignment

Because feedback messages weren’t part of the original scope, I partnered with design and product to drive alignment and secure buy-in for the new framework:
* Reframed the problem around user trust, accessibility, and business outcomes.
* Illustrated how missing feedback would increase support volume and onboarding drop-offs.
* Secured consensus despite initial engineering pushback, ensuring full implementation.

## Outcomes: transparency, accessibility and trust

The original approach carried significant business and UX risks:
 * Lower conversion: users might abandon the process when blocked without explanation.
 * Higher support costs: missing feedback would drive calls to the support line.
 * Erosion of trust: newcomers, already navigating an unfamiliar banking system, would feel uncertain and unsupported.
 * Compliance failure: the flow failed WCAG 3.2.2, which requires that state changes be announced to users.

By introducing a clear, layered feedback framework, my redesigned experience:
* Increased user confidence during a sensitive onboarding step.
* Reduced frustration and lowered support burden.
* Ensured accessibility compliance while supporting a broader range of user needs and English proficiency levels.
* Aimed to increase onboarding completion by explaining blockers and surfacing next steps.