# Project Capture Document for Audit: Locked Files Audit
#### *Author:* Eric Julander
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 12:41*

## Background
While copying courses from their blueprints we need to make sure that files which are locked stay locked and vice versa. This audit will just compare the copied course to its blue print to find any changes.

-----

## Definition of Done
The project will be complete once it can return audit results that report if there are any files which were originally locked but were unlocked during the copy and vice versa.

-----

# Requirements

### General Requirements
#### Success

#### Failures:
A failed audit can be caused by multiple different scenarios.
<!--
    
-->
- <span style="color:red"> Mismatched Course Failure</span>: If the course and blueprint are completley different it will throw this failure. The two cannot be compared if they are not the same.


#### Warnings:
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
Total Time: Approximately 7-11 Hours or about 2-3 work-days.
#### Day 1
- Work on pulling and requesting all the files for courses. (≈1-2 Hours)
- Work on comparing the lock configurations and lock dates for files in the courses. (≈2-3 Hours)
#### Day 2
- Work emmiting the "Mismatched Course Failure" (≈2-3 Hours)
- Various patches and bug fixes" (≈2-3 Hours)

<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

-----

#### *Approved By:* 
#### *Approval Date:*
