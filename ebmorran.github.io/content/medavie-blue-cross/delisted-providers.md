---
title: "Delisted providers in search"
date: 2022-02-10T22:53:58+05:30
draft: false
author: "Elizabeth Morran"
image: /images/map-sample.png
disableMainImg: true
description: 
summary: "An update to our mobile provider search, adding a filter for delisted providers."           
socialShare: false
toc: false
---
<div id="delisted-img-container" style="margin:auto; padding-bottom: 25px;">
<img src="/image_samples/medavie/delisted-providers/description.png" alt="Screenshot describing the delisted provider filter" style="margin: auto; width: 70%;">
</div>

## Request
Sometimes, a healthcare provider will be removed from the Blue Cross network, making their services ineligible for coverage. This can be for various reasons, from legal issues to the provider having retired. Because of contractual obligations with an external stakeholder, we needed to include these providers in our mobile app's provider search feature, while clearly labeling them as ineligible.

On this project, I collaborated with a UX designer to implement the needed changes.

## Constraints
Since there are sometimes sensitive legal issues with a provider becoming ineligible, we needed to avoid revealing or suggesting details. We did not want users to see these providers unless they were specifically looking for them, and we needed to make it obvious which providers were ineligible. 

Finally, we needed to define "ineligibility," but we couldn't say that these providers are necessarily "not covered" or "can't be claimed," since plan members can still claim services from before the time the provider became ineligible.

## Ideation and solution
### Labeling
There were several options available for labeling these ineligible providers, considering what that status covers and the language used by some of our competitors. Options I rejected included:
- **Ineligible:** Used internally at Medavie, but could have negative implications.
- **Inactive:** Potentially misleading, as it may be taken to be mean that the provider is retired.
- **Out of network:** Canadian health insurance companies generally don't have a "provider network," so this might cause confusion.

Ultimately, I decided to suggest the term **delisted**. "Delisted" is neutral-sounding and has the advantage of *not* having any obvious meaning or implications. The user will not read anything into it other than the explanation we provide.

The explanation I provided is:
> Delisted providers may not be eligible for coverage under your Blue Cross plan.

This is intentionally ambiguous, to encourage members to choose providers who are not delisted while not definitively saying their coverage will be denied.

While the designer suggested displaying labels on both active and delisted providers, I thought this would draw unnecessary attention and raise questions about what "active" means. We decided to label only delisted providers in search results.

### Display

<img src="/image_samples/medavie/delisted-providers/brainstorming.jpg" alt="Whiteboard brainstorming options for delisted provider label" style="margin: auto; width: 100%; padding-bottom:10px;">

When it came to displaying these providers in search, I identified three possible scenarios:
1. Search does not return delisted providers
2. Search returns both delisted and active providers
3. Search only returns delisted providers.

<img src="/image_samples/medavie/delisted-providers/draft-options.jpg" alt="Draft options for delisted provider search filter" style="margin: auto; width: 100%; padding-bottom:10px;">

Because delisted providers can't be claimed, we wanted to make sure that users were exposed to the explanation of "delisted provider" before they could toggle them on or off in the search results. Initially, the designer created an alert message that would appear in scenario 2, whenever a search contained delisted providers. My concern with an alert was that it could be intrusive, since most users don't want to see delisted providers. I suggested displaying a filter where both the description of "delisted provider" and the toggle button were collapsed by default, so that they would be exposed at the same time, but only if the user chose to investigate that option.

<img src="/image_samples/medavie/delisted-providers/search-delisted-only.jpg" alt="Search results showing only delisted providers" style="margin: auto; width: 70%; padding-bottom:10px;">

Since the delisted filter and search results are hidden by default, the previous experience would not work for scenario 3. We didn't want to bring the user to an empty search results page. Normally, when a search returns no results, an alert bottom sheet appears requesting the user try again. We repurposed this alert to let them know their search didn't match any active providers, and encourage them to search for something else.

<img src="/image_samples/medavie/delisted-providers/description.png" alt="Expanded filter explaining delisted providers" style="margin: auto; width: 100%; padding-bottom:10px;">

In search results and in the user's list of saved providers, delisted providers would be labeled clearly. On individual provider pages, a prominent alert would appear with a brief explanation that the provider is delisted.

<img src="/image_samples/medavie/delisted-providers/final-flow.jpg" alt="Final flow for delisted provider search" style="margin: auto; width: 100%; padding-bottom:10px;">

We presented our solution to the stakeholders, and it was accepted. 