# life-stream-model-api
This application exposes the API for the Life Stream business model.
It is was a conscious choice to separate the business API from the user interface code and resources as is common in a typical Mean application.
This is only a MongoDB, Express and Node application. Thus, the user interface Angular or otherwise will be implemented in other packages and application(s).

I fell like the organizational features of most GTD Applications/PIMs/Todo Applications/List Applications are to limiting.
I want to be able to organize items with different simultaneous schemes to visualise what I am accountable for in many different ways with having the modify the items itself.

An additional purpose of this application is to demonstrate the use of lower level libraries and APIs over integrated full stacks, code generation and scaffolding.
Full stacks are great but one of the objectives of this project is to demonstrate uses of the foundational libraries such as Node, Express and MongoDB.

## Life Concerns
I am kicking around a few names for the generalized concern that is the core data object.
- Items
- Elements
- Things
 
### Examples of specific Concerns:
- ToDos
    - Name
    - Modification Dates
    - Priority
    - Priority Modification Dates
    - Star
    - Star Modification Dates
    - Completed
    - Completed Date
    - Start Date
    - Due Date
    - Duration
    - Alert
    - Recurrence
    - Picture Picture(s)
    - Audio Clip(s)
    - Location(s)
    - Note
    - Action (create a button to activate a...)
        - Call
        - Message
        - Mail
        - Visit
        - URL
        - Google
- Tasks
- Notes
- Ideas

### Common Concern features and properties
All concerns shall have the following properties and features.
- Creation Date
- Modification Date
- An ordered list of Tags and the date the Tag was added.
- May optimize it's Tags.
- In exactly one Folder.

### Activities to do with Concerns
- Prioritization
- Planning
- Workflow
- Gantt chart
- Mind Mapping

## Tags
### Examples of specific Classes of Tags that could be applied to Concerns:
- Concern states
    - Done
    - Paused
    - Blocked
    - Deferred
    - Communicate
    - In Progress
    - OBE (Overtaken By Events)
    - ROT (Ran Out of Time))
- Contacts/People
    - Family Members
    - Team Members
- Business Associativity *I have several business entities. What business entity is this related to?* 

### Tag Features
- All tags shall be able to be members of groups and act as groups themselves.
- Tags are simple and are logically named nodes in a graph.
    - The Tag Name
    - A Ordered list of Parent Tags
    - An Ordered list of child Tags
    - A Tag an not be an immediate parent or child of itself.
    
## Folders
Folders are simply a hierarchical organization mechanism where folders have one (or no) parent and an ordered list of children.
Shall be a first class business entity but may actually be implemented with Tags. 

## Un-categorized Application Features
Content Repository? integrate with other content repository applications and services like pocket.
Track Productivity
Focus
On Track

Group things that need to be done or acted upon during a particular trip. Creating a new tag doesn't fell right.

## Applications With Complimentary Features.
- 2Do
- OmniTask
- Simple Note
- EverNote

## Process 
- [Extreme Programming](http://www.extremeprogramming.org/)
- [TDD](http://c2.com/cgi/wiki?TestDrivenDevelopment)
- [BDD](http://behaviourdriven.org/)

## Useful libraries and specifications.
- [REST](https://en.wikipedia.org/wiki/Representational_state_transfer)
- [JSON](http://www.json.org/)
- [Node.js](https://nodejs.org/)
- [Express](http://expressjs.com/)
- [MongoDB](https://www.mongodb.org/)
- [Mongoose ODM](http://mongoosejs.com/)
- [q](http://documentup.com/kriskowal/q/)
- [lodash](https://lodash.com/)
- [JSON Web Tokens](https://jwt.io/)

## Useful Testing libraries
- [Should.js](https://shouldjs.github.io/)
- [supertest-as-promised](https://github.com/WhoopInc/supertest-as-promised)
- 

## Potentially useful libraries and specifications.
- [Open API Initiative (OAI)](https://openapis.org/)
