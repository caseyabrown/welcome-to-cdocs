 # Documentation plan - [TeamName]

_**Context**: The following document is an internal Documentation Plan template that can be used for the Incident Response and Observability team, describing how I (the technical writer), plan to completely revamp and launch their entire documentation set._

```
Primary author(s):  Casey Brown
Created: 
Last updated: 
Core Reviewers:  
JIRA ticket: N/A
Goal mapping: TBD
```

## Overview

This document outlines the goals, objectives, and scope of the Incident Response & Observability (IRO) documentation set. The IRO team has expanded the Incident Commander rotation, which means that there are engineers that are new to the incident management process. By revamping the IRO documentation, engineers can feel confident and ready to command any incident. With the new IRO documentation, training courses can also be revamped and point to the new documentation set as a reference.

## Problem

The Incident Response & Observability team must provide Engineers with clear guidelines and procedures for incident management in one, centralized documentation platform.

Once the new documentation is created, the IRO team needs a clear, documented process to keep existing documentation up-to-date and to add any new documentation.

## Goal

The embedded technical writer will eventually need to move on to other docs projects. The goal of this project is to deprecate outdated content, create new documentation, and set the IRO team up for success to maintain the documentation. This documentation plan outlines the following:

* Audit process of existing docs
* New information architecture (IA) for IRO docs
* Migration process (from Confluence to Backstage)
* Docs creation and updating process
* Docs reviewing process

## Documentation audience

<table>
  <tr>
   <td><strong>Persona</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>Engineers
   </td>
   <td>Employees (engineers) that are part of the incident process and need how-to guides to learn more about incident management.
   </td>
  </tr>
  <tr>
   <td>Customer Operations (CustOps)
   </td>
   <td>Employees (Product Support Specialists, Communication Leads, any other roles in CustOps) that would like to understand incident management in the Engineering org.
   </td>
  </tr>
  <tr>
   <td>Incident Response & Observability (IRO)
   </td>
   <td>The team responsible for creating and maintaining the IRO documentation.
   </td>
  </tr>
</table>

## Roles and responsibilities

Content for Incident Response & Observability can be grouped under two major content types:

* Technical (software user guides, API endpoint documentation, etc.)
* Team content (Runbooks, team processes, etc.)

The IRO team is responsible for maintaining the IRO documentation in Backstage. 

## Stakeholders

<table>
  <tr>
   <td><strong>Person or team</strong>
   </td>
   <td><strong>Role</strong>
   </td>
  </tr>
  <tr>
   <td>Incident Response & Observability (IRO) team  
   </td>
   <td>The team responsible for reviewing and maintaining the IRO documentation.
   </td>
  </tr>
  <tr>
   <td>Technical Program Manager
   </td>
   <td>The embed TPM for the IRO team. The TPM will help make sure the team is thinking about documentation when planning their work for the week/month/quarter/year.
   </td>
  </tr>
  <tr>
   <td>Technical Writer
   </td>
   <td>The embed TW will create the initial docs, and then provide guidance on information architecture, technical content, and documentation platforms (Backstage or Confluence).
   </td>
  </tr>
</table>

## Proposal

This proposal has several required phases, beginning with creating an Incident Commander (IC) 1-pager and ending with a process to maintain IRO documentation.

<table>
  <tr>
   <td><strong>Phase</strong>
   </td>
   <td><strong>Details</strong>
   </td>
   <td><strong>Owner</strong>
   </td>
   <td><strong>Status</strong>
   </td>
   <td><strong>Date started/done</strong>
   </td>
  </tr>
  <tr>
   <td rowspan="4" >1 - Create IC one-pager
   </td>
   <td>Conduct IC interviews
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Draft IC 1 pager: Google doc draft 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Publish IC 1-pager (in Confluence and Backstage) 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Collect and implement feedback for IC 1-pager 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td rowspan="2" >2 - Audit Incident Response & Observability wiki in Confluence
   </td>
   <td>Create spreadsheet and audit content with team: &lt;Link to spreadsheet>
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Archive old pages and Confluence spaces
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>3 - Improve the information architecture (IA) for IRO docs entity
   </td>
   <td>Propose new IA for IRO docs and get approval from Manager and IRO team.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>4 - Establish Backstage presence for IRO
   </td>
   <td>Create incident-response-observability-docs entity.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td rowspan="6" >5 - Draft docs for IRO
   </td>
   <td>Send TW newsletter that introduces new docs and Backstage link – noting that it’s early release and we’d like to hear feedback.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Add note to top of every page, signaling that content is <strong>early release</strong>.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Draft and publish docs 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Organize content nav based on new IA in audit spreadsheet.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Host and attend docs bash sessions to get IRO team to review and approve docs.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Create Glean Answers for IRO collection.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td rowspan="4" >6 - Migrate content from Confluence wiki space to Backstage docs entity
   </td>
   <td>As docs are published, remove any outdated content from Confluence.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Keep track of archived pages in Confluence. 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Redirect Confluence docs to docs in Backstage.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Migrate any team content to team section in Backstage.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td rowspan="5" >7 - Deprecate Confluence IRO wiki space
   </td>
   <td>Send TW newsletter that announces deprecation of IRO wiki.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Send announcement in IRO newsletter (or announce in Slack) 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Archive the entire IRO wiki space.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Update any goto links, pinned docs in Slack.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Remove <strong>early release</strong> notes from docs in Backstage.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td rowspan="6" >8 - Process for updating existing docs and adding new docs 
   </td>
   <td>Set up Looker Studio dashboard for IRO docs to keep track of # of page views.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Document the process and workflow updating existing docs and adding new docs. 
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Introduce docs workflow to team.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Implement docs workflow.
   </td>
   <td>Technical Writer
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Continue adding Glean Answers for IRO collection.
   </td>
   <td>IRO team
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Announce in IRO newsletter (or Slack) when new docs are available.
   </td>
   <td>IRO team
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

## Out of Scope

This documentation plan does not include the following: 

* How teams can request for documentation from the IRO team.
* A workflow for updating documentation alongside the CustOps team. CustOps and IRO docs are separate. We don’t recommend that the CustOps team copy and paste docs into their own wiki; rather, they should link out to IRO docs. Backstage is accessible to anyone with an Active Directory account.
* New training is not part of this documentation plan, however, the TW recommends using this new documentation set as guidance for training.

## Questions

* Will the team be willing to contribute an hour a day to updating and writing documentation?

# Resources

* Google Drive folder for IRO doc drafts
* Incident Response & Observability doc audit

## Revisions

1. [date] - Documentation plan created.
2. [date] - Documentation plan edited.
3. [date] - Added dates to Proposal table.