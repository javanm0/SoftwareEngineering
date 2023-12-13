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