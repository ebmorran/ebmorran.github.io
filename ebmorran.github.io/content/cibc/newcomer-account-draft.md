---
title: "Reducing user dropoffs in KYC flow"
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
          - "Stakeholder management"    
toc: true
---
**Role:** Content Designer     
**Project:** Adding manual identity verification to onboarding flow for newcomer banking product     
**Timeline:** July 2025 - August 2025


## Overview
When CIBC shifted from automatic to manual identity verification in a newcomer banking product, I led content design for the project that added document upload to the onboarding flow. The initial project requirements included little visible or explicit feedback in the upload process, at risk of user dropoff and extra support calls. 

I identified the issue early, proposed a messaging framework and collaborated with design, product and engineering to integrate it seamlessly. The new system gave users confidence at a critical onboarding step and reduced confusion during a sensitive identity check.

| Flow step | Before | After |
| ----------- | ----------- | ----------- |
| **After document upload** | <img src="/image_samples/cibc/newcomer/before-1-after-upload.png" alt="Before state 1" style="margin: auto; width: 100%; padding-bottom:10px;">| <img src="/image_samples/cibc/newcomer/message-1.png" alt="Message 1" style="margin: auto; width: 100%; padding-bottom:10px;"> |
| | *Upload is complete, but what now? Why can't I proceed?* | *Clear, visually obvious explanation: my documents are under review and I'll get an email.* |        |
| **Documents were verified** - user receives "check the portal for an update" email and clicks link | <img src="/image_samples/cibc/newcomer/before-2-upload-succeeded.png" alt="Before state 2" style="margin: auto; width: 100%; padding-bottom:10px;"> | <img src="/image_samples/cibc/newcomer/message-2.png" alt="Message 2" style="margin: auto; width: 100%; padding-bottom:10px;"> |
| |   | Text        |
| **Documents could not be verified** - user receives "check the portal for an update" email and clicks link | <img src="/image_samples/cibc/newcomer/before-3-upload-failed.png" alt="Before state 3" style="margin: auto; width: 100%; padding-bottom:10px;"> | <img src="/image_samples/cibc/newcomer/message-3.png" alt="Message 3" style="margin: auto; width: 100%; padding-bottom:10px;"> |
| | Paragraph   | Text        |

## The problem

Per business requirements, the document status appeared only under the "Upload your passport..." button. The current status and next step were never clearly surfaced, forcing users to rely on visual searching and deduction.

* **After upload:** The status under "Upload your passport..." changed to "Completed". There was no sign that their documents were under review: they were blocked from the next step without explanation.
* **If the documents were approved:** The next step, "Download wire transfer instructions", silently changed to "Available."
* **If the documents were rejected:** The status under "Upload your passport..." changed to ask the user to retry. Space constraints prevented us from telling the user what would happen if their documents were rejected again.

I raised concerns about this approach, identifying key risks:
* Lack of feedback during a high-stakes task undermines trust and increases drop-off, support calls, and user frustration. 
* It also fails WCAG's success criterion 3.2.2 (on input: change), which requires that users are informed of state changes.
<img src="/image_samples/cibc/newcomer/user-flow.png" alt="User flow diagram for manual ID verification" style="margin: auto; width: 100%; padding-bottom:10px;">


The user is now aware of:
* What happened to their documents
* Why they can't proceed right now, and
* What will happen next. 


The user does not have to hunt for information: they know exactly where to look to proceed.
The user doesn't have to visually scan the page to know what happened. They are clearly informed of next steps and how to recover from further issues:
* This is their last chance to upload the documents.
* If the next document upload fails, they can still verify their identity in person instead of online.

## Alignment and outcome

The developers on the team were reluctant to make these changes, arguing that the existing status indicators were enough. But with backup from the UX designer, I strongly advocated for this solution, asking the team to put themselves into the shoes of a newcomer:
* They're unfamiliar with Canadian culture and banking practices.
* They're likely feeling tension, and afraid of making mistakes in a bureaucratic system.
* They could have any age, amount of education, degree of English ability or level of ease with technology. 

This user would need clear instructions, reassurance and predictable steps. 

The product owner agreed with my reasoning, and the team implemented all three messages. This improved transparency, reduced confusion, and created a more supportive experience during a sensitive step in the immigration process.