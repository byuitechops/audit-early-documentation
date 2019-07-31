# Project Capture Document for Audit: Groups 
#### *Authors:* Lucas Wargha, John Reiley, Eric Julander
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 09:30*

## Background

 The "Groups" audit is part of a big audit project that BYUI IT department is working on. The purpose for this audit is to test that groups were set up correctly during each semester. Course Groups have four main components which will be tested thoughout the audit. 
 These components are:
 - Group Categories
 - Groups Preferences and Configurtions
 - Group Discusssion Associations
 - Group Assignment Associations

 These sub audits will be explained more indepth later in the document. 

-----

## Definition of Done

   This audit will be complete once it is able to preform a proper audit on all four aforementioned categories.

-----

# Requirements

## General Requirements

## Group Category Sub-audit
**Pass:**
When the audit finds no missing groups or conflicting group configurations, it will emit a success.

**Failures:**
A failed audit can be caused by multiple different scenarios.
<!--
    
-->
- <span style="color:red"> Missing Group Failure</span>: If the coppied course is missing a group from the blueprint it will emit this failue.

- <span style="color:red"> Mismached Configuration Failure</span>: If the corresponding groups have grop configurations that conflict it will emit this error.


**Warning:**
<span style="color:yellow">No Group Categories Warning:</span> If both the blueprint and the coppied course have no group categories it will emit this warning. It seems like this should be an unusual occurance and might be an error. 

## Groups Preferences and Configurtions Sub-audit
- **Pass:** If the groups permissions, configurations, and associated group categories match those of the blueprint, it will emit a success.
- **Failures:**

    <span style="color:red"> Mismatched Group Category Fail</span>: If a group is assigned to a group category that is different than that of the associated blueprint course, it will emit this failure. It will compare the `name`, `is_public`, `followed_by_user`, `join_level`, `context_type`, and `permissions` attributes of the group object.

    <span style="color:red"> Mismatched Permission Configuration Fail</span>: If a group's permissions and configurations differ from that of the blueprint, it will emit this error. 
## Group Assignment Associations Sub-audit
- **Pass:**
    - Both BP and CC have null values for the `group_category_id` member of the **`assignment`** object.  
    - Both BP and CC have values for the `group_category_id` AND same values for `name`, `role`, `self_signup`, `auto_leader`, and `group_limit` members of the **`group_category`** object. 

- **Fail:** Only BP or CC have a null value for the `group_category_id` OR unmatching values for `name`, `role`, `self_signup`, `auto_leader`, and `group_limit` members of the **`group_category`** object.  


## Group Discusssion Associations Sub-audit
- **Pass:**
    - Both Blueprint and Course Copy have null values for the `group_category_id` member of the **`discussion_topic`** object or they are both linked back to the same group category.  
    - Both Blueprint and Course Copy have values for the `group_category_id` AND same values for `name`, `role`, `self_signup`, `auto_leader`, and `group_limit` members of the **`group_category`** object. 

- **Fail:** Only BP or CC have a null value for the `group_category_id` OR unmatching values for `name`, `role`, `self_signup`, `auto_leader`, and `group_limit` members of the **`group_category`** object.



### Input Requirements
#### API Calls
##### Blueprint Subscriptions API Call
This is how we find all of the information relating to the course blueprint.

    GET /api/v1/courses/:course_id/blueprint_subscriptions

##### Group Categories
We need to ensure that all of the groups stay associated with the proper group category. We need to make this API call to get all of the group categories for the courses.

    GET /api/v1/courses/:course_id/group_categories

##### Group API Call
This gives us a list of all groups in the course.

    GET /api/v1/courses/:course_id/groups

##### Discussion Topics API Call
This gives us a list of all discussion topics in the course.

    GET /api/v1/courses/:course_id/discussion_topics

##### Couse Assignments API Call
This gives us a list of all the associated assignments in the course.

    GET /api/v1/courses/:course_id/assignments


<!-- {
  "name","is_public","followed_by_user","join_level","context_type","permissions"
} -->
#### Source of Inputs
All inputs will be received via the encompassing Audit Project.

#### Definition of Inputs
<!-- TBD: do not fill out just yet -->
- Course Id to run this audit on.
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

<!-- -----

## Questions/Concerns

    Against what are we testing the groups? What properties should we be checking when checking groups and what defines a warn/pass/error in this audit? 
    -Properties that would be evalulated in this audit.
    1)name
    2)max_membership
    3)join_level
    4)is_public
    5)description
    6)member_count
    7)context type ?
    8)leader == NULL
    9)concluded == false
----- -->

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By: Jake Schwantes* 
#### *Approval Date: 31 July 2019*
