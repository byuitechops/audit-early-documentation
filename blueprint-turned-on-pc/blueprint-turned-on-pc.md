# Project Capture Document for Audit: Blueprint Turned On
#### *Author: Cameron Thompson*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*
## Background

During copy, a semester blueprint might not get turned on. Making copies for the semester sections is okay but any changes to the semester blueprint might not carry over to the semester sections, making the students miss important changes to their course.


-----
## Definition of Done

This audit will go and check to see if the semester blueprint has the blueprint setting turned on. 

-----
# Requirements
### General Requirements
<!-- What counts as pass/fail/warn? -->
A course will pass when: A semester blueprint has the blueprint setting turned on. 

A course will fail when: A semester blueprint has the blueprint setting turned off.

A course will warn when: A course that isn't a blueprint has the blueprint setting turned on.

---
### Input Requirements
#### Source of Inputs
All inputs will be received via the encompassing Audit Project.
#### Definition of Inputs
<!-- TBD: do not fill out just yet -->
- Course Id(s) to run this audit on.
---
### Output Requirements
#### Destination
Returned to the invoked method from the Audit Project.
#### Definition of Outputs
<!-- TBD: do not fill out just yet -->
- Results of the Pass/Fail/Warn status of this audit and associated messages.
---
### User Interface
An extension of the base Audit class from `namespace Byui.CourseAudits.Business.Model.Audits`.
#### Type:
Audit Project class
-----
## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
2019 Sep 1
<!-- What priority is this audit? -->
Med
-----
#### *Approved By: Jake Schwantes* 
#### *Approval Date: 22 July 2019*
