# Key Components Doc for Audit: Disscussion Associations
#### *Author: John Reiley*
#### *Date: July 17, 2019*

# Preliminary Design

## Magic Box Chart

![alt text](images/discussion-associations.jpg)

<!-- Think through the process as much as makes sense, and then create a magic box chart with the whiteboard and place it here. -->

## Explanation of Design
1. An API call will be made to the endpoint `/courses/:course_id/blueprint_subscriptions` which returns a blueprint subcription object like the following:  

    `[ { "blueprint_course": { "id": 35764 } } ]`

2. The id member value will then be extracted. The following API call will then be made with the course id and course blueprint id: `/courses/:course_id/discussion_topics` .

3. The `group_category_id` member of the `discussion_topic` objects for the blueprint and course will be compared.  If **both** values are **not null**, then the `group_category` object will be fetched using the following API call: `/courses/:course_id/group_categories` .

4. The following members of the `group_category` object will then be compared:
    - `name`
    - `role`
    - `self_signup`
    - `auto_leader`
    - `group_limit`
 
### Used Libraries
- Canvas Wrapper



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

### *Insert Component name here*

Diagram:

*Insert Diagram Here*

Explanation:

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

### *Insert Module Name Here*
#### How to Test:





-----

#### *Full Design Approved By:* 
#### *Full Design Approval Date:*


<!-- Diagram Types:
 - Data Flow (I think this will be the most popular)
 - Structure Charts (This is really good for showing input and output of every function)
 - UML Class Diagram (a must for object oriented projects) -->
