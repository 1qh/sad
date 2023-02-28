# Intro

- A sys
  - a collection of elements/components that are
    interrelated & work together towards a common goal
  - takes input & produces output
- Goal
  - Every information sys has a lifecycle
  - Main phases: Understanding of requirements/needs, ana,
    - des, Implementation, op & Maintenance
    - Can be linear (sequential)
    - Can repeat phases

### 5 Phases

1.  Understanding of requirements/needs
    - Clarifying what information sys is built to meet needs of users
    - immediate & future needs, explicit & implicit needs
1.  ana
    - Diving into nature & details of sys, showing what sys is supposed to do & data it uses
1.  des
    - Making sys des decisions to satisfy:
      - requirements identified in ana phase
      - actual constraints
1.  Implementation
    - Programming & testing
1.  op & Maintenance
    - Putting sys into use, making corrections & upgrades if unsuitable points are detected

### Method

Combination of 3 factors

- Concepts & M
- Implementation process: Step-by-step activities to do
- Support tools: sw to help (support) SAD

## OO Ming

### M & Ming

- M is an abstraction/an image/a representation of a described real sys:
  - From a certain point of view,
  - To some degree of abstraction,
  - By some form of understandable representation (text, D, graphs)
- Ming is use of M to perceive & describe a sys
- SAD process is also called sys Ming process
- Purpose of Ming:
  - understand
  - communicate (exchange)
  - complete
- A good Ming must satisfy:
  - Easy to
    - read
    - understand
    - communicate (exchange)
    - implement
  - Verifiable
  - Rigid
  - Complete

### Ming methods

- Notation: Concepts & M
- Process: Steps to do, products (documents, M) to be produced at each phase, how to run process, how to evaluate quality
- CASE (computer aided sw engineering) tool: Support sw for Ming process, capable of:
  - Producing M & D
  - Quickly transforming & adjusting M & D
  - Checking syntax, rigidness, completeness
  - Testing & evaluating
  - Simulation of M execution

# UML

- a language for
  - Visualization
  - Specification
  - Construction
  - Documentation
- Can be used in any sys dev process
- Throughout sys dev lifecycle
- Used by different implementation technologies

## Views

- Different M to describe a sys
- Each M can only describe sys from a certain point of view
- 5 different views of a sys
  - relate & complement each other
  - Each view is made by a number of D (M)
  - A D (M) may belong to several views
- Each role in sys dev process (analyst, deser, integrator, tester, end user) is usually interested only in a certain view of sys

### Usecase

- From outside looking at sys
- Influence (relate to) 4 remaining views
- As point of view of
  - end users
  - analysts
  - testers
- Not reflect internal organization, but only clarifies main/important funcs that sys must satisfy for users
- Static M
  - Usecase D
- Dynamic M
  - Communication D
  - State machine D
  - Activity D

### des

- Logical View
- View inside sys (structure), show tasks of sys
- View of sys deser
- Static M
  - C D
  - O D
- Dynamic M
  - Communication D
  - State machine D
  - Activity D

### Process

- Parallel View
- Reflects ctrl processes, execution processes, showing synchronous op of sys
- Used with D like in des View, focusing on active C
  - Active C: a C that represents for ctrl/execution processes

### Implementation

- Component View
- View on release form of sw
- Shows relatively independent components & files that can be assembled to make sys run
- Static M
  - Component D
- Dynamic M
  - Communication D
  - State machine D
  - Activity D

### Deployment

- A view of hardware architecture & infrastructure on which sys is deployed
- Specify distribution & arrangement of sys's components on hardware units & infrastructure platforms
- Static M
  - Deployment D
- Dynamic M
  - Communication D
  - State machine D
  - Activity D

## D in UML 2.0

- Structure D:
  - C D
  - O D
  - Deployment D
  - Package D
  - Component D
  - Composite structure D
- Behavior D:
  - Usecase D
  - Activity D
  - Sequence D
  - Communication D
  - State machine D
  - Timing D
  - Interaction overview D

## Elements of a D

- Nodes
  - Elements of M (D)
  - Represented by a 2D graphic form
  - Ex: C, Package
- Edges (links/paths)
  - Are elements of M (D)
  - Represented by a linear graphic form
  - Ex: asso, Dependency, Generalization

### Add meaning to a D

- Specification
  - A textual statement of syntax & semantics
- Adornment
  - Role, Multiplicity, Qualifier
- Stereotype
  - String of characters, enclosed in quotes (<<…>>)
- Property & Tagged value
  - Give more information to an element of D
  - Example: {label=value}, {label_boolean}
- Constraint
  - Add conditions/constraints to an element of D

## Ming with UML

- Ming sys from multiple views
  - Can use 5 views to sys
  - Depending on sys is small/large, simple/complex
  - Decide to describe (to M) sys by suitable views
- Ming sys by different abstraction levels
  - Depends on phases (of sys dev process) & user needs
  - Can be at logical/overview level or detailed level

# SDP

- A structured (ordered) set of activities required to develop a sw sys
  - Example: Waterfall, Prototyping, Spiral
  - Not exist a single ideal SDP process suitable for all practical problems & requirements

### Select suitable SDP

- Type of sw sys to be built
  - Build sys from scratch >< Upgrade, update from an existing sys
  - Common (popular) >< Customized or unique
  - Defined sw requirements >< sw requirements change (quickly)
  - Critical sys >< Business sys
- Size of
  - sw dev pj
  - dev team
- pj implementation time
- Characteristics of sw dev team
  - Experience
  - Motivation (encouragement)
  - Work attitude (effort)
- Budget of sw dev pj

### Main activities

- Feasibility study
- Requirements ana & specification
- des
- Implementation
- Testing
- Deployment
- Maintenance

## Waterfall

- Phases
  - Feasibility ana
  - Requirements ana & specification
  - des
  - Implementation (Programming) & Testing
  - Deployment & Maintenance
- M
  - Most used
  - Based on a set of sequentially ordered phases
  - Once SDP ends & sw sys is handed over (signed off) to customer, sw sys cannot be changed or adjusted
    - order of phases is deterministic & results of a previous phase will be used as input for following ones
  - SDP can only be reopened (in response to adjustments/changes) through a formal change process
  - Non-overlapping, non-repeating phases
- Advan & disadvan
  - Advantages
    - Simple, easy to understand & use
    - documents are completed after each phase
    - sw requirements are provided early to testers
    - Allows PM to easily plan & ctrl execution
    - Well known by non-professional, easy to use for communication
  - Disadvantages
    - Only suitable for real problems when sw requirements are clearly defined, complete & fixed from beginning (before des phase)
    - Not suitable for long-running pjs
    - Those pjs that may have risk or uncertainty factors
    - Hard to have initial results (versions) soon
- When to use
  - sw requirements are clearly defined, complete & fixed
  - definition of product (sw sys) does not change
  - related & necessary technologies are mastered
  - resources & experience of sw dev team are sufficient
  - time of pj execution is short

## Prototyping M

- Phases
  - Requirements
  - ana
  - Quick des
  - Prototype building
  - Prototype evaluation
  - des
- M
  - Instead of fixing requirements before proceeding with des or implementation, a prototype is built to understand exact sw requirements
  - Each prototype is built upon current sw requirements (obtained
  - from evaluation of previous prototypes)
  - By using prototypes, customers can get real feel
    - because interactions with prototype allow customers to have a better, more precise understanding of requirements
  - Using prototypes is reasonable for dev of large & complex sw sys
    - when there is no requirement gathering process or inbuilt sys to help define sw requirements
  - A prototype is usually not a complete sw sys & many details are not implemented
- Advan & disadvan
  - Advantages
    - Users are actively involved in SDP
    - Using a prototype as a working M of sys, users gain a better understanding of sys being built
    - Errors, problems can be detected early
    - Early to get evaluation feedback from users for better solutions
    - Missing funcs can be discovered early
    - funcs unclear or difficult to operate may be detected
  - Disadvantages
    - Users may think sw dev is easy & become inconsistent in expression of requirements
    - Planning is not done at beginning of pj, which may lead to pj management problems: undefined
      - deadlines
      - budgets
      - deliverables
    - Leads to prolong SDP
    - Developers tend to deliver a basic working prototype, rather than a real complete product
- When to use
  - sw requirements cannot be determined at time of pj initiation
  - users (for various reasons) cannot express requirements clearly
  - developing "look & feel" or UI
    - because these features are difficult to describe by documentation, but obtained through trial use
  - customers ask for proof of feasibility
  - demos needed for senior management board
  - technology problems need to be tried & tested

## Spiral

- M
  - based on a hybrid combination of iterative of Prototyping & sequential of Waterfall
    - Focus on risk ana
  - Dev through a series of incremental releases
    - In initial iterative steps of dev, versions can be simply sketched M on paper or prototypes
    - In later iterative dev steps, increasingly mature versions are created
- Advan & disadvan
  - Advantages
    - Focus on risk ana, reduce risks in pjs
    - Suitable for large & particularly important pjs
    - New funcs may be added later
    - Initial versions of sw sys are created early
  - Disadvantages
    - High cost (time, resources, money) to apply
    - Risk ana requires high skills & experience
    - success of pj depends strongly on risk ana phase
    - Not suitable for small pjs
- When to use
  - When assessment (ana) of costs & risks is important
  - For medium-high-risk pjs
  - Users are uncertain about their needs
  - Complex & large sw requirements
  - Need to develop a new product line
  - Desire for significant changes (careful research & investigation is required)

## Agile

- M
  - incremental & iterative
  - Dev through incremental & rapid cycles
  - Helps create small-scale enhanced versions
    - where a next version is built on features of previous one
  - Each enhanced version is carefully tested to ensure sw quality
  - Used for sw dev pjs that require quick completion times
    - Extreme Programming (XP) is 1 of famous methods belonging to agile M
- Advan & disadvan
  - Advantages
    - Satisfy customers with agile enhanced sw versions
    - Emphasis on interactions between actors rather than processes & tools (customers, developers & testers constantly interact with each other)
    - Frequent communication between business ana & programming team
    - Adapt (response) quickly to changing requests
    - Even allowing changes of sw requirements are added later
  - Disadvantages
    - For large sw sys, this agile M makes it difficult to estimate necessary costs & effort at beginning of SDP
    - Less emphasis on required des & documentation
    - Usually only senior developers can make necessary decisions during dev
      - not suitable for inexperienced developers, unless working in conjunction with experienced ones
- When to use
  - New changes can be implemented at low cost, by frequent creation of enhanced versions
  - To implement a new feature, developers only need a few days, or even a few hours to implement
  - Unlike waterfall, in agile, planning is (much) less cost
  - assumes that user needs will (often) change
  - Changes can always be requested & features can always be added or removed based on customer feedback
  - Both developers & users of sys find they have more freedom of time & choices than M that strictly follow a sequence of steps (waterfall)

## RUP

- Rational Unified Process is a Ming process using UML

### Basic principles

- Iteration & incremental
  - pj is divided into short loops or stages for easy ctrl
  - At end of each loop, executable part is produced in a gradually added
- Focus on architecture
  - complex sys is divided into modules for easy deployment & maintenance
  - architecture is presented in 5 different views
- Led by UCs
  - UCs influence every phase of sys dev, basis for
    - defining loops & enhancement
    - dividing work within team
  - Needs understanding: Detect UCs
  - ana: Dive into description (specification) of UCs
  - des & implementation: Build sys according to UCs
  - sys testing & acceptance: Follow UCs
- ctrl risks
  - Early detect & eliminate risks to pj

### Main phases

- Inception
  - Give an overview of sw sys (funcs, performance, technology) & sw dev pj (scope, goals, feasibility)
  - Conclusion of whether to develop or give up pj?
- Elaboration
  - More detailed ana of sys (funcs & static structures)
  - Propose a sys architecture prototype
- Construction
  - Focus on sys des & implementation
  - sys architecture is detailed & edited
  - Finishes when a complete sys with accompanying technical documentation is created
  - Take most time & effort
- Transition
  - Transfer sys to end users: data conversion, installation, testing, training

### Main steps

1. Preliminary study
   - like Inception
1. Identify & describe UCs
   - Understand user needs & identify UCs
   - Each UC must be specified (described) in form of a scenario and/or a sequence D
1. app domain Ming
   - Provide CD that reflect all concepts & businesses
   - C here are domain C (not des C)
1. Define C / O involving in UCs
   - For each UC, define entity, ctrl, boundary C
1. Ming interactions in UCs
   - O interact by exchanging messages
   - Create UC scenarios: Sequence, Communication D
1. Behavior Ming
   - ctrl O have ability to react to events coming from outside
   - Use state machine D to describe behavior of ctrl O
1. Create UI prototype
   - Use GUI des tools to create (des) interfaces prototype early, making sys's Ming & implementation easier
1. des sys architecture
   - des sys's overall architecture
   - Divide into sub-sys
   - Use component D to describe physical components
   - Use deployment D to describe arrangement & deployment of sys's executable components to hardware & infrastructure platform
1. Detailed des
   - For C, assos, properties, methods
   - Determine sys's implementation solution
1. Implementation
   - Programming & testing
   - sys is approved (accepted) on UCs

# ana of environment & needs

## Goal

- This is preliminary study step
- Investigate & study about environment & business context of sys to be built
- Identify func & non-func requirements, risks & constraints
- pj definition & planning
- Should we develop or give up pj?

## Method

- Studying written materials
  - Complete documents
    - Transaction documents
    - Archive documents (papers, files)
    - Reporting documents (plan, statistics)
  - Fill-in documents
    - Inquiry documents (questionnaire, collection form)
- Interviewing
  - Interview with written materials to explain/add/check/update written information
  - Interview without written materials: seminar, individual/group interview
  - Survey form with open/closed questions
- Observing
  - Work execution process, Business document processing flow
  - Count number of transactions, count processing time

## Sys overview document

- Aggregate studied & collected information into an overview report of sys
- Each sys is always placed in a business environment
  - At this stage, it is not possible to clearly determine boundary between sys to be built & environment
- Describe op of users, equipment & computers in a business environment
- include
  - Business goal
  - Main tasks/main funcs
  - Business processes
    - Should be described (presented) by activity D
  - Types of information used in sys
  - Requirements for sys to be built about
    - funcs
    - quality, performance
    - priorities, restrictions, constraints

## Pj planning

- Define
  - scope & limitations
  - goals & priorities
- Propose a solution (at a general/preliminary level) & demonstrate its feasibility
- Anticipate & assess risks
  - misunderstanding needs
  - outdated technology
  - limited human resources & experience
  - limited time to complete
- Create implementation plan
  - human resource
  - finance
  - timetable
  - considering risks

# Func ana

## Goal

- Give a preliminary look at sys's func
  - Business processes
  - func requirements
- func ana is only intended to show major funcs (sys's requirements)
  - Without going further into minor funcs
  - Because currently & commonly used method of ana & des is OO (not func-oriented)

## Ming business processes by activity D

- Goal of Ming business processes
  - pj will be started with a Preliminary Research to understand Business Environment of sys to be built
  - In that environment, users, equipment & computers work together according to certain Business Processes
  - Activity D describes activities following flow from 1 activity to another
    - A business process
    - Execution logic of a
      - UC or a group of UCs
      - usage scenario
      - complex op
  - UML M equivalent to block D or data flow D in func-oriented ana & des method
- Activities & Transitions
  - directed graph, consisting of: Nodes are activities, Edges are transitions, Start node (bold black dot) & End node(s) (bold black dot with border)
  - Activity is a job, can be handled by hand – example: form filling, or processed by computer – example: display information on screen
  - Transition is transition from 1 activity to another
- Branching
  - A guard <> is a condition check, attached to a transition, to indicate that transition is performed only when this condition is satisfied
  - 2 kinds of guards:
  - A decision node
    - A single incoming flow & multiple outgoing flows
      - these outgoing flows must be mutually-exclusive
  - A merge node - Multiple incoming flows & a single outgoing flow - this merge point is passed when an incoming flow occurs - Merge node should not be used to synchronize concurrent flows!
- Synchronization (of concurrent flows)
  - Synchronization bars are used to open or close parallel execution branches:
    - Opening parallel execution branches by a synchronization bar to show a single incoming transition & multiple outgoing ones
      - called a fork
    - Closing parallel execution branches by a synchronization bar to show multiple incoming transitions & a single outgoing one
      - called a join
    - A join can be passed only when all incoming execution branches complete
- Line-separating & partitioning
  - Like swim-lanes in a swimming pool
  - Each activity must be placed in a line & each line shows execution of 1 or more O
    - Transitions may change lines freely
  - An activity may be partitioned, each partition contains activities that have some characteristic in common - For example, a partition for major usage scenario & several other partitions for minor ones.
- O creation & O flow
  - Specify that some activity
    - creates an O
    - modifies O's state
    - takes as input an O for processing
  - draw additional O (with their states, if necessary)
  - connect those O to related activities with dashed arrows (called O flows)
  - An O flow from 1 activity to an O & then continue to another activity can be seen as a ctrl flow (a transition) between 2 activities.

## Ming func requirements by UC D

- Goal of Ming func requirements
  - Define major sys funcs expected by users (called func requirements)
  - Describe ana results with UML UC D
- order of work
  - Ming work environment of sys by actors
  - Ming requirements by UCs
  - Determining relations (actors, UCs)
  - Creating UC D

### Ming work environment of sys by actors

- Actors is role of 1 or more users or external (outside sys to be built) O that interact with sys
- Types of actors:
  - Users vs. external sys/O
  - Primary vs. secondary (a.k.a. supporting)

### Ming requirements by UCs

- A UC is a representation of a set of sys actions that provide a result to an actor
- Characteristics
  - be associated with 1 or more actors
  - lead to a specific result
  - be a set of actions
- Specification
  - In natural language
    - Name of UC
    - Description of usage purpose
    - (Primary, secondary) actors
    - Trigger (event)
    - Pre-conditions
    - Post-condition
    - Main (a.k.a. normal) flow
    - Alternative flows
  - Supplemented by an activity D or a sequence D

### Determining relations

- Generalization between actors
  - Actor A is a generalization of actor B, if B inherits all characteristics of A
- Communication between an actor & a UC
  - If actor & UC communicate with each other
  - If communication is one-way, use arrow
- Generalization between UCs
  - UC X is a generalization of UC Y, if Y inherits all characteristics of X (can modify & add)
- Inclusion between UCs
  - If UC X always include content of UC Y into content of X at a position (inclusion point) specified in specification of X
  - X (UC at beginning of arrow) is called base UC
- Extension between UCs
  - If UC X conditionally include content of UC Y into content of X at a position (extension point) specified in specification of X
  - X (UC at end of arrow) is called base UC

# Structure ana

- Goal
  - Preliminary determine main C that make up sys
    - not complete (final) version of C

## O & C

### Definition

- O
  - An abstract representation of a (physical or conceptual) entity that has a clear identity & boundary in real world
    - including state & behavior of that entity
    - aiming at simulating or ctrlling that entity
  - state of an O is represented by a set of atts
    - At a time, each att of O has a certain value
  - behavior of an O is represented by a set of ops
    - which are services it can perform when requested by another O
  - identifier of an O is what distinguishes it from another
- C
  - description of a set of O that share same atts, ops, relations, constraints & semantics
  - a C is a type
    - each O of C is an instance

### atts

- A named property of a C that takes a value for each O of that C at a time
- `[Visibility] [/] Name [: Type] [Multiplicity] [= Initial value] [{Property-string}]`
  - Visibility
    - How att is seen & used by other C
      - Private - not accessible from any other C
      - Protected # only accessible from C that inherit current C
      - Package ~ accessible from C belonging to same (most inner) package of current C
      - Public + accessible from any other C
  - Type
    - Basic types like Integer, Real, Boolean
    - Structured types like Point, Area, Enumeration
    - Type is another C
  - Multiplicity
    - number of possible values assigned to att
      - Ex: [0..1] shows that att is optional (may take no or 1 value)
  - Initial value
    - default value assigned to att when an O is instantiated from that C
  - Property-string
    - defines values that can be assigned to att, usually used for enumeration-typed atts
      - Ex: status: Status = unpaid {unpaid, paid}
- An att may have C scope if it reflects general characteristics of C
  - C-scoped atts must be underlined
  - Example: att `number-of-invoices` of C `Invoice`
- An att is derived, if its value is calculated from values of other atts of C
  - Derived atts must include a slash '/' at beginning
  - Example: /age (while att /birthday exists)

### ops

- An op is a service that an O can respond to when requested (via a message)
- ops are implemented as methods
- `[Visibility] Name [(Parameter list)] [:Return type] [{Property-string}]`
  - Visibility is defined same as for atts
  - Parameter list is a list of parameters, separated by commas, each of form:
  - `[Direction] Name : Type [= Default value]`
    - Direction
      - either of in, out, inout or return depending on parameter is
        - may not be modified (in)
        - may be modified to communicate information to caller (out)
        - may be modified (inout)
        - or to return result to caller (return)
    - Default value
      - value to be used when corresponding parameter is missing in call
  - Property-string
    - includes pre-conditions, postconditions, effects on O state

## Relations

### Dependency

- Used to express a (dependent) C that is affected by any changes in another (independent) one
  - opposite direction is not necessarily
- dependent C needs to use independent 1 to specify or implement it
- UML represents dependency relation with a dashed arrow from dependent C to independent one

### Generalization

- extraction of common characteristics of many C to form a simpler (more generalize) C
  - Called a super-C
- On contrary, specialization is enhancement (addition) that adds some new characteristics from a given C, forming a more specific C
  - Called a sub-C
- a C can have no, 1 or more super-C(es)
  - a C with
    - only 1 super-C is called simple inheritance
    - multiple super-C is called multiple inheritance
- a C that has no super-C & has sub-C is called a root C (base C)
- inheritance is used in programming to describe a sub-C that has all atts, ops & relations described in its super-C
  - Sub-C can add new (own) atts, ops & relations
  - A sub-C can re-define (overwrite) an op of supper-C: Polymorphism
- Abstract C
  - have no instance O
  - but only used to describe common characteristics of sub-C
  - contains abstract ops
    - with only title (name)
    - without implementation
    - redefined (overwritten) & implemented in sub-C
  - name of abstract C & title of abstract op
    - must be italicized
    - may include property string {abstract}
  - Ex
    - Animal is an abstract C generalized from C Horse, Tiger, Bat
    - Abstract op sleep()
      - specifically implemented in sub-C Horse, Tiger, Bat in different ways
      - but keeping same name sleep()

### asso

- Link represents some actual relation between instances (O) of 2 C
  - Ex: wife-husband link, teacher-student link, motorbike-owner link, customer-invoice link
- asso is a relation between 2 C, consisting of a set of links of same type (of same meaning) between instances of those 2 C
  - a relation (in mathematical sense) between 2 sets (2 C)
- Navigation
  - A link between 2 O (of 2 C in an asso)
    - mean O "know each other"
    - By link, from 1 O we can find other
  - may be bi-directional (from both ends) on an asso
  - may be restricted in 1 direction
    - add an arrow to navigated end & a slash to unnavigated end
- Role
  - In an asso between 2 C, each C plays a different role
  - role name (with first letter in lowercase) can be appended to each end of link
    - thus role is also called name of an asso end
  - a role represents a subset of O of corresponding C
- Multiplicity
  - Each end of asso may also contain a multiplicity to indicate (minimum & maximum) number of instances of that end participating in asso with 1 instance at other end
    - 1
      - 1 & only one
    - 0..1
      - 0 or 1
    - m..n
      - From m to n (natural numbers)
    - 0..\* or \*
      - From 0 to many
    - 1..\*
      - From 1 to many
- Qualifier
  - Search problem
    - Given an O at 1 end of asso
    - find an O or set of O connected to it at other end
  - To reduce number of O found
    - limit search area to (values of) certain atts (called qualifiers)
  - Shown in a small box attached to end (C) of asso, where navigation originates
  - Applied to 1-to-many or many-to-many assos, to reduce from many to 1 (or 0..1), or to reduce from many to many (but number is less)
- asso C
  - An asso itself may also need to have specific atts
    - UML supports this by asso C
  - a C as usual (with atts, ops & assos)
    - but name-box can be optionally named or left blank
    - attached to asso by a dashed line
- N-ary asso
  - There can be an asso between more than 2 C, in sense of a plural (a tuple-n) relation
  - Represented by a small rhombus (diamond) symbol, connected by solid lines to participating C & may also have an asso C attached
- Aggregation
  - M a "whole-part" relation between a C of "whole" & "part" O.
  - Represented by attaching an empty rhombus (diamond) symbol to end at "whole" side
  - Example
    - Student ("part" C) has an aggregation asso with University ("whole" C)
    - an O of Student has "study-at" relation with multiple O of University
- Composition
  - Type of an aggregation with stronger ownership relation
    - "part" belongs only to a single "whole"
    - "whole" is responsible for creating & destroying "part"
  - When "whole" is destroyed, "part" is also (automatically) destroyed
  - Composition is represented by attaching a solid rhombus (diamond) to end at "whole" side of asso

## CD & OD

- a CD is a D that shows a set of C & relations (asso, aggregation, composition, generalization, dependency) between them
- CD are used to M static structures of sys, including all declared elements
- An OD represents static structure of a CD in a specific way
  - O instead of C, Links instead of assos

## Determining domain C

### Goal & execution process

- Starting from concepts of things in app domain
  - abstract them into C called domain C
- used to reflect and simulate real-world things
  - store & provide information
- Execution process
  - Identifying domain concepts
  - Determining assos & atts
  - Generalizing concepts

### Identifying domain concepts

- Search sources
  - Domain concepts are concepts about things (concrete or abstract)
    - used by users & business experts
    - when they discuss about that domain
- To search for domain concepts
  - Knowledge of business domain
  - Interviews with users & business experts
  - document that describes
    - an overview of sys & needs
    - UCs (created in previous step of SDP)
- How to identify concepts
  - Read sys description document (describing requirements):
    - Nouns can be O or atts
    - Verbs can be ops
  - Based on that, identify following O:
    - Entity (motorbike, airplane, sensor)
    - Role (teaching, monitoring)
    - Event (landing, interrupting, motorbike registration)
    - Interaction (lending, discussion)
    - Organization (company, faculty, C)
- Name & assign responsibility
  - Responsibility
    - role & use purpose of C
    - not structure of that C
      - Although latter responsibility will allow us to define structure (properties & assos) & behavior (ops) of C
  - Help to check if C selection is reasonable
    - If you can choose a name
      - & assign clear & concrete responsibility
        - C selection is good
      - but responsibility
        - same as (or similar to) responsibility of another C
          - combine those 2 C into one
        - too long (complex)
          - split that C into several ones
    - Difficult to choose a reasonable name or describe responsibility
      - analyze more deeply to choose appropriate representations

### Determining assos & atts

- atts & assos of domain C can be directly determined from
  - document describing sys & needs
  - statements of domain experts & users
  - responsibilities of C defined in previous step
- From description of responsibility of C Student
  - Information needed to register & calculate tuition fees for a student
    - infer atts
      - name
      - student code
      - address
  - Student is a person who is allowed to register to credit courses of a university
    - infer asso
      - between Student & CreditCourse with the
      - asso name maybe "register"

### Generalizing C

- To optimize C representation M
  - extract common parts between C to form a more general C
- Student & Lecturer have common atts (name, id code)
  - define a more generalized C Person

## Determining C involving in UCs

### Goal

- Domain C are same for every sw app of domain
- specifics of a sw app are in its UCs
- to study current sw app
  - analyze structure & behavior of these UCs in depth
- A UC is viewed as a collab of several O, including
  - domain C
  - app-specific C
- purpose of this step
  - analyze static structure of UCs
- tasks
  1. Determine C involving in UCs
  1. Add relations between C to create a CD for each UC

### Procedure

- UCs are studied (analyzed) to determine C that participate in each of these UCs
- C that participate in UC are called ana C, including 3 types:
  - Boundary C (dialog C)
    - communicate (exchange) information between actors & sys, represent
      - screens for communicating with users, allow
        - information to be collected
        - results to be displayed
      - interfaces between sys & devices that it ctrls or collects information
    - For each pair of (actor, UC), there must be at least 1 boundary C
      - main boundary C may need auxiliary boundary C
        - to delegate some of its overwhelming responsibilities
    - boundary O have same lifecycle as with its associated UCs
  - ctrl C
    - Manage & ctrl progress in a UC
      - Engine that makes UC progress
    - Contain business rules & are intermediate between boundary C & entity C
      - allow from screen (UI) to manipulate information contained in entity C
    - For each UC, create at least 1 ctrl C
    - When moved to des phase
      - not necessarily going to exist as a real C
        - since its task can be dispersed into other C
    - but during ana phase
      - necessary to have
        - ensure that funcs or behaviors in UCs are not left out
  - Entity C
    - Business C
      - determined directly from description of domain
      - will be confirmed if they appear in UCs
    - persistent C
      - data & relations are retained (databases or files) after UCs finish
    - It is confirmed that an entity participate in a UC
      - if information contained in that entity C is mentioned in UC

### Creating a CD for each UC

- reflect the static structure of collab (between C)
- Include all determined C & necessary structural elements (atts, ops, assos) of each C
  - atts must store enough information about O needed in collab
  - ops provide required service capabilities of each C engaging in collab
  - assos create links between C
    - allow to know & communicate with each other in collab
- Adding atts & ops
  - entity C temporarily have only atts
    - atts describe persistent information of sys
  - ctrl C temporarily have only ops
    - ops represent business processing logics, business rules & behaviors of sys
  - boundary C have both atts & ops
    - atts describe fields to
      - collect information
      - output results
    - results are distinguished by notation of derived atts
    - ops represent actions user performs on interface screen
- Adding assos
  - Boundary C are only associated with ctrl C or with other boundary C
    - an asso is one-way from a boundary C to a ctrl C
      - unless ctrl C again creates a new dialogue (a page displaying results)
  - Entity C are only associated with ctrl C or with other entity C
    - An asso of an entity C with a ctrl C is always one-way
      - from ctrl C to the entity C
  - ctrl C may be associated with all types of C
    - including also with other ctrl C
- Adding actors
  - An actor is connected to only 1 (or several) boundary C
    - not associated with any ctrl or entity C
