# Project Capture Document for Audit: Group Categories
#### *Author:* Eric Julander
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 12:41*

## Background
While copying courses from their blueprints we need to make sure that all groups and their respective configurations get coppied aswell.

-----

## Definition of Done
The project will be complete once it can return audit results that report if there are any groups missing or conflicting configurations within a group.

-----

# Requirements

### General Requirements
#### Success
When the audit finds no missing groups or conflicting group configurations, it will emit a success.

#### Failures:
A failed audit can be caused by multiple different scenarios.
<!--
    
-->
- <span style="color:red"> Mismatched Course Failure</span>: If the course and blueprint are completley different it will throw this failure. The two cannot be compared if they are not the same.
- <span style="color:red"> Missing Group Failure</span>: If the coppied course is missing a group from the blueprint it will emit this failue.
- <span style="color:red"> Mismached Configuration Failure</span>: If the corresponding groups have grop configurations that conflict it will emit this error.


#### Warning:
<span style="color:yellow">No Group Categories Warning:</span> If both the blueprint and the coppied course have no group categories it will emit this warning. It seems like this should be an unusual occuracne and might be an error. 
<!-- What counts as pass/fail/warn? -->
### Input Requirements
#### Source of Inputs
All inputs will be passed in by the auditor.

#### Definition of Inputs
<!-- TBD: do not fill out just yet -->
- The org unit ids of courses and their blueprints to make the comparisons for.
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
Total Time: Approximately 3-5 Hours or about 1 work-day.
#### Day 1
- Work on pulling and requesting all the groups for courses and checking for any missing groups. (≈1-2 Hours)
- Work on comparing the configrations between the respective courses. (≈2-3 Hours)

**Priority:** HIGH

**Deadline:** September 1, 2019

<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

-----

#### *Approved By:* 
#### *Approval Date:*
