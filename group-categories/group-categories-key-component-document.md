# Key Components Doc for Group Categories Audit
#### *Author: Eric Julander*
#### *Date: July 10th, 2019*

# Preliminary Design

## Magic Box Chart

![Group Categories Magic Box Chart](images/group-categories-magic-box.jpg)

<!-- Think through the process as much as makes sense, and then create a magic box chart with the whiteboard and place it here. -->

## Explanation of Design
<!-- Add explanation of the Magic Boxes image above. Answers to the prompts below may also be appropriate to include here. -->
The audit requires the org unit ids for the blueprint course and the course copy. It will compare the two courses to make sure that they are the same. After that it will make sure that there are no missing groups and that all of those group's configurations are the same. After that, the program will emit failures, successes, and warnings based off of the results recieved from the previous audit components.

### Used Libraries
None
## Things to Consider Before Getting Project Approved
- Are there any approved libraries that I can use? [Link to Approved Library List]
- Are there design patterns that will help?  [Link to Design Patterns]
- Can I design it so that it is a general tool instead of a specific solution?
- How can it be easily expanded?
- What does the minimum viable product look like?

## Prep for Learning Phase
- What do I need to learn
- How will I learn it
- What will I do to learn it (prototypes/tutorials/research time limit?)
- What is the definition of done for my learning process
- How do I measure the progress of learning
- Is there a deliverable that can be created during the learning process?

-----

#### *Preliminary Design Approved By:* 
#### *Preliminary Design Approval Date:*

# Full Design

## Component Diagrams
<!-- Diagrams and companion explanations for all Key Components.
These would include information about inputs, outputs, and what a function does for every major function. -->

<!-- For each component, the following template will be followed: (In other words, the template below will repeat for each component)-->
### Object Definitions:
#### GroupCategory:
This holds the same structure as the Canvas Group Categories Object.
https://canvas.instructure.com/doc/api/group_categories.html
#### Status Object
- *Status* - Contains a value describing the success of the operation ( 0 = pass, 1 = warning, 2 = failure)
- *Message* - The message accompanying the status of the operation.

### Methods:
#### GetFileList
This grabs a GroupCategory object from the canvas API.

##### Parameters: 

- *AuthToken*: The API Token for canvas. 
- *OrgId*: The org unit id for the course.

##### Outputs:

- *GroupCategory*: A POCO which holds the data of a Canvas Group Category Object.

#### CoursesMatch (Courses are the Same)
This checks wether the two courses are the same. If the courses are completley different, it will emit a "Mismatched Course Failure" though the status object. If the courses are the same it will emit a "success" through the status object.

##### Parameters: 

- *BlueprintCourse*: GroupCategoryObject for the blueprint course. 
- *CopiedCourse*: GroupCategoryObject for the copied course.

##### Outputs:

- *StatusObject*: The status of the preformed operation (pass, warning, failure)

#### GroupsMatch (No Groups Missing)
This checks that both the blueprint and the copied courses have matching group categories. If the categories are not matching, it will emit a "Missing Group Failure" though the status object. If neither the blueprint or the course copy have group categories, it will emit a "No Group Categories Warning" through the status object. If the courses have matching group categories, it will emit a success through the status object.

##### Parameters: 

- *BlueprintCourse*: GroupCategoryObject for the blueprint course. 
- *CopiedCourse*: GroupCategoryObject for the copied course.

##### Outputs:

- *StatusObject*: The status of the preformed operation (pass, warning, failure)

#### ConfigurationsMatch (Configurations are the Same)
This checks that both the blueprint and the copied courses have matching group category configurations. If the configurations are not matching, it will emit a "Mismached Configuration Failure" though the status object. If the courses have matching group category configurations, it will emit a success through the status object.

##### Parameters: 

- *BlueprintCourse*: GroupCategoryObject for the blueprint course. 
- *CopiedCourse*: GroupCategoryObject for the copied course.

##### Outputs:

- *StatusObject*: The status of the preformed operation (pass, warning, failure)

#### EmitError
This emits an error message to insert into the AuditReport object.

##### Parameters::

- *StatusObject*: A status object to convert into a canvas audit report message.

##### Outputs:

- *AuditReportMessage*: The error message to insert into the final AuditReport
#### EmitWarning
This emits an warning message to insert into the AuditReport object.

##### Parameters::

- *StatusObject*: A status object to convert into a canvas audit report message.

##### Outputs:

- *AuditReportMessage*: The warning message to insert into the final AuditReport
#### EmitSuccess
This emits an success message to insert into the AuditReport object.

##### Parameters:

- *StatusObject*: A status object to convert into a canvas audit report message.

##### Outputs:

- *AuditReportMessage*: The success message to insert into the final AuditReport

*Insert Explanation here*

<!-- For a future release:
## Test Plans
For each major function the test plan template will be as follows (in other words the template below will repeat for each test) 
### *Insert name of component here (e.g. convertIdToCourseObject function)*
#### Test 1: *Insert Test name here*
Summary: 
 *Insert Test Summary Here*
 Type: *Insert Type here (Unit Test, Manual Test, Selenium/Puppeteer test (Overkill?))* 
Procedure:
1. *Insert Steps here*
1. *and here*
1. *and here*
Expected Outcome:
*Insert Expected Outcome here*
-->

## Test Plans

### GetFileList
#### How to Test:
This will grab the contents of a sandbox course and compare it to an exisiting object of that course. If they match, the test will pass.
### CoursesMatch (Courses are the Same)
#### How to Test:
We will pass in two courses. One course will be an actual copy while the other course will be completley different. We will compare both to the blueprint. The different course should fail and the copy should passs.
### GroupsMatchMatch (No Groups Missing)
#### How to Test:
We will pass in two courses which are identical and two which are nearly identical. The only difference will be that one course will have a group category that does not exist in the other. If the test works properly, it will emit a success for the former and a failure for the latter. We will then pass in two identical course objects which have not groupcategories. This should emit a warning status object from the function.

### ConfigurationsMatch (Configurations are the Same)
#### How to Test:
In this test we will pass in two courses which have matching group category configurations and two courses which have conflicting configurations. The former should emit a success while the latter should emit a failure.
### EmitError
#### How to Test:
We will pass in a status object flagged as an error. If it works properly, the function should pass an Auditor Error Message.
### EmitWarning
#### How to Test:
We will pass in a status object flagged as a warning. If it works properly, the function should pass an Auditor Warning Message.
### EmitSuccess
#### How to Test:
We will pass in a status object flagged as a success. If it works properly, the function should pass an Auditor Success Message.





-----

#### *Full Design Approved By:* 
#### *Full Design Approval Date:*


<!-- Diagram Types:
 - Data Flow (I think this will be the most popular)
 - Structure Charts (This is really good for showing input and output of every function)
 - UML Class Diagram (a must for object oriented projects) -->



