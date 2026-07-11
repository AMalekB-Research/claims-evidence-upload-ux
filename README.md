# claims-evidence-upload-ux
Insurance Claims — Evidence Upload Redesign

*Company name anonymised — available to discuss 
in interview*

**Role:** Self-initiated UX Researcher & Designer  
**Domain:** Insurance / Personal Injury Claims  
**Tools:** Figma, Observational Research  
**Type:** Concept proposal with business case  

---

## Overview

As a personal injury claims hander at a mid-sized UK motor insurance provider, 
I have seen first hand the pain points both the cutomer and employees experience.
This naturalistic oberservation reseach taks, 
was based directly on these observations over the 2.8 years I have been working in the role, 
handling inbound claims start to finsih along with manning phonelines. 
I identified a critical friction point in the evidence submission
journey that was costing the business an estimated 
£24,000–£38,000 per year in excess handler time.

---
## The Problem Statment 

Policyholders were failing to submit supporting eviednce for their claims, 
inturn causing manual intervetion by handlers,
delays settlements and increased operational costs. 
Despite being willing and cooperative. 
This was not a motivation problem — it was a process design problem.

### Business Impact

| Metric | Current State |
|--------|--------------|
| Handler time per evidence chase | 10–15 mins |
| Annual cost of manual chasing | £24,000–£38,000 |
| Evidence submission channel | Email / WhatsApp |
| GDPR audit trail | Inconsistent |
| Policyholder confusion post-submission | High |


**Key observation:** Policyholders were not 
unwilling to submit evidence.
The process itself was failing them silently.


### Design Process
Empathise → Define → Ideate → Prototype → Test


#### Four Core Failure Points Identified

**1. Email barriers**
File size limits silently blocked photo 
submissions — the most common evidence type — 
with no clear error message shown to the user.

**2. WhatsApp upload failures**
Compressed file resolution made evidence 
unusable. Duplicate sends created confusion. 
No submission confirmation was possible.

**3. Missing contact information**
Incomplete policyholder details prevented 
proactive outreach, forcing handlers to 
wait for inbound contact.

**4. Technical access barriers**
Users with lower digital literacy defaulted 
to phone calls rather than digital submission, 
consuming handler time that better design 
could have prevented.


#### Psychology Frameworks Applied

My BSc Psychology background directly 
informed how I interpreted these observations:

- **Cognitive Load Theory** — the existing 
  process placed excessive decision burden 
  on policyholders at an already stressful moment
- **Learned Helplessness** — repeated failed 
  attempts caused users to abandon digital 
  submission entirely
- **Nielsen's Heuristic 1** — visibility of 
  system status was completely absent, leaving 
  users with no feedback on whether their 
  submission had succeeded or failed


---

## Research Approach

**Method:** Observational research through direct 
daily operational experience

As a Personal Injury Claims Handler I worked 
directly with policyholders throughout the 
evidence collection process, giving me first-hand 
visibility of failure points from both sides — 
the policyholder attempting to submit and the 
handler attempting to receive.

**Core insight:** Policyholders were not unwilling 
to submit evidence. The submission process itself 
created too much friction, confusion, and too many 
points of failure.

**Four failure points identified:**

1. Technical access vulnerabilities in existing 
   upload channels
2. Email file size limits blocking evidence 
   submission entirely
3. WhatsApp upload failures and duplicate sends 
   creating confusion
4. Missing contact information preventing proactive 
   outreach

#### Research Limitations

This research was observational rather than 
formally structured:

- Findings based on pattern recognition across 
  claims handled rather than a controlled study
- Policyholder perspectives inferred from 
  behaviour rather than direct interview
- Business impact estimate based on reasonable 
  assumptions rather than audited operational data

These limitations would be addressed in a 
formal validation phase — outlined in the 
Test section below.

---

## The Solution

A guided evidence upload flow embedded within the 
existing policyholder mobile app, integrated 
directly with the internal claims management CRM.

**User flow:**

<img width="2600" height="620" alt="evidence_upload_flow_v4" src="https://github.com/user-attachments/assets/8e89c933-9894-4455-a94d-5cde65f3e4b0" />
---

## Key Design Decisions

**Push notification trigger**
Removes reliance on policyholder initiative — 
the single biggest reason evidence was not 
submitted. Handler sends request, policyholder 
receives direct prompt. 
Removing reliance on users to remember to submit.

**Structured form with CRM validation**
Policy number, claim reference and date of loss 
validated against database records before 
submission is accepted. Ensures GDPR compliance 
and creates a clean audit trail.

**Explicit error states designed**
Two primary error states built:
- Information not found — guides user to verify 
  their details with specific field-level prompts
- Incorrect file format — clearly communicates 
  accepted formats with a direct retry path

Both error states include contact details for 
immediate handler support, preventing abandonment.

**Confirmation receipt**
Full upload summary emailed to policyholder 
including claim number, upload timestamp, and 
file list. Reduces follow-up anxiety and 
eliminates repeat contact to confirm receipt.

## Figma Prototype

[view screens](figma-screens/)

---

## Projected Business Impact

| Metric | Before | After |
|--------|--------|-------|
| Handler time per evidence chase | 10–15 mins | 0 mins |
| Annual cost of manual chasing | £24–38k | Minimal |
| Evidence submission channel | Email/WhatsApp | In-app guided flow |
| GDPR audit trail | Inconsistent | Automated |
| Policyholder confusion on next steps | High | Eliminated |

---

## What I Would Validate Next

Before development I would run the following 
research to validate design assumptions:

**Usability testing**
- 5-8 policyholders recruited across age groups 
  and varying levels of tech literacy
- Moderated task: submit evidence without 
  handler assistance
- Measure task completion rate, error frequency, 
  and time on task

**Tasks I would set participants:**

1. Submit three pieces of evidence for a 
   fictional claim using only the app
2. Recover from an intentional error state 
   without handler assistance
3. Locate and interpret the confirmation 
   receipt email

**Metrics I would measure:**

- Task completion rate
- Error frequency and recovery rate
- Time on task
- Qualitative feedback on confusion points

**Post-launch metrics (30/60/90 days):**

| Metric | Goal |
|--------|------|
| Evidence upload completion rate | Significant increase vs baseline |
| Inbound calls re: evidence | Measurable reduction |
| Average claim lifecycle | Shorter |
| SLA compliance rate | Improved |
| Handler time on evidence chasing | Near zero |
---

## What This Project Demonstrates

- Research-led problem identification from 
  direct operational experience
- Business impact quantification before 
  design begins
- End-to-end UX thinking — notification trigger 
  through to CRM integration
- Error state design with compliance and 
  audit trail awareness
- Validation planning — knowing what to test 
  before shipping

---

The most valuable lesson from this project was that being closest to the problem 
doesn't mean you automatically see the solution. 
It took stepping back from the daily operational noise, applying a 
research lens, and asking _why_ policyholders were behaving as they were — not just 
_that_ they were — before the solution became obvious.

My psychology background made that shift natural. 
Combining it with UX methodology gave it structure.

