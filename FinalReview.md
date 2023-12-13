# Final Review
Software Engineering  
CPSC 480-020  
Javan Miller  

### Testing
- Black Box Testing
    - Focuses on Input and Output
    - Represents the views of the users
    - Tests the following
        - Functionality
        - User input validation
        - Output results
        - State transitions
        - Boundary cases and off-by-one errors
- Grey Box Testing
    - Is like black box testing, but you can can peek
    - Allows you to dig around a little to ensure the system works as it's supposed to below
    the surface
    - Tests the following
        - Verifying auditing and logging
        - Data designed for other systems
        - System-added information
        - Scraps left laying around
- White Box Testing
    - Is the deepest level of testing
    - Allows one to see exactly what's going on inside the code
    - Is typically completed code-on-code, rather than exercised by a human
    - Tests the following
        - Testing all the different branches of code
        - Proper error handling
        - Working as documented
        - Proper handling of resource constraints

### Use Case and Use Case Diagram
**Need to be able to draw a diagram**
- Use Cases
    - Describes what a system does but now how it does it
    - Achieves a discrete goal for the user
    - May map to several use cases
    - Represent the functional requirements of the system 
        - *Note: Non-functional requirements are stated elsewhere*
- UML Use Case Diagrams
    - Describes a set of sequences
    - Represents actors with the system itself

### Process Models
- Waterfall Model
    - Heavyweight, single-pass, heavy planning-based approach
    - Each phase is completed and verified before the next phase begins
    - Very similar to the "Big Bang" approach
        - Completing all of the work at once as opposed to an iterative approach
        - Developers typically spend more time on planning in the Big Bang appoach
    - Requires extreme amounts of planning to be successful
    - Was designed to solve the software crisis
    - Prescriptive rather than descriptive
    - Requirements not always known in advance and are often added in other phases
    - Band-Aid Approach - Design for Change
        - Since requirements are volatile, design to allow for future changes
        - Increases flexibility, which could in turn increase complexitiy
        - Increases cost of the intiial software
        #### Phases
        Requirements -> Design -> Implementation -> Verification -> Maintenance    
- Agile
    - Lightweight, doing (vs. planning), multiple passes, evolutionary approach
    - Far more successful than the Waterfall approach
    - Strongly iterative and evolutionary
    - Are several different Agile Process Models:
        - eXtreme Programming
            - Pure agile approach
            - Given as a set of best practices
            - Pushes good practices to their **extreme**
            - Design is kept as simple as possible
            - Strongly involves refactoring, TDD, etc.
        - Rational Unified Process (RUP)
            - Developed by Rational Software (IBM)
            - Has a lot of tool support - Rational Method Composer (RMC)
            - Is between document-driven and agile approaches
            - Has the following phases:
                - Inception - determine objectives, costs, schedule, and risks
                - Elaboration - analysis to determine architecture
                - Construction - implementation
                - Transition - release, integration into existing systems
        - Scrum *(more detail below)*
        - And so many more...

### Software Evolution
- Greenfield Development
    - Start with nothing and create a finished product with no existing code, design, or
    previous system
    - Most SE education stresses greenfield development
    - Very little greenfield development exists in the real world
    - What CS students invision themselves doing
- Brownfield Development
    - Start with an existing project/environment and create a finished product with existing
    code, design, or previous system
    - Most SE education treats brownfield development as a side topic
    - What most CS students end up doing
- Maintenance
    - Corrective Maintenance
        - Fix bugs/problems
    - Adaptive Maintenance
        - Change to fit new environment (API, compiler)
    - Perfective Maintenance
        - Improve performance or maintainability
    - Preventative Maintenance
        - Detect and correct latent problems before they become actual problems
    - Maintenance is roughly 80% of the cost of the system over its lifetime
- Lehman's Laws of Software Evolution
    - Software must change over time
    - Changes cause complexity; complexity increases the cost of change
    - Software projects in an organization tend towards the same quality, bug rate, etc.
    - Over time, the rate of development for each iteration doesn't very much
    - Must implement features that were previously not considered necessary
    - Without changes, the software appears to decrease in quality
    - What affects software evolutiojn is a multi-level, multi-iteration process

### Refactoring
- Refactoring - the process of changing a software system in such a way that it does not
alter the external behavior of the code yet improves its internal structure
- Testing must be in place before making any refactoring changes
- The current, expected behavior of the software must not change during refactoring
- Legacy Code - any code that does not have a unit-testing suite
- Why Refactor?
    - Design Preservation
        - Refactoring improves the design of existing code
    - Comprehension
        - Refactoring makes code more readable
    - Debugging
        - Greater program comprehension leads to easier debugging
    - Faster Programming
        - Good design is essential for rapid development
        - Poor design allows for quick process but soon slows process down
            - Spend time debugging
            - Changes take longer as you understand the system and find duplicate code
        - Supported by Lehman's Laws
#### Refactoring Techniques
- Introduce Explaining Variable
- Rename Method
- Move Method
- Pull-Up Method
- Change Value to Reference
- Remove Parameter
- Extract Hierarchy

### Scrum
- Scrum - Iterative agile software development framework
- Time measurements
    - Sprint
        - Fixed duration of 1 week to 1 month
    - Timebox
        - Fixed amount of time allocated, and when done, the activity is finished
- Backlog
    - Product backlog 
        - List of requirements ordered by business values and needs
        - Typicall in user story format
    - Sprint backlog 
        - List of work the development team attempts in the next sprint
- Sprint Planning Meeting
    - Occurs at the start of the sprint
    - Select what work the team does
    - Put together the sprint backlog
    - The entire team works on prioritizing the product backlog (4 hours)
    - The development team creates a plan for the sprint (4 hours)
- Story Time
    - Estimation for backlog using planning poker or other methods
    - Should not take longer than an hour
    - Does not include breaking stories into tasks
    - The team decides the number of meetings per week
- Daily Scrum Meeting
    - Everyone on the development team has an update
    - Limited to 15 minutes at the same location and time everyday
    - Discuss the following
        - What have you done since yesterday?
        - What are you planning to do today?
        - What obstacles are in your way?
- Burn Down Chart
    - The status of the work on the sprint backlog
- Increment
    - All the product backlog completed during a sprint
- Sprint Review Meeting
    - Review user storeis completed and uncompleted during the sprint
    - Demo the completed user stories
    - 4-hour time limit
- Sprint Retrospective
    - What went well?
    - What could be improved?
    - Entire team reflects on past sprint
    - Time for making continuous process improvements
    - 3-hour time limit

### SE Code of Ethics
#### Principles
1. Public
1. Client and Employer
1. Product
1. Judgement
1. Management
1. Profession
1. Colleagues
1. Self

#### Definitions
1. Public - Software engineers should act consistently with the public interest
1. Client and Employer - Software engineers should act in a manner that is in the best interest
of their client and employer consistent with the public interest
1. Product - Software engineers should ensure that their products and related modifications meet
the highest professional standards possible
1. Judgment - Software engineers shall maintain integrity and independence in their professional
judgment
1. Management - Software engineering managers and leaders shall subscribe to and promote an
ethical approach to the management of software development and maintenance
1. Profession - Software engineers shall advance the integrity and reputation of the profession
consistent with the public interest
1. Colleagues - Software engineers shall be fair to and supportive of their colleagues
1. Self - Software engineers shall participate in lifelong learning regarding the practice of
their profession and shall promote an ethical approach to the practice of the profession