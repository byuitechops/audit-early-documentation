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
Success will be defined as having each lock status for the files in the copied course to match those in the blueprint.
#### Predefined Failures:
A failed audit can be caused by multiple different scenarios.
- <span style="color:red"> Http Connection Error</span>: This will be emited when the audit script fails to connect to the internet, find the courses with the specified codes, is missing authentication, or any other network issues like this. 
- <span style="color:red"> Mismatched Course Error</span>: If the course and blueprint are completley different it will throw this error. The two cannot be compared if there are too many mismatched elements.
- <span style="color:red"> Mismatched Lock Configuration Error</span>: If the copied course has a lock configuration which differs from the blueprint, it will emit this error for the course.

#### Predefined Warnings:
<span style="color:yellow">Missing File Warning:</span> A warning will be issued when it finds any content which is not found in both courses. For example: Suppose there is a file that is locked in the blueprint, but that file cannot be found in the copied course. When this happens it will emit a missing file warning.
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
Total Time: Approximately 11-18 Hours or about 4 work-days.
#### Day 1
- Work on pulling and requesting all the files for courses. (≈4-6 Hours)
#### Day 2
- Work on emitting the "Http Connection Error" (≈1-2 Hours)
- Work on comparing the lock configurations for files in the respective courses. (≈2-3 Hours)
#### Day 3
- Work on emmiting the "Mismatched Lock Configuration Error" (≈1-2 Hours)
- Work on emmiting the "Missing File Warning" (≈1-2 Hours)
#### Day 4
- Work emmiting the "Mismatched Course Error" (≈2-3 Hours)
- Various patches and bug fixes" (≈2-3 Hours)

<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

-----

#### *Approved By:* 
#### *Approval Date:*
