# Project Capture Document for Audit: Student Enrollments Are Correct
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 4:46*
## Background
<!-- 
Explain the context of the problem.
Explain key terms/words, words that may be unfamiliar to a new hire.
Do Example: 
    
    Corey and his team have been manually going through the html for all images in canvas and entering alt image text.
    This has been very time consuming.
Don't Example:
    Without project templates, we have been left with readmes that share all different kinds of data, and some of them were missing key
    points of data. Additionally, we have no standard for code templates. We don't want to add a lot of overhead to setting up a project
    with templates and code setup.
-->
-----
Some classes after their conversion could have a problem with not having any students enrolled. This could be an issue because students need to have the right roles and if that's not the case we would have problems. We need to avoid this issue. This audit will get the api call to get student enrollments for all given course codes and will ensure that students are enrolled with the right role. 

## Definition of Done
<!-- 
What is/are the project outcome(s)?
("Can you give me one sentence describing what you want done?")
We are trying to clean up the yard by Mow, Edge, and Rake.
Do Example:
    We are creating a tool to find all images that are in need of alt text in canvas 
    which will automate this process by showing an image and prompting for alt text.
Don't Example 2:
    We are using yeoman to create a generator that will add all needed documentation and
    set up the code with all needed scripts, templates, and integrations.
-->
-----
We are creating this audit so we can check whether students have the right role in given courses. We will be making the API call to get the students and their roles, then making sure that the roles are correct. If there is a student with an incorrect role, it will fail. We will also warn of suspicious behaivor (see below.)
### General Requirements
<!-- What counts as pass/fail/warn? -->
Pass: Students have the student role

Warning: If there are no teacher roles, if there are all students, if there are not students enrolled

Fail: If a student doesn't have student roll.
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
<!-- What priority is this audit? -->
-----
The deadline is Sep 1, 2019.

The priority is high?
#### *Approved By:* 
#### *Approval Date:*
