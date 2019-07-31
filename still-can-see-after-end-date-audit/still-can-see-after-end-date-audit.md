# Project Capture Document for Audit: _Still Can See After End Date_ 
#### *Author: Kaylee Hartzog & Seth Bolander*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 10, 13:52*

## Background

After a course ends, students want to be able to still access the course even when they are not taking it anymore. Not being able to go back to that course would mean that the student would not be able to look back and see what they did and learned in the course. This audit will make sure that the course has this ability.

-----

## Definition of Done

The audit needs to be able to successfully test whether a given course does _not_ restrict 'past view' for students. An API call to the course (`/api/v1/courses/{courseCode}`) gives you this information on the `restrict_student_past_view` key, which should be `false`.

-----

# Requirements

#### Pass:

Course object has `restrict_student_past_view` set to `false` or `0`.

#### Fail:

Course object has `restrict_student_past_view` set to `true` or `1`.

#### Warn:

Not sure yet

-----

### Questions/Concerns

- If a student doesn't complete a course, does that mean they are not allowed to see the course after the course ends? (We think yes, but Canvas handles this issue itself).

-----

## Expectations
### Timeline
**Deadline:** 2019 Sep 1

**Priority:** Low

-----
#### *Approved By: Jake Schwantes* 
#### *Approval Date: 30 July 2019*
