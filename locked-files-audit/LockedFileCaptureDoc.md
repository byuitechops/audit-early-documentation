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
Success will be defined as having each lock configuration for the files in the copied course correspond with those in the blueprint.
#### Predefined Failures:
A failed audit can be caused by multiple different scenarios.
<!--
    "locked_for_user": false
    "lock_at": "1776-07-04T06:59:56Z",
    "unlock_at": "1770-03-05T06:59:56Z",
    "locked": false,
-->
- <span style="color:red"> Mismatched Course Failure</span>: If the course and blueprint are completley different it will throw this failure. The two cannot be compared if there are too many mismatched elements.
- <span style="color:red"> Mismatched Lock/Unlock Date Failure</span>: If the file in the copied course is not assigned a lock/unlock date but the corresponding blueprint file does. The opposite also applies.
- <span style="color:red"> Mismatched Lock Configuration Failure</span>: Each file has the settings ```locked_for_user``` and ```locked```. The former determines if a file is locked for students while the latter determines if it is locked for everbody in general. These two preferences need to correspond with the blueprint courseor it will emit an failure.

#### Predefined Warnings:
<span style="color:yellow">Missing File Warning:</span> A warning will be issued when it finds any content which is not found in both courses. For example: Suppose there is a file that is locked in the blueprint, but that file cannot be found in the copied course. When this happens it will emit a missing file warning.
<!-- What counts as pass/fail/warn? -->
### Input Requirements

#### Source of Inputs
All inputs will be passed in by the auditor.

#### API Calls:
Blueprint Subscriptions
> GET /api/v1/courses/:course_id/blueprint_subscriptions

Course Files
> GET /api/v1/courses/:course_id/files

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
- Work on comparing the lock configurations for files in the courses. (≈2-3 Hours)
#### Day 2
- Work emmiting the "Mismatched Course Failure" (≈2-3 Hours)
- Various patches and bug fixes" (≈2-3 Hours)

<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

**Priority:** HIGH

**Deadline:** September 1, 2019

## Questions and Concerns:
Locked files have lock and unlock dates. These dates are sure to be innactuate if we are copying them from the blueprint. Do we need to check for the accuracy of these items? If so, how could we go about doing that?

-----

#### *Approved By: Jake Schwantes* 
#### *Approval Date: 25 July 2019*
