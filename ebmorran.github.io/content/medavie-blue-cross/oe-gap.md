---
title: "Online Enrolment in Admin Portal"
date: 2024-02-10T22:53:58+05:30
draft: true
author: "Elizabeth Morran"
image: /image_samples/medavie/oe-gap/flowchart.png
disableMainImg: false
description: 
summary: "Upgrading our Group Admin Portal to allow employees to enrol in their own plans."           
socialShare: false
toc: 
---

## Request
The Group Admin Portal (GAP) is a Medavie portal for Group Administrators to manage their groups, plan members and benefits. "Group Administrator" (GA) refers to anyone at a company or other organization who's responsible for overseeing their benefit plans. Often, this will be an HR representative, but at smaller companies it may be the business owner or an office administrator.

Individually adding the personal details of employees to a plan can be tedious, so Medavie offers a pre-existing solution called Online Enrolment, where employees are invited to fill out their own personal information online, saving the GA time and reducing data entry errors. At present, the GA can offer Online Enrolment by sending Medavie a spreadsheet of employee names and email addresses to send the invitations. 

The purpose of this project is to add Online Enrolment features to GAP, so that GAs can add employees, track online enrolment progress and finalize details within the portal.

## Constraints
* Two existing systems with their own features and states
* We have no ability to change anything about the OE experience itself in any way: we are stuck with whatever it allows us to input, whatever data it already outputs, and however it works for the member
* It was determined by stakeholders that all OE features would be a modification of the current "Add Member" experience
* Current GA "action log" somewhat mysterious: adding OE statuses to this can make it even more confusing, especially since current OE statuses have same/similar names with different meanings
* GA normally creates plan details up front, but since these depend on employee-entered information in OE, the plan information needs to be added at the end before finally submitting everything to Medavie's system
* Balancing GA vs member experience (when to allow editing details, consequences of editing)
* Invitation email may be forward-dated, complicating the explanation of what "submit" does


## Ideation and solution

### Understanding the system



Add member:
* Wanted to have a basic explanation of what online enrolment does
* Need to explain the email will be sent on the enrolment start date (not immediately)
* We also need to explain the reminder email. Initially the information provided gave the first option as "one week"... I had to grill them to find out it was actually once per week.
* Making sure the GA understands they need to create the access code.

Summary screen:
* Because the member submits the details of their family member and dependents etc themselves, the GA can't finalize the plan details at this stage. Therefore, all the screens relating to the member's self-entered details *and* the plan details are skipped. We need an explanation of why they suddenly skipped those screens (they may find this disorienting). The full explanation is that there isn't enough information for them to complete the plan details until the employee provides their family and COB info, but I don't want to overload on this screen so I just let them know they'll finalize after online enrolment is complete.

Confirmation screen:
* We need to show success
* We also need to say how this will appear in the action log
* How to cancel it