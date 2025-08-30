---
title: "Designing a portal that works the way advisors do"
date: 2022-02-10T22:53:58+05:30
draft: false
author: "Elizabeth Morran"
image: /images/advisor-portal-screenshot.png
description: "Our research uncovered advisors' true mental models, shaping a portal that cut friction and accelerated decision-making."
summary: "Our research uncovered advisors' true mental models, shaping a policy-first portal that cut friction and accelerated decision-making."
socialShare: false
badges:
           - "User research"
           - "Usability testing"
           - "User interviews"   
           - "Stakeholder communication"
           - "Heuristic evaluation"
           - "Behavioral observation"
toc: true
images_policy_before:
  - src: "/image_samples/medavie/advisor-portal-study/original-landing-snipped.png"
    caption: "Dashboard before redesign. There was no consensus on how to select and sort this table."
    alt: "Original advisor portal dashboard showing an unsorted table of clients."
  - src: "/image_samples/medavie/advisor-portal-study/original-client-list.png"
    caption: "If a client wasn't on the dashboard, advisors would click 'Clients' in the main nav."
    alt: "Original client list page requiring advisors to navigate through clients to find a policy."
  - src: "/image_samples/medavie/advisor-portal-study/original-client-details.png"
    caption: "To find policy details, advisors needed to click through the 'Client Details' page."
    alt: "Original client details page displaying limited policy information."
  - src: "/image_samples/medavie/advisor-portal-study/original-policy-details.png"
    caption: "Policy details reached after 2 or 3 clicks."
    alt: "A policy details page, showing the essential details Advisors want to see."

images_policy_after:
  - src: "/image_samples/medavie/advisor-portal-study/new-landing-snipped.png"
    caption: "Dashboard after redesign. Policies centered and sorted by renewal date."
    alt: "Redesigned dashboard displaying a streamlined policy table sorted by renewal dates."
  - src: "/image_samples/medavie/advisor-portal-study/new-policies-list-snipped.png"
    caption: "Skip the 'Client' layer entirely, heading directly to a policy or the policies list."
    alt: "Updated policies list page allowing direct navigation to policies without going through client details."
  - src: "/image_samples/medavie/advisor-portal-study/new-policy-details-snipped.png"
    caption: "Policy details reached after 1 or 2 clicks. Client info displayed per policy instead of vice-versa."
    alt: "Redesigned policy details page with client data integrated per policy."

images_marketing_materials:
  - src: "/image_samples/medavie/advisor-portal-study/original-marketing-materials-snipped.png"
    caption: "Before: Users were overwhelmed by the many topic options, not realizing they were optional. They overlooked the inline search button, scrolling past it and scanning the page to find the bottom button."
    alt: "Original marketing materials search interface showing an overcrowded list of topic filters."
  - src: "/image_samples/medavie/advisor-portal-study/new-reference-materials-snipped.png"
    caption: "After: Collapsed filter options into a single drop-down menu, progressively disclosing filtering options and emphasizing the search button."
    alt: "Redesigned reference materials search with simplified dropdown filters."
  - src: "/image_samples/medavie/advisor-portal-study/new-reference-materials-filters-snipped.png"
    caption: "After: Filter menus are multi-select. When nothing is selected, 'all topics' and 'all audiences' are the default."
    alt: "Updated reference materials filters supporting multi-select options for flexible searching."

images_policy_docs:
  - src: "/image_samples/medavie/advisor-portal-study/policy-documents-snipped.png"
    caption: "Before: An unnecessary 'Select all' toggle slowed down users."
    alt: "Original policy documents page showing a 'Select all' toggle that confused and slowed down users."
  - src: "/image_samples/medavie/advisor-portal-study/policy-documents-noselect-snipped.png"
    caption: "After: Toggle removed. 'Select all' is now the default behavior if neither or both types are selected."
    alt: "Updated policy documents page with 'Select all' toggle removed."
--- 

**Team:** Elizabeth Morran (content designer), Tayla Gurgel (UX designer)  
**Project:** Building a comprehensive portal for advisors of group health insurance plans     
**Timeline:** June - July 2024  
**Methods:** Task-based usability testing, semi-structured interviews

## The goal: use research to drive clarity and strategy

I led content design for Advisor Connect, a new portal giving Group Advisors self-serve access to client data, forms and policy brochures, reducing their reliance on MBC account executives. But the product team had conflicting visions, and existing personas based on external research couldn't resolve them.

At the outset, we had little understanding of advisors' workflows, or even the nature of the data we were displaying. I pushed to run this study to validate assumptions about terminology, navigation and the content model, ensuring the portal matched how advisors think and work.

We combined semi-structured interviews with task-based usability testing on a high-fidelity prototype:  
* Six remote interviews with five structured usability tasks focused on locating policies, forms and resources  
* Think-aloud protocol to capture real-time reactions  
* Cluster analysis to identify behavioral patterns

## Key finding: The core content model was wrong

### Before: the journey to policies, buried under clients
{{< slideshow id="policy_before" from="images_policy_before" >}}

- The portal was built with the client as the core object, forcing them to click into a policy from the client page. 
- We didn't know what criteria to use to select the homepage table, or how we should sort tables by default.

### After: the policy as the core object of the portal
{{< slideshow id="policy_after" from="images_policy_after" >}}

- We found that Advisors primarily think in terms of policies, sometimes even using "policy" and "client" interchangeably.
- I redesigned the IA around policies, including client information within Policy Details instead of forcing users through unnecessary layers.
- Renewal dates were added to policy tables and used as the default sort (soonest), following the Advisors' emphasis on their importance.

## Terminology and order in main navigation
### Before: marketing materials were neither seen as important nor as marketing materials
<figure class="image">
  <img src="/image_samples/medavie/advisor-portal-study/original-navigation.png" alt="Before state 1" style="width:100%;padding-bottom:10px;">
  <figcaption class="image-caption">Original navigation, centering Marketing Materials.</figcaption>
</figure>

The original name for our archive of marketing toolkits and brochures was "Library." Aiming to be more descriptive, I changed it to "Marketing Materials" and tested my new name by asking Advisors to find a brochure or flyer. 

A whopping *none* of the Advisors went to the right page first, mostly choosing "Policy Documents" instead. When asked, Advisors didn't seem to consider flyers and brochures related to marketing.

### After: clear, organized main navigation
<figure class="image">
  <img src="/image_samples/medavie/advisor-portal-study/new-navigation.png" alt="After state 1" style="width:100%;padding-bottom:10px;">
  <figcaption class="image-caption">New navigation, centering Advisors' priority: policies. Marketing Materials renamed to Reference Materials.</figcaption>
</figure>

* The new name, "Reference Materials," aligns with the name of our familiar and widely-used Reference Toolkits, implying a slightly broader scope. 
* Advisors downplayed their usage of these materials. We moved "Reference Materials" to the end of the main navigation menu to bring "Policies" front and center.
* The new navigation includes shortcuts to three frequently used external sites: forms, reports and the Group Admin Portal, a related set of tools.

## Improving document search
### Before and after: simplifying Reference Materials page
{{< slideshow id="marketing" from="images_marketing_materials" >}}

### Before and after: removing unnecessary toggle on Policy Documents page
{{< slideshow id="policy_docs" from="images_policy_docs" >}}

## Driving alignment and delivering impact

This study became the turning point for the project. By grounding design decisions in evidence, we replaced months of opinion-driven debate with a clear, shared direction. We used our findings to bring product, design and business stakeholders into alignment around a policy-first navigation model and an advisor-centered experience.

### Key outcomes
* Rebuilt the portal's information architecture to match how advisors actually think and work
* Simplified navigation and terminology, making high-frequency tasks like finding policies, forms, and renewal dates faster and more intuitive
* Reduced advisors' reliance on account executives by improving self-serve access to critical tools and documents
* Accelerated decision-making by resolving stakeholder conflicts and unblocking the roadmap
* Established a user-centered foundation that shaped the MVP and future feature development

By uncovering advisors' real mental models, we didn't just improve usability: we defined the product's strategic direction and gave stakeholders the confidence to move forward.