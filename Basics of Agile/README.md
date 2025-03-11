# Basics of Agile
## Table of Contents
- [Agile model/methodology/approach](#agile-model-agile-methodology-agile-process)
- [Scrum](#scrum)
    - [Scrum Roles](#scrum-roles)
    - [Scrum Terminology](#scrum-terminology)
    - [Scrum Board](#scrum-board)
    - [Definition of Ready (DoR) & Definition of Done (DoD)](#definition-of-ready-dor--definition-of-done-dod)

## Agile model/ Agile methodology/ Agile process
Agile is an Iterative and Incremental Approach.
The process of Requirement collection, design, coding, testing and deployment is repeated again and again. We add small amount of features to the existing product over iterations.
### Principles of Agile
- The customer should not have to wait until the entire software is complete. 
- The development team delivers small portions of the software after developing and testing them while the customer is using the software.
- We should be able to accomodate requirement changes easily.

There will be good communication between the Customer, Business Analyst, Developers and Testers.

### Advantages
- Requirement changes are allowed in any stage of development (or) We can accomodate requirement changes in the middle of development.
- Releases will be very fast (Weekly).
- Customer need not wait for a long time.
- Good communication between team.
- It is a very easy model to adopt.

### Disadvantages
There is less focus on design and documentation since we deliver the software very fast.

## Scrum
Scrum is a framework through which we build software product by following Agile Principles.

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.neonrain.com%2Fwp-content%2Fuploads%2F2017%2F02%2Fscrum_process_afa_5000.jpg&f=1&nofb=1&ipt=988c4f27d5f025796cc14755f417a314d529beaff02e32aadb1d29401e17402b&ipo=images" alt="Scrum Framework at a glance" style="width:100%;">

### Scrum Roles
Scrum includes a group of people called as scrum team. Normally consists of 5-9 members.
- [Product Owner (PO)](https://www.geeksforgeeks.org/product-owner-definition-roles-and-responsibilities/)
- [Scrum Master (SM)](https://www.geeksforgeeks.org/scrum-master/)
- Developer Team (Dev)
- Tester team (QA)

#### Product Owner
- Define the features of the product
- Prioritize features according to market value
- Adjust features and priority in every iteration as needed
- Accept or reject work results.

#### Scrum Master
- The main role is facilitating and driving the agile process

#### Developers and QA
- Develop and Test the software

### Scrum Terminology
- **User Story** - A feature/module in a software is called a [user story](https://www.atlassian.com/agile/project-management/user-stories).
- **Epic** - Collection of user stories. [Read more](https://www.atlassian.com/agile/project-management/epics)
- **Product Backlog** - Contains list of user stories. Prepared by product owner. [Read more](https://www.atlassian.com/agile/scrum/backlogs)
- **Sprint/Iteration** - Period of time to complete the user stories, decided by the product owner and team, usually 2-4 weeks of time. [Read more](https://www.atlassian.com/agile/scrum/sprints)
- **Sprint planning meeting** - Meeting conducts with the team to define what can be delivered in the sprint and duration. [Read more](https://resources.scrumalliance.org/Article/sprint-planning-meeting)
- **Sprint Backlog** - List of commited stories by Dev/QA for specific sprint. [Read More](https://www.atlassian.com/agile/project-management/sprint-backlog)
- **Scrum Meeting** - Meeting conducted by Scrum Master everyday for 15 minutes. Called as **[Scrum call/Standup Meeting](https://meetingnotes.com/blog/what-are-scrum-meetings)**.<br> Covers questions like:
    - <code>What did you do yesterday?</code>
    - <code>What will you do today?</code>
    - <code>Are there any impediments in your way?</code>
- **Sprint retrospective meeting** - Occurs once a sprint at the end of the sprint. The entire team, including the Scrum Master, Product Owner should participate to discuss what went wrong and what went good and what should be changed in the upcoming sprints. [Read more](https://www.atlassian.com/team-playbook/plays/retrospective)
- **Story Points** - Rough estimation of user stories, will be given by Dev&QA in the form of [fibonacci series](https://www.geeksforgeeks.org/fibonacci-sequence/). [Read more](https://www.atlassian.com/agile/project-management/estimation)
- **Burndown chart** - Shows how much work is remaining in the sprint. This is maintained by the scrum master daily.

### Scrum Board
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fhygger.io%2Fwp-content%2Fuploads%2F2019%2F11%2F7.png&f=1&nofb=1&ipt=f07f29637aa8420b49bc7568c98eb6a79860095251947d05c384ef38806ca933&ipo=images" alt="Scrum Board" style="width:100%;">

### Definition of Ready (DoR) & Definition of Done (DoD)
#### Definition of Ready (DoR)
- User Story is clear
- User Story is testable
- User Story is feasible
- User Story is defined
- User Story is Acceptance criteria defined
- User Story dependancies identified
- User Story sized by development team
- Scrum team accepts User Experience Artefacts
- Performance criteria identified, where appropriate
- Team has a good idea what it will mean to Demo the User Story

#### Definition of Done (DoD)
- Code produced (All 'to do' items in code completed)
- Code commented, checked in and run against current version in source control
- Peer reviewed (or producedd with pair programming) and meeting development standards
- Builds without errors
- Unit test written and passing
- Deployed in system test environment and passed system tests
- Passed UAT (User Acceptance Testing) and signed off as meeting requirements
- Any build/deployment/configuration changes are implemented/documented/communicated
- Relevant documentation/diagrams produced and/or updated
- Remaining hours for task set to zero and task closed