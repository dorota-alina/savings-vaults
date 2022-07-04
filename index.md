---
title: "Work plan for documenting Savings Vaults "
menuTitle: "Savings Vaults"
description: "Revolut is releasing a new product feature that lets customers earn interest by saving money in a Savings Vault. Read this blog post for an overview of the feature. Your task is to work with the product team and any other stakeholders to produce comprehensive technical documentation about this new feature. Describe how you would approach this task (max. 600 words)."
author: Dorota Wojcik
date: 2022-06-29
---

Here are the actions I'd take to produce the requested documentation:

## Search and learn

### Scamming

1. Identify available resources on Revolut products, Vaults, Savings Vaults, related features, and its users - internal materials, docs, blog posts, Internet, etc
2. Use the above for a preliminary self-study - quick research

### Identify stakeholders

1. Identify Project Lead (Technical Lead), Product Owner, Feature Owner, and possibly other product/ marketing/ sales persons with some expertise on Savings Vaults.
2. Identify the technical engineers/ devs working on the feature who can support you (SMEs).
3. Contact all of them and agree on a suitable form of cooperation:
   * Preferably, a recorded call (which could be stored and/or shared, but, most of all, played back).
   * Email
   * Chat
   * Sharing docs/ materials via a CMS.

### Define requirements

1. Define your audience (internal Revolut devs, external devs, regular Revolut end users, etc). - consult Product Owner or a counterpart
2. Define the scope - consult Product Owner or a counterpart about what type of docs specific users would need:
   * Getting started?
   * Conceptual feature description?
   * Use cases/ User journeys? What specifically?
   * How-tos/ tutorials (explaining how to use Savings Vaults)?
     * Via UI?
     * Via CLI?
     * APIs?
   * Operational manuals (explaining how to get Savings Vaults up and running (installation, integration, configuration, etc)
     * Via UI? (highly unlikely)
     * Via CLI?
     * APIs?
* API docs?

## Get hands-on practice

Test Savings Vaults yourself.
1. Depending on how the feature is available (dev environment, test/UAT env., pre-prod/staging env., etc), set up your local environment or acquire access to a relevant website. To do that, use info in README files and, if needed, seek support from the SMEs.
2. When set up, check out all possible use cases and journeys that the users might want to take.

### Deep dive into the subject

Self-study focused on the part to be covered in the docs:

* Use existing internal or external resources.
* Request the introduction and demo of the Savings Vaults feature from the SMEs.
* Check if there's already been any similar/parallel documentation from  Revolut or its competitors and gather good practices if any.

## Down to writing

### Early draft

1. Try to produce an initial draft or at least docs plans and check what info you're missing.
2. Consult the initial draft - request support from the SMEs in the agreed form to acquire the missing info.

### Mature draft

Refine your initial draft and produce a proper one based on the collected info.

## Assure the quality

### Test the docs

1. Test how-tos, tutorials, instructions, and any procedural parts yourself.
2. Request testing the same from the QA team.

### Review & approval

1. Distribute the draft for review to the agreed stakeholders (preferably different from SMEs): devs, engineers, architects, product/ marketing/ sales folks.
2. Update the docs according to the comments received after the testing and the review.
3. Request the final approval from the agreed stakeholder (Project Lead, Tech Lead, or similar).

## Publish the docs

### Merge (GitHub)

1. Merge all relevant PRs (GitHub) to the release branch and tag your branch if needed.

### Deploy (Jenkins)

1. Publish your docs to the internal preview (if any) triggering a relevant pipeline in Jenkins.
2. Verify the preview for any possible mistakes and correct them if needed.
3. Publish your docs to the public view triggering a relevant pipeline in Jenkins.
4. Verify the website for any possible mistakes.
