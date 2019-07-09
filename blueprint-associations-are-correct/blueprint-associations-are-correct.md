# Project Capture Document for Audit: Blueprint Associations are correct 
#### *Author: Cameron Thompson*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*
## Background

Durring course copy, courses could have their blueprint associations disorganized from what they are supposed to be. This causes a great deal of headache to fix the blueprint associations, taking time and money from the University and its employees. 

-----
## Definition of Done

This audit will check the courses to make sure that the correct courses that are dirived from a blueprint are children of the correct blueprint. If not then the audit will flag the course to be connected to the correct blueprint course. Additionaly, if a course is connected to a parent blueprint, then the audit will check to make sure it is the correct parent course for the child course. For example, if FDMATH 108 is a child course, the audit will check to see if the parent course is the semester blueprint of FDMATH 108.

-----
# Requirements
### General Requirements
<!-- What counts as pass/fail/warn? -->
A course will pass when: The child courses match the correct parent blueprint course

A course will fail when: When a child course is not connected to a parent blueprint or the course is matched with the incorrect blueprint parent course.

A course will warn when: When a semster blueprint doesn't have children (No sections created for the course)
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
#### *Approved By:* 
#### *Approval Date:*
