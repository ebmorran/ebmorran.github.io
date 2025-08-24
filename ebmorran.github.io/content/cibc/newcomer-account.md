---
title: "Status visibility during manual ID review"
date: 2025-08-01T22:53:58+05:30
draft: false
author: "Elizabeth Morran"
image: /images/passport-photo.jpg
disableMainImg: true
description: "Improving communication during manual identity verification"
summary: "Improving communication during manual identity verification."               
socialShare: false
badges:
          - "Design thinking"
          - "Content design"    
          - "UX strategy"
          - "Stakeholder management"    
toc: true
---
&nbsp;  

## Context
In a banking product for newcomers to Canada, we transitioned from automatic to manual identity verification in our secure portal. As the content designer assigned to this project, I worked with a UX designer to create the new upload flow for the user's ID documents.

<img src="/image_samples/cibc/newcomer/user-flow.png" alt="User flow diagram for manual ID verification" style="margin: auto; width: 100%; padding-bottom:10px;">

The verification process:
* The user uploads their documents. They can't proceed to the next step (funding the account) until manual review is complete. 
* Upon review, the user gets an email notification prompting them to log in to the secure portal to see if the documents were approved. 
* If the documents couldn't be verified, they'll have a second chance to upload before the system forces them to confirm their identity in person.
* If the documents are approved, they can fund the account.

## The problem
<img src="/image_samples/cibc/newcomer/base-screen.png" alt="Original document upload screen with status under the upload button" style="margin: auto; width: 50%; padding-bottom:10px;">

Per business requirements, the document status appeared only under the "Upload your passport..." button. The current status and next step were never clearly surfaced, forcing users to rely on visual searching and deduction.

* **After upload:** The status under "Upload your passport..." changed to "Completed". There was no sign that their documents were under review: they were blocked from the next step without explanation.
* **If the documents were approved:** The next step, "Download wire transfer instructions", silently changed to "Available."
* **If the documents were rejected:** The status under "Upload your passport..." changed to ask the user to retry. Space constraints prevented us from telling the user what would happen if their documents were rejected again.

I raised concerns about this approach, identifying key risks:
* Lack of feedback during a high-stakes task undermines trust and increases drop-off, support calls, and user frustration. 
* It also fails WCAG's success criterion 3.2.2 (on input: change), which requires that users are informed of state changes.

## My contribution
To mitigate these risks and clarify the process, I proposed three contextual banner messages, with corresponding statuses under "Upload your passport and immigration document."

### After upload
<img src="/image_samples/cibc/newcomer/message-1.png" alt="Information banner showing documents under review" style="margin: auto; width: 50%; padding-bottom:10px;">

* **Information banner:** "We received your documents. You'll get an email when we're done reviewing them."
* **Status changes:** "Upload your passport and immigration document" updates to "Under review," reinforcing the banner message. 

The user is now aware of:
* What happened to their documents
* Why they can't proceed right now, and
* What will happen next. 

### Documents approved
<img src="/image_samples/cibc/newcomer/message-2.png" alt="Success banner after documents are approved" style="margin: auto; width: 50%; padding-bottom:10px;">

* **Success banner:** "We verified your documents and it's time to make a one-time wire transfer to your new account. Select 'Download wire transfer instructions' to continue." 
* **Status changes:** As in the original requirements, the "Upload your passport" status changes to "Completed on \[date\]," and the "Download wire transfer instructions" status changes to "Available." 

The user does not have to hunt for information: they know exactly where to look to proceed.

### Documents rejected
<img src="/image_samples/cibc/newcomer/message-3.png" alt="Warning banner when document verification fails" style="margin: auto; width: 50%; padding-bottom:10px;">

* **Warning banner:** "We couldn't verify your documents. Please upload your passport and immigration document again to continue your account setup. If we still can't verify your identity, you can show us your documents at a CIBC Banking Centre when you arrive in Canada."
* **Status changes**: "Upload your passport" status changes to "Your documents couldn't be verified. Upload them again to continue."

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