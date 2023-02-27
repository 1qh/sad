# Intro

- A sys

  - a collection of elements/components that are
    interrelated & work together towards a common goal

  - takes input & produces output

- Goal

  - Every information sys has a lifecycle
  - Main phases: Understanding of requirements/needs, Analysis,
    - Design, Implementation, Operation & Maintenance
    - Can be linear (sequential)
    - Can repeat phases

### 5 Phases

1.  Understanding of requirements/needs

    - Clarifying what information sys is built to meet needs of users
    - immediate & future needs, explicit & implicit needs

1.  Analysis

    - Diving into nature & details of sys, showing what sys is supposed to do & data it uses

1.  Design

    - Making sys design decisions to satisfy:
      - requirements identified in analysis phase
      - actual constraints

1.  Implementation

    - Programming & testing

1.  Operation & Maintenance

    - Putting sys into use, making corrections & upgrades if unsuitable points are detected

### Method

Combination of 3 factors

- Concepts & models
- Implementation process: Step-by-step activities to do
- Support tools: sw to help (support) SAD

## OO modeling

### Model & modeling

- Model is an abstraction/an image/a representation of a described real sys:

  - From a certain point of view,
  - To some degree of abstraction,
  - By some form of understandable representation (text, diagrams, graphs)

- Modeling is use of models to perceive & describe a sys

- SAD process is also called sys modeling process

- Purpose of modeling:

  - understand
  - communicate (exchange)
  - complete

- A good modeling must satisfy:

  - Easy to
    - read
    - understand
    - communicate (exchange)
    - implement
  - Verifiable
  - Rigid
  - Complete

### Modeling methods

- Notation: Concepts & models

- Process: Steps to do, products (documents, models) to be produced at each phase, how to run process, how to evaluate quality

- CASE (computer aided sw engineering) tool: Support sw for modeling process, capable of:

  - Producing models & diagrams
  - Quickly transforming & adjusting models & diagrams
  - Checking syntax, rigidness, completeness
  - Testing & evaluating
  - Simulation of model execution

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

- Different models to describe a sys
- Each model can only describe sys from a certain point of view
- 5 different views of a sys
  - relate & complement each other
  - Each view is made by a number of diagrams (models)
  - A diagram (model) may belong to several views
- Each role in sys dev process (analyst, designer, integrator, tester, end user) is usually interested only in a certain view of sys

### Usecase

- From outside looking at sys
- Influence (relate to) 4 remaining views
- As point of view of
  - end users
  - analysts
  - testers
- Not reflect internal organization, but only clarifies main/important functions that sys must satisfy for users
- Static models
  - Usecase diagram
- Dynamic models
  - Communication diagram
  - State machine diagram
  - Activity diagram

### Design

- Logical View
- View inside sys (structure), show tasks of sys
- View of sys designer
- Static models
  - Class diagram
  - Object diagram
- Dynamic models
  - Communication diagram
  - State machine diagram
  - Activity diagram

### Process

- Parallel View
- Reflects control processes, execution processes, showing synchronous operation of sys
- Used with diagrams like in Design View, focusing on active classes
  - Active class: A class that represents for
    control/execution processes

### Implementation

- Component View
- View on release form of sw
- Shows relatively independent components & files that can be assembled to make sys run
- Static models
  - Component diagram
- Dynamic models
  - Communication diagram
  - State machine diagram
  - Activity diagram

### Deployment

- A view of hardware architecture & infrastructure on which sys is deployed
- Specify distribution & arrangement of sys’s components on hardware units & infrastructure platforms
- Static models
  - Deployment diagram
- Dynamic models
  - Communication diagram
  - State machine diagram
  - Activity diagram

## Diagrams in UML 2.0

- Structure diagrams:
  - Class diagram
  - Object diagram
  - Deployment diagram
  - Package diagram
  - Component diagram
  - Composite structure diagram
- Behavior diagrams:
  - Usecase diagram
  - Activity diagram
  - Sequence diagram
  - Communication diagram
  - State machine diagram
  - Timing diagram
  - Interaction overview diagram

## Elements of a diagram

- Nodes
  - Elements of model (diagram)
  - Represented by a 2D graphic form
  - Ex: Class, Package
- Edges (links/paths)
  - Are elements of model (diagram)
  - Represented by a linear graphic form
  - Ex: Association, Dependency, Generalization

### Add meaning to a diagram

- Specification
  - A textual statement of syntax & semantics
- Adornment
  - Role, Multiplicity, Qualifier, etc.
- Stereotype
  - String of characters, enclosed in quotes (i.e., <<…>>)
- Property & Tagged value
  - Give more information to an element of diagram
  - Example: {label=value}, {label_boolean}
- Constraint
  - Add conditions/constraints to an element of diagram

## Modeling with UML

- Modeling sys from multiple views
  - Can use 5 views to sys
  - Depending on sys is small/large, simple/complex
  - Decide to describe (to model) sys by suitable views
- Modeling sys by different abstraction levels
  - Depends on phases (of sys dev process) & user needs
  - Can be at logical/overview level or detailed level

# SDP

- A structured (ordered) set of activities required to develop a sw sys
  - Example: Waterfall, Prototyping, Spiral, etc.
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
- Requirements analysis & specification
- Design
- Implementation
- Testing
- Deployment
- Maintenance

## Waterfall

- Phases

  - Feasibility analysis
  - Requirements analysis & specification
  - Design
  - Implementation (Programming) & Testing
  - Deployment & Maintenance

- Model

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
    - Allows PM to easily plan & control execution
    - Well known by non-professional, easy to use for communication
  - Disadvantages
    - Only suitable for real problems when sw requirements are clearly defined, complete & fixed from beginning (before Design phase)
    - Not suitable for long-running pjs
    - Those pjs that may have risk or uncertainty factors
    - Hard to have initial results (versions) soon

- When to use

  - sw requirements are clearly defined, complete & fixed
  - definition of product (sw sys) does not change
  - related & necessary technologies are mastered
  - resources & experience of sw dev team are sufficient
  - time of pj execution is short

## Prototyping model

- Phases
  - Requirements
  - analysis
  - Quick design
  - Prototype building
  - Prototype evaluation
  - Design
- Model

  - Instead of fixing requirements before proceeding with design or implementation, a prototype is built to understand exact sw requirements
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
    - Using a prototype as a working model of sys, users gain a better understanding of sys being built
    - Errors, problems can be detected early
    - Early to get evaluation feedback from users for better solutions
    - Missing functions can be discovered early
    - Functions unclear or difficult to operate may be detected
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
  - developing "look and feel" or UI
    - because these features are difficult to describe by documentation, but obtained through trial use
  - customers ask for proof of feasibility
  - demos needed for senior management board
  - technology problems need to be tried & tested

## Spiral

- Model

  - based on a hybrid combination of iterative of Prototyping & sequential of Waterfall
    - Focus on risk analysis
  - Dev through a series of incremental releases
    - In initial iterative steps of dev, versions can be simply sketched models on paper or prototypes
    - In later iterative dev steps, increasingly mature versions are created

- Advan & disadvan

  - Advantages
    - Focus on risk analysis, reduce risks in pjs
    - Suitable for large & particularly important pjs
    - New functions may be added later
    - Initial versions of sw sys are created early
  - Disadvantages
    - High cost (time, resources, money) to apply
    - Risk analysis requires high skills & experience
    - success of pj depends strongly on risk analysis phase
    - Not suitable for small pjs

- When to use
  - When assessment (analysis) of costs & risks is important
  - For medium-high-risk pjs
  - Users are uncertain about their needs
  - Complex & large sw requirements
  - Need to develop a new product line
  - Desire for significant changes (careful research & investigation is required)

## Agile

- Model

  - incremental & iterative
  - Dev through incremental & rapid cycles
  - Helps create small-scale enhanced versions
    - where a next version is built on features of previous one
  - Each enhanced version is carefully tested to ensure sw quality
  - Used for sw dev pjs that require quick completion times
    - Extreme Programming (XP) is one of famous methods belonging to agile model

- Advan & disadvan

  - Advantages
    - Satisfy customers with agile enhanced sw versions
    - Emphasis on interactions between actors rather than processes & tools (customers, developers, & testers constantly interact with each other)
    - Frequent communication between business analysis & programming team
    - Adapt (response) quickly to changing requests
    - Even allowing changes of sw requirements are added later
  - Disadvantages
    - For large sw sys, this agile model makes it difficult to estimate necessary costs & effort at beginning of SDP
    - Less emphasis on required design & documentation
    - Usually only senior developers can make necessary decisions during dev
      - not suitable for inexperienced developers, unless working in conjunction with experienced ones

- When to use

  - New changes can be implemented at low cost, by frequent creation of enhanced versions
  - To implement a new feature, developers only need a few days, or even a few hours to implement
  - Unlike waterfall, in agile, planning is (much) less cost
  - assumes that user needs will (often) change
  - Changes can always be requested & features can always be added or removed based on customer feedback
  - Both developers & users of sys find they have more freedom of time & choices than models that strictly follow a sequence of steps (waterfall)

## RUP

- Rational Unified Process is a modeling process using modeling language UML

### Basic principles

- Iteration & incremental
  - pj is divided into short loops or stages for easy control
  - At end of each loop, executable part is produced in a gradually added
- Focus on architecture

  - complex sys is divided into modules for easy deployment & maintenance
  - architecture is presented in 5 different views

- Led by use cases

  - Use cases influence every phase of sys dev, basis for
    - defining loops & enhancement
    - dividing work within team
  - Needs understanding: Detect use cases
  - Analysis: Dive into description (i.e., specification) of use cases
  - Design & implementation: Build sys according to use cases
  - sys testing & acceptance: Follow use cases

- Control risks
  - Early detect & eliminate risks to pj

### Main phases

- Inception
  - Give an overview of sw sys (functions, performance, technology) & sw dev pj (scope, goals, feasibility)
  - Conclusion of whether to develop or give up pj?
- Elaboration
  - More detailed analysis of sys (functions & static structures)
  - Propose a sys architecture prototype
- Construction
  - Focus on sys design & implementation
  - sys architecture is detailed & edited
  - Finishes when a complete sys with accompanying technical documentation is created
  - Take most time & effort
- Transition
  - Transfer sys to end users: data conversion, installation, testing, training

### Main steps

1. Preliminary study

   - like Inception

1. Identify & describe use cases

   - Understand user needs & identify use cases
   - Each use case must be specified (described) in form of a scenario and/or a sequence diagram

1. Application domain modeling

   - Provide class diagrams that reflect all concepts & businesses
   - classes here are domain classes (not design classes)

1. Define classes / objects involving in use cases

   - For each use case, define entity, control, boundary classes

1. Modeling interactions in use cases

   - Objects interact by exchanging messages
   - Create use case scenarios: Sequence, Communication diagrams

1. Behavior modeling

   - Control objects have ability to react to events coming from outside
   - Use state machine diagrams to describe behavior of control objects

1. Create UI prototype

   - Use GUI design tools to create (design) interfaces prototype early, making sys’s modeling & implementation easier

1. Design sys architecture

   - Design sys’s overall architecture
   - Divide into sub-sys
   - Use component diagrams to describe physical components
   - Use deployment diagrams to describe arrangement & deployment of sys's executable components to hardware & infrastructure platform

1. Detailed design

   - For classes, associations, properties, methods
   - Determine sys’s implementation solution

1. Implementation

   - Programming & testing
   - sys is approved (accepted) on use cases

# Analysis of environment & needs

## Goal

- This is preliminary study step
- Investigate & study about environment & business context of sys to be built
- Identify functional & non-functional requirements, risks & constraints
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
- Describe operation of users, equipment & computers in a business environment

- include
  - Business goal
  - Main tasks/main functions
  - Business processes
    - Should be described (presented) by activity diagrams
  - Types of information used in sys
  - Requirements for sys to be built about
    - functions
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

# Function analysis

## Goal

Give a preliminary look at sys's functionality

Business processes
Functional requirements

Function analysis is only intended to show major
functions (sys’s requirements)

Without going further into minor functions

Because currently & commonly used method of
analysis & design (taught in this course) is objectoriented (not function-oriented)

SAD

4

Modeling business processes by activity diagrams (1)

Goal of modeling business processes

Usually, pj will be started with a Preliminary Research
step to understand Business Environment of sys to
be built

In that environment, users, equipment, & computers work
together according to certain Business Processes

Business Processes
Diagrams

are

often

SAD

described

using

Activity

5

Modeling business processes by activity diagrams (2)

Goal of modeling business processes (2)

Activity Diagram is a diagram that describes activities following
flow from one activity to another

Activity Diagram may be used to describe:
A business process
Execution logic of a use case or a group of use cases
Execution logic of a usage scenario
Execution logic of a complex operation

Activity diagrams are UML models equivalent to block diagrams
or data flow diagrams in Function-oriented Analysis and
Design method
SAD

6

Modeling business processes by activity diagrams (3)

Activities & Transitions

An activity diagram is a directed graph, consisting of: Nodes are
activities, Edges are transitions, Start node (bold black dot: ),
and End node(s) (bold black dot with border:
)
Activity is a job, can be handled by hand – example: form filling,
or processed by computer – example: display information on the
screen

Representation of an activity:

Name of Activity

Transition is transition from one activity to another

Representation of a transition:
Activity 1

SAD

Activity 2

7

Modeling business processes by activity diagrams (4)

Branching

A guard ( ) is a condition check, attached to a transition, to
indicate that transition is performed only when this condition
is satisfied

To support branching, UML provides 2 kinds of guards:
A decision node: A single incoming flow & multiple
outgoing flows (these outgoing flows must be mutuallyexclusive);
A merge node: Multiple incoming flows & a single outgoing
flow (this merge point is passed when an incoming flow
occurs). Merge node should not be used to synchronize
concurrent flows!

SAD

8

Modeling business processes by activity diagrams (5)

Example of a decision node:
Checking temperature

[too cold]
Heating

[too hot]
Cooling

SAD

9

Modeling business processes by activity diagrams (6)

Synchronization (of concurrent flows)

In an activity diagram, synchronization bars are used to open or
close parallel execution branches:

Opening parallel execution branches
by a synchronization bar to show a single
incoming transition & multiple
Stop heating
outgoing ones – called a fork

Closing parallel execution branches
by a synchronization bar to show multiple
incoming transitions & a single
outgoing one – called a join

[too hot]

Ventilating

Checking temperature

A join can be passed only when all incoming execution
branches complete
SAD

10

Modeling business processes by activity diagrams (7)

Line-separating and
partitioning

An activity diagram may be lineseparated, like swim-lanes in a
swimming pool. Each activity
must be placed in a line, and
each line shows execution of
one or more objects. Transitions
may change lines freely.

An activity may be partitioned,
each partition contains activities
that have some characteristic in
common. For example, a partition
for major usage scenario and
several other partitions for minor
ones.
SAD

11

Modeling business processes by activity diagrams (8)

Object creation & Object flow

In an activity diagram, we want to specify that some activity
creates an object, or modifies object's state, or takes as input
an object for processing => We draw additional objects (with their
states, if necessary) in activity diagram, & connect those
objects to related activities with dashed arrows (called object
flows). An object flow from one activity to an object & then
continue to another activity can be seen as a control flow (a
transition) between two activities.

Example: following figure shows a sales process, where an
object (“Đơn hàng”) has been created & changed state through
activities.

SAD

12

Modeling business processes by activity diagrams (9)

Object creation & Object flow (2)

A sales
process:

SAD

13

Modeling functional requirements by use
case diagrams (1)

Goal of modeling functional requirements

Define major sys functions expected by users (called
functional requirements)

Describe analysis results with UML use case diagrams

order of work is as follows:
Modeling work environment of sys by actors
Modeling requirements by use cases
Determining relations (actors, use cases)
Creating use case diagrams

SAD

14

Modeling functional requirements by use
case diagrams (2)

Modeling work environment of sys by actors

Actors is role of one or more users or external (i.e.,
outside sys to be built) objects that interact with
sys

Types of actors:

Users vs. external sys/objects

Primary vs. secondary (a.k.a. supporting)

Representation of actors:

<<actor>>
External sys
Customer

SAD

15

Modeling functional requirements by use
case diagrams (3)

Modeling requirements by use cases

Definition of use case:
A use case is a representation of a set of sys
actions that provide a result to an actor

Characteristics of a use case:
A use cases must be associated with one or more actors
A use case must lead to a specific result
A use case must be a set of actions

SAD

16

Modeling functional requirements by use
case diagrams (4)

Modeling requirements by use cases

Representation of a use case:

Specification of a use case:
In natural language

Rút tiền

Name of use case
Description of usage purpose
(Primary, secondary) actors
Trigger (event)
Pre-conditions
Post-condition
Main (a.k.a. normal) flow
Alternative flows

Supplemented by an activity diagram or a sequence diagram
SAD

17

Modeling functional requirements by use
case diagrams (5)

Determining relations
There are different types of relations:

a) Generalization between actors

Actor A is a generalization of actor B, if B inherits all the
characteristics of A

Representation:

Online customer (B)
SAD

Customer (A)

18

Modeling functional requirements by use
case diagrams (6)
b) Communication between an actor & a use case

If actor & use case communicate with each other

Representation:
Withdraw
money
Customer

If communication is one-way, use arrow

SAD

19

Modeling functional requirements by use
case diagrams (7)
c) Generalization between use cases

Use case X is a generalization of use case Y, if Y inherits all the
characteristics of X (can modify & add)

Representation:
Withdraw
money

Withdraw cash

SAD

Withdraw by
transfer

20

Modeling functional requirements by use
case diagrams (8)
d) Inclusion between use cases

If use case X always include content of use case Y into the
content of X at a position (i.e., inclusion point) specified in the
specification of X

X (use case at beginning of arrow) is called base
use case

Representation:

Base use case
Withdraw
money

«include»
Authenticate
customer

SAD

21

Modeling functional requirements by use
case diagrams (9)
e) Extension between use cases

If use case X conditionally include content of use case Y
into content of X at a position (i.e., extension point) specified
in specification of X

X (use case at end of arrow) is called base use
case

Representation:

Base use case
Withdraw
money

Condition: {User requests priority}

«extend»

Quick
withdrawal

Extension point: Request for priority
SAD

22

Modeling functional requirements by use
case diagrams (10)

Creating use case diagrams

Nodes are actors & use cases:
Teacher

Select
courses

Edges can be either of 4 types:
Generalization (between actors or use cases):

Communication between actor & use case:

Inclusion between use cases:

Extension between use cases:

SAD

<<include>>
<<extend>>

23

Illustrative example exercise (1)
(A) Modeling business processes
Đầu bài: Để nâng cấp hệ thống thông tin của mình, một công ty muốn,
trong bước đầu, vạch ra một quy trình đào tạo (QTĐT) cho nhân viên
của mình, để sau đó tin học hoá một phần quy trình này

1. QTĐT bắt đầu khi có một Nhân viên (NV) gửi đến Người phụ trách
   đào tạo (PTĐT) một đề nghị được đi đào tạo. Người PTĐT xem xét đề
   nghị này và đưa ra trả lời đồng ý hay không đồng ý.
2. Nếu đồng ý, Người PTĐT tìm trong danh mục cơ sở đào tạo (CSĐT)
   một nơi có các lớp đào tạo thích hợp, thông báo nội dung đào tạo lại
   cho NV đã xin đi đào tạo, cùng với một danh sách các kỳ học sẽ mở tới
   đây. Khi NV đã chọn kỳ học, Người PTĐT gửi một đăng ký cho NV đó
   tới cơ sở đào tạo.
   SAD

24

Illustrative example exercise (2)
(A) Modeling business processes
Đầu bài (…tiếp theo)

3. Nếu sau khi đăng ký hoặc sau khi gửi đề nghị đào tạo, mà NV không
   thể tham dự được, NV phải báo sớm cho Người PTĐT để huỷ đăng ký
   hay huỷ đề nghị đào tạo.
4. Sau khi đào tạo xong, NV phải nộp lại cho Người PTĐT một giấy xác
   nhận sự có mặt và giấy nhận xét kết quả học tập.
5. Người PTĐT kiểm tra lại hoá đơn mà CSĐT gửi tới, trước khi
   chuyển cho kế toán trả tiền.

SAD

25

Illustrative example exercise (3)
(A) Modeling business processes
Bước 1: MHH quy trình trên bằng một biểu đồ ca sử dụng (mức đỉnh)

Để MHH nghiệp vụ (NgV), ta dùng các biểu tượng sau, do Jacobson

đề xuất (được dùng trong RUP và trong Rational Rose 2000):

Quy trình NgV Tác nhân NgV

Nhân viên NgV

Biểu đồ ca sử dụng
NgV (mức đỉnh):

Nhân viên

Thực thể NgV

Gói NgV

Cơ sở ĐT
Quy trình
đào tạo

Người PTĐT
SAD

Kế toán
26

Illustrative example exercise (4)
(A) Modeling business processes
Bước 2: Mô tả QTĐT bằng một biểu đồ hoạt động, có phân tuyến
:Nhân viên

:Người PTĐT

:Cơ sở ĐT

:Kế toán

Lập đề nghị
Xem xét đề nghị
[từ chối]
[chấp nhận]

Tìm CSĐT
Chọn kỳ học

Liên lạc CSĐT
Đăng ký ĐT

Đi đào tạo
Lập HĐ
Kiểm tra HĐ
Chi HĐ
SAD

27

Illustrative example exercise (5)
(A) Modeling business processes
Bước 2 (tiếp): Thêm vào biểu đồ hoạt động các đối tượng NgV đã được sản sinh cùng
với trạng thái của chúng nếu có
:Nhân viên

:Người PTĐT

:Cơ sở ĐT

:Kế toán

Lập đề nghị
Đơn xin ĐT
{chờ duyệt}

Xem xét đề nghị
[từ chối]
[chấp nhận]

:Công văn y/c

Tìm CSĐT

Chọn kỳ học
Đơn xin ĐT

:Giấy triệu tập

Liên lạc CSĐT

Đi đào tạo

{đã thực hiện}

{đáp ứng}

Đăng ký ĐT

{chờ đăng ký}

Đơn xin ĐT

Đơn xin ĐT

Lập hóa đơn

:Hoá đơn

:Phiếu chi

Kiểm tra HĐ
SAD

: Nhận xét

Chi HĐ

28

Illustrative example exercise (6)
(B) Modeling functional requirements
Bước 3: Từ mô hình nghiệp vụ, xác định phạm vi của Hệ thống (HT) tin học hóa
:Nhân viên

:Người PTĐT

:Cơ sở ĐT

:Kế toán

Lập đề nghị

HT tin
học hoá

Xem xét đề nghị
[từ chối]

[chấp nhận]

Tìm CSĐT
Chọn kỳ học
Liên lạc CSĐT
Đăng ký ĐT
Đi đào tạo
Lập HĐ
Kiểm tra HĐ
Chi HĐ
SAD

29

Illustrative example exercise (7)
(B) Modeling functional requirements
Bước 4: Xác định các yêu cầu của Hệ thống tin học hoá (Hệ thống YCĐT)

Hệ thống YCĐT cho phép bắt đầu một yêu cầu đào tạo và theo dõi nó cho đến khi
hoàn tất việc đăng ký đào tào cho một nhân viên
Hệ thống YCĐT phải tin học hoá các hoạt động nghiệp vụ sau:

Soạn thảo một đề nghị đào tạo (Nhân viên);

Xem xét một đề nghị (Người PTĐT);

Tìm cơ sở đào tạo (Người PTĐT);

Chọn lớp và kỳ học (Nhân viên);

Đăng ký đào tạo (Người PTĐT).

Muốn đáp ứng các yêu cầu trên, Hệ thống phải quản lý một danh mục CSĐT mà Nhân
viên có thể đọc và Người PTĐT có thể viết vào đó và tổ chức nó theo chủ đề
Lưu ý: Nhân viên có thể huỷ Đăng ký đào tạo, hoặc huỷ Đề nghị đào tạo

SAD

30

Illustrative example exercise (8)
(B) Modeling functional requirements
Bước 5: Lập biểu đồ ca sử dụng cho Hệ thống YCĐT
Từ các hoạt động nghiệp vụ,
phát hiện các ca sử dụng:

Đề nghị được đào tạo (ĐT),

Đăng ký ĐT,

Huỷ yêu cầu ĐT,

Tra cứu danh
mục CSĐT

Quản lý danh
mục CSĐT

Nhân viên
Đề nghị ĐT

Huỷ yêu cầu

<<include>>

Tra cứu danh
mục CSĐT

Đăng ký ĐT
Người PTĐT

<<include>>

Quản lý danh
mục CSĐT
SAD

<<actor>>
Cơ sở ĐT

31

Illustrative example exercise (9)
(B) Modeling functional requirements
Bước 6: Mô tả chi tiết (đặc tả) ca sử dụng ‘Quản lý danh mục CSĐT’
I. Mô tả chung

Tên: Quản lý danh mục CSĐT

Loại: Chi tiết

Nội dung tóm tắt: Người PTĐT có trách nhiệm cập nhật thường xuyên
danh mục CSĐT, trong đó chứa các thông tin cần thiết về các CSĐT. Phần
lớn các chỉnh sửa đều bắt nguồn từ các CSĐT.

Tác nhân: Người PTĐT.

Ngày lập: 20/11/2015

Ngày cập nhật: 01/02/2016

Phiên bản: 3.0

Người lập: Lê Anh (leanh@company.com)

SAD

32

Illustrative example exercise (10)
(B) Modeling functional requirements
Bước 6 (tiếp): Mô tả chi tiết (đặc tả) ca sử dụng ‘Quản lý danh mục CSĐT’

II. Mô tả các kịch bản
Điều kiện tiên quyết (Pre-conditions): Người PTĐT đã được giao trách nhiệm

Kịch bản chính (Normal flow):

1. Ca sử dụng bắt đầu khi một CSĐT báo cho Người
   PTĐT các thay đổi của họ
2. Người PTĐT có thể bổ sung một CSĐT mới, loại
   bỏ một CSĐT cũ, hay cập nhật thông tin của một
   CSĐT đang tồn tại.
   Khi bổ sung hay cập nhật, Người PTĐT có thể điều
   chỉnh lịch học của các lớp đào tạo

3. Hệ thống thông báo cho các người dùng đang kết
   nối hãy coi chừng dùng phải một phiên bản cũ của
   danh mục CSĐT
   Khi loại bỏ một CSĐT cũ, hệ thống sẽ cho: Người
   PTĐT biết các NV đã đăng ký vào các lớp bị loại bỏ,
   và các NV đó biết các đăng ký đã bị huỷ bỏ

4. Khi cần, Người PTĐT có thể bổ sung thêm một loại
   hình đào tạo mới
5. Người PTĐT xác nhận các điều chỉnh đã thực hiện

6. Hệ thống thông báo cho các người dùng đang kết
   nối là đã có một phiên bản mới của danh mục CSĐT

SAD

33

Illustrative example exercise (11)
(B) Modeling functional requirements

Các kịch bản ngoại lệ (Alternative flows) có thể:

A1: Thông tin không đầy đủ.
Kịch bản A1 khởi động ở điểm 2 của kịch bản chính.
A2: Khi các thông tin liên quan tới một CSĐT mới là không đầy đủ (vd:
thiếu ngày cho các lớp đào tạo), thì CSĐT đó được đưa vào danh mục
CSĐT nhưng chưa cho đăng ký, và CSĐT đó phải được cập nhật sau.
Kịch bản chính tiếp tục từ điểm 2

Các ràng buộc (constraints):

Xung đột: Ca sử dụng mỗi lần chạy chỉ làm việc với một Người PTĐT
Sẵn dùng: Danh mục CSĐT có thể truy cập được trong khoảng thời gian
từ 09:00 thứ hai đến 17:00 thứ sáu. Các cập nhật cần hạn chế tối đa
trong khoảng thời gian đó.
SAD

34

sys Analysis and
Design
(IT3120E)
Quang Nhat Nguyen
quang.nguyennhat@hust.edu.vn

Academic year 2022-2023

Content:

intro of OO SAD

intro of modeling language UML

intro of SDP

Analysis of environment & needs

Function analysis

Structure analysis

Interaction analysis

Behavior analysis

Design of sys’s overall architecture

Class detail design

UI design

Data design

SAD

2

Structure analysis

Goal of structure analysis

Objects & classes

Determining domain classes

Determining classes involving in use cases

Illustrative example exercise

SAD

3

Goal of structure analysis
Preliminary determine main classes that

make up sys

This is not complete (i.e., final) version of the
classes

SAD

4

Objects & classes

Definition & representation of objects & classes

Attributes

Operations

Relations

Dependency
Generalization
Association

Class diagram & Object diagram

SAD

5

Definition of object & class (1)

An object (in IT) is an abstract representation of a (physical
or conceptual) entity that has a clear identity & boundary in
real world, including state & behavior of that entity,
aiming at simulating or controlling that entity

state of an object is represented by a set of attributes. At a
time, each attribute of object has a certain value.
behavior of an object is represented by a set of operations,
which are services it can perform when requested by another
object.
identifier of an object is what distinguishes it from another

SAD

6

Definition of object & class (2)

A class is a description of a set of objects that share the
same attributes, operations, relations, constraints, and
semantics

A class is a type, & each object of class is an
instance

SAD

7

Representation of objects & classes

Representation of classes
Class-A

Class-A

attributes

Class-A

operations

Representation of objects
object-x :Class-A

object-x

attributes = values

SAD

:Class-A

8

Attributes (1)

An attribute is a named property of a class that takes a value
for each object of that class at a time

Syntax of an attribute:
[Visibility] [/] Name [: Type]
[Multiplicity] [= Initial value]
[{Property-string}]

SAD

9

Attributes (2)
[visibility] [/] name [: type] [multiplicity]
[= initial value] [{property-string}]

Visibility tells how attribute is seen & used by
other classes

Private, denoted by '-', if attribute is not accessible from any
other class
Protected, denoted by '#', if attribute is only accessible from
classes that inherit current class
Package, denoted by '~', if attribute is accessible from
classes belonging to same (i.e., most inner) package of
current class
Public, denoted by '+', if attribute is accessible from any other
class
SAD

10

Attributes (3)
[Visibility] [/] Name [: Type] [Multiplicity]
[= Initial value] [{Property-string}]

Type is type of attribute's values

Basic types like Integer, Real, Boolean

Structured types like Point, Area, Enumeration

Type is another class

Multiplicity is number of possible values assigned
to attribute

Example: [0..1] shows that attribute is optional (i.e., it may
take no or one value)

SAD

11

Attributes (4)
[Visibility] [/] Name [: Type]
[Multiplicity] [= Initial value] [{Propertystring}]
Initial value is default value assigned to attribute
when an object is instantiated from that class
Property-string defines values that can be assigned
to attribute, usually used for enumeration-typed
attributes

Example: status: Status = unpaid {unpaid, paid}

SAD

12

Attributes (5)

An attribute may have class scope if it reflects the
general characteristics of class

Class-scoped attributes must be underlined
Example: Attribute number-of-invoices
Invoice

of class

An attribute is derived, if its value is calculated from the
values of other attributes of class

Derived attributes must include a slash '/' at beginning
Example: /age (while attribute /birthday exists)

SAD

13

Operations (1)
An operation is a service that an object can respond to
when requested (via a message)
Operations are implemented as methods

Syntax of an operation:
[Visibility] Name [(Parameter list)] [:
Return type] [{Property-string}]

Visibility is defined same as for attributes
Parameter list is a list of parameters, separated by commas,
each of form:
[Direction] Name : Type [= Default value]

SAD

14

Operations (2)

Direction may be either of in, out, inout or return
depending on parameter is: may not be modified (in),
may be modified to communicate information to caller
(out), may be modified (inout), or to return result to
caller (return)
Default value is value to be used when the
corresponding parameter is missing in call

Property-string includes pre-conditions, postconditions, effects on object state, etc.

SAD

15

Relations

There are three possible relationships between classes:

Dependency

Generalization

Association

SAD

16

Dependency relation (1)

Dependency relation is used to express a (dependent)
class that is affected by any changes in another
(independent) one
opposite direction is not necessarily

Usually, dependent class needs to use the
independent one to specify or implement it

UML represents dependency relation with a dashed
arrow from dependent class to independent one

SAD

17

Dependency relation (2)
A

B

operation1()

getC(): C

C

operation2()

operation1() {
b.getC().operation2()
}

Use a stereotype to express specific
type of dependency, for example:
<<use>>, <<refine>>

SAD

18

Generalization relation (1)

Generalization is extraction of common characteristics of
many classes to form a simpler (i.e., more generalize) class

On contrary, specialization is enhancement (i.e.,
addition) that adds some new characteristics from a given
class, forming a more specific class

Called a sub-class

A class can have no, one or more super-class(es)

Called a super-class

A class with only one super-class is called simple inheritance
A class with multiple super-classes is called multiple inheritance

A class that has no super-class & has sub-classes is called
a root class (i.e., base class)
SAD

19

Generalization relation (2)

term “inheritance” is commonly used in
programming languages to describe a sub-class that has
all attributes, operations, & relations described in
its super-class

Sub-classes can add new (own) attributes, operations, and
relations
A sub-class can re-define (i.e., overwrite) an operation of the
supper-class: Polymorphism

Representation of generalization relation:
Tiger

SAD

Animal

20

Generalization relation (3)

Through generalization, we can make abstract classes, i.e., those
classes that have no instance objects, but are only used to describe
common characteristics of sub-classes

An abstract class usually contains abstract operations, i.e., those
operations with only title (i.e., name) & without implementation

Abstract operations must be redefined (i.e., overwritten) & implemented
in sub-classes
name of abstract class & title of abstract operation must
be italicized & may include property string {abstract}

Example: Animal is an abstract class generalized from classes
Horse, Tiger, Bat. It has an abstract operation sleep(). This
abstract operation will be specifically implemented in sub-classes
Horse, Tiger, Bat in different ways, but keeping same name
sleep()
SAD

21

Association relation (1)

Link represents some actual relation between
instances (objects) of two classes
Example: wife-husband link, teacher-student link,
motorbike-owner link, customer-invoice link, etc.

Association is a relation between two classes,
consisting of a set of links of same type (i.e., of the
same meaning) between instances of those two classes
This is a relation (in mathematical sense)
between two sets (two classes)

SAD

22

Association relation (2)

Representation of link:

giáp: Student
ất: Student

hust: University

bính: Student
đinh: Student

neu: University

mậu: Student

Representation of association:
University

SAD

study-at

Student

23

Association relation (3)

Navigation on an association

A link between two objects (of two classes in an association)
means that objects "know each other"

By link, from one object we can find other

Navigation may be bi-directional (i.e., from both ends) on an
association

Navigation may be restricted in one direction

Then we add an arrow to navigated end & a slash to the
unnavigated end

Invoice

contains

SAD

Address

24

Association relation (4)

Role

In an association between two classes, each class plays a
different role

role name (with first letter in lowercase) can be appended
to each end of link (thus role is also called name of an
association end)

In terms of meaning, a role represents a subset of objects of the
corresponding class
study-at

student

School

wife

Person
employer
institution

teach-at

teacher

SAD

husband

getmarried
25

Association relation (5)

Multiplicity

Each end of association may also contain a multiplicity to indicate the
(minimum & maximum) number of instances of that end participating in
association with one instance at other end

Commonly used values of multiplicity:
1

1 & only one

0..1

0 or 1

m..n

From m to n (m & n are natural numbers)

0.._ or _

From 0 to many

1..\*

From 1 to many
1..\*

student \*

School

Person

1..\*

teacher \*

SAD

26

Association relation (6)

Qualifier

Search problem: Given an object at one end of association, find an
object or set of objects connected to it at other end

To reduce number of objects found, we can limit search area to
(values of) certain attributes

These attributes are called qualifiers

Such attribute is shown in a small box attached to end (class)
of association, where navigation originates

Thus, qualifier is applied to 1-to-many or many-to-many associations,
to reduce from many to 1 (or 0..1), or to reduce from many to many (but
number is less)
Bank

bankName

accountnumber

SAD

0..1 Account

accountnumber
27

Association relation (7)

Association class

An association itself may also need to have specific attributes

UML supports this by association classes

Association class is a class as usual (with attributes, operations,
and associations), but name-box can be optionally named or left
blank, & it is attached to association by a dashed line
Company \*
employer
institution

1..\*
employee

Person

Job
description
employed date
salary

SAD

28

Association relation (8)

N-ary association

There can be an association between more than two classes, in the
sense of a plural (i.e., a tuple-n) relation
An n-ary association is represented by a small rhombus (diamond)
symbol, connected by solid lines to participating classes and
may also have an association class attached
Course

Room

Lecture

Class

SAD

29

Association relation (9)

Aggregation

In many association relations, two parties (i.e., classes) are
considered equal, neither side is emphasized more than other

However, sometimes we want to model a "whole-part" relation
between a class of "whole" objects & a class of "part" objects.
This is aggregation association, represented by attaching an
empty rhombus (diamond) symbol to end at “whole” side
of association
University

Example: Class Student (i.e., “part” class) has an
aggregation association with class University (i.e., the
“whole” class); & an object of class Student has
“study-at” relation with multiple objects of class
University
SAD

1..\*
studyat

- Student

30

Association relation (10)

Composition

A composition is a type of an aggregation with stronger ownership
relation, in that a “part” class belongs only to a single “whole” class
and “whole” class is responsible for creating & destroying the
“part” class
When “whole” class is destroyed, “part” class is also
(automatically) destroyed
Composition is represented by attaching a solid rhombus (diamond)
to end at “whole” side of association
University

Car

1
belong
1..\* -to

1

1

Engine

-engine: Engine

+start()

+start()

Faculty
SAD

31

Class diagram & Object diagram

A class diagram is a diagram that shows a set of classes & the
relations (association, aggregation, composition, generalization,
dependency) between them

Class diagrams are used to model static structures of sys,
including all declared elements

An object diagram represents static structure of a class diagram in
a specific way
Objects instead of classes, Links instead of associations
Person employee

long: Person
manager

- 1 manager

việt: Person
SAD

manager
hùng: Person

32

Determining domain classes

Goal & execution process

Identifying domain concepts

Adding associations & attributes

Generalizing classes

SAD

33

Goal & execution process
Starting from concepts of things in application
domain, we abstract them into classes called domain
classes
These domain classes are often only used to reflect and
simulate real-world things, so their role is often just to
store & provide information about those things
Execution process:

Identifying domain concepts
Determining associations & attributes
Generalizing concepts

SAD

34

Identifying domain concepts (1)

Search sources
Domain concepts are concepts about things (concrete or
abstract) used by users & business experts when they
discuss about that domain
To search for domain concepts, we rely on:

Knowledge of business domain
Interviews with users & business experts
document that describes an overview of sys and
needs
documents that describe use cases (created in the
previous step of SDP)

SAD

35

Identifying domain concepts (2)

How to identify concepts?

Read sys description document (i.e., describing
requirements):

Nouns can be objects or attributes,

Verbs can be operations

Based on that, identify following objects:

Entity (e.g., motorbike, airplane, sensor, etc.)

Role (e.g., teaching, monitoring, etc.)

Event (e.g., landing, interrupting, motorbike registration, etc.)

Interaction (e.g., lending, discussion, etc.)

Organization (e.g., company, faculty, class, etc.)
SAD

36

Identifying domain concepts (3)

Name & assign responsibility

Next is naming & assigning responsibility to each of the
newly defined classes
Responsibility describes role & use purpose of class, not
structure of that class
Although latter responsibility will allow us to define structure
(i.e., properties & associations) & behavior (i.e.,
operations) of class
Student

Information needed to
register & calculate tuition
fees for a student. Student is
a person who is allowed to
register to credit courses of a
university.

SAD

37

Identifying domain concepts (4)

Name & assign responsibility (…continued)

Naming & assigning responsibility to a class also help to check
if class selection is reasonable:

If you can choose a name & assign clear & concrete
responsibility, then class selection is good;

If you can choose a name, but responsibility is same as
(or very similar to) responsibility of another class, then you
should combine those two classes into one;

If you can choose a name, but responsibility is too long (too
complex), then you should split that class into several ones;

Difficult to choose a reasonable name or describe the
responsibility, then you should analyze more deeply to choose
appropriate representations
SAD

38

Determining associations & attributes (1)

First, many attributes & associations of domain classes
can be directly determined:
From document describing sys & needs,
From statements of domain experts & users, and
From responsibilities of classes defined in the
previous step

Later, we will add more associations & properties, as well
as add operations to classes, when we do analysis of
interaction & behavior of sys

SAD

39

Determining associations & attributes (2)

Example: From description of responsibility of the
class "Student", we have:
sentence "Information needed to register and
calculate tuition fees for a student" help us infer some
attributes such as name, student code, address, etc.
of class “Student”
sentence "Student is a person who is allowed to
register to credit courses of a university" help us infer
that there is an association between class
“Student” & class “CreditCourse” with the
association name maybe “register"
SAD

40

Generalizing classes

In order to optimize class representation model, we seek to extract
common parts between classes to form a more general class

For example, classes “Student” & “Lecturer” have common
attributes (e.g., name, id code, etc.) => We may need to define a more
generalized class (e.g., class “Person”)
Person
name
id code

Student
majors

Lecturer
term

SAD

41

Determining classes involving in use cases

Goal of determining classes involving in use cases

Procedure (of steps) to help determine classes
participating in use cases

Create a class diagram for each use case

SAD

42

Goal of determining classes involving in use cases

In previous step, we just studied domain, but not the
current sw application => classes determined are just
domain classes

These domain classes are same for every sw application of the
domain!

specifics of a sw application are in its use cases. So, to
study current sw application, we have to analyze the
structure & behavior of these use cases in depth.
A use case is viewed as a collaboration of several objects, including
domain classes & application-specific classes
purpose of this step is to analyze static structure of use
cases. We will have to do following tasks:

1. Determine classes involving in use cases
2. Add relations between classes to create a class diagram for
   each use case
   SAD

43

Determining classes involving in use cases (1)

use cases are studied (analyzed) to determine the
classes that participate in each of these use cases

classes that participate in use case are called
analysis classes, including 3 types:
Boundary class
Control class
Entity class

SAD

44

Determining classes involving in use cases (2)

Boundary classes, (a.k.a. dialog classes):

These are classes that communicate (exchange) information
between actors & sys:

Typically, they represent screens for communicating with the
users, allowing information to be collected or results to be displayed

They may also represent (hardware/sw) interfaces between
sys & devices that it controls or collects information

For each pair of (actor, use case), there must be at least one
boundary class

This main boundary class may in turn need auxiliary boundary
classes to delegate some of its overwhelming responsibilities

Usually, boundary objects have same lifecycle as with its
associated use cases
SAD

45

Determining classes involving in use cases (3)

Control classes:

These are classes that manage & control progress in a
use case, i.e., it is "engine" that makes use case progress
Control classes contain business rules & are intermediate
between boundary classes & entity classes, allowing from the
screen (UI) to manipulate information contained in
entity classes
For each use case, we need to create at least one control class
A control class, when moved to design phase, is not
necessarily going to exist as a real class, since its task can be
dispersed into other classes, but during analysis phase, it is
necessary to have it to ensure that functions or behaviors in the
use cases are not left out
SAD

46

Determining classes involving in use cases (4)

Entity classes:

These are business classes, determined directly from the
description of domain, & will be confirmed if they appear in the
use cases

Entity classes are persistent classes, i.e., classes whose data and
relations are retained (usually in databases or in files) after their use
cases finish

It is confirmed that an entity participate in a use case if the
information contained in that entity class is mentioned in use
case

Representation:

<<boundary>>

SAD

<<control>>

<<entity>>

47

Creating a class diagram for each use case (1)

Goal & requirements:
ultimate goal of Step 4 in RUP process (i.e.,
Determine classes participating in use cases) is to
draw a class diagram for each use case, to reflect the
static structure of collaboration (between classes)
diagram of classes participating in use case
will be foundation on which interactions
between classes take place, which we will explore in
depth in next step

SAD

48

Creating a class diagram for each use case (2)

diagram of classes participating in a use case
must include all determined classes & the
necessary structural elements (attributes, operations,
associations) of each class

attributes must store enough information about the
objects needed in collaboration
operations provide required service capabilities
of each class engaging in collaboration
associations create links between classes,
allowing them to know each other & communicate with
each other in collaboration

SAD

49

Creating a class diagram for each use case (3)

Adding attributes & operations:
entity classes temporarily have only attributes. These
attributes describe persistent information of sys
control classes temporarily have only operations. These
operations represent business processing logics,
business rules, & behaviors of sys
boundary classes have both attributes & operations:

attributes describe fields to collect information or to output
results. results are distinguished by notation of derived
attributes

operations represent actions that user performs on the
interface screen
SAD

50

Creating a class diagram for each use case (4)

Adding associations:

Boundary classes are only associated with control classes or with
other boundary classes. Usually, an association is one-way from
a boundary class to a control class, unless control class again
creates a new dialogue (e.g., a page displaying results).

Entity classes are only associated with control classes or with
other entity classes. An association of an entity class with a
control class is always one-way (from control class to the
entity class).

Control classes may be associated with all types of classes
(including also with other control classes)

SAD

51

Creating a class diagram for each use case (5)

Adding actors:
Finally, we add actors to class diagram
An actor is connected to only one (or several) boundary
class(es)

An actor is not associated with any control or entity class!
<<boundary>>
A_Boundary_Class
attr1
attr2
/result

Actor
đốitác

operation1()
operation2()

<<control>>
A_Control_Class

operation1()
operation2()

SAD

<<entity>>
An_Entity_Class
data_attr1
data_attr2
data_atrr3

52

Illustrative example exercise (1)
Mô hình hóa cấu trúc tĩnh được thực hiện dựa vào văn bản phát biểu bài
toán. Phát biểu đó được biên tập lại có lược bớt như sau:

1.

2.

3.

4.

5.

6.

QTĐT bắt đầu khi người phụ trách đào tạo (PTĐT) nhận được một đề nghị
đi đào tạo từ một nhân viên (NV).
Người PTĐT xem xét đề nghị này và đưa ra trả lời đồng ý hay không đồng
ý.
Nếu đồng ý, người PTĐT tìm trong một danh sách các lớp đào tạo để chọn
một lớp đào tạo phù hợp.
Người PTĐT thông báo nội dung của lớp đào tạo cho NV đã xin đi đào tạo,
cùng với một danh sách các kỳ học sẽ mở tới đây.
Khi người NV đã chọn kỳ học, người PTĐT gửi một yêu cầu đăng ký cho
NV đó tới cơ sở đào tạo.

Người PTĐT kiểm tra lại hoá đơn mà cơ sở đào tạo gửi tới, trước khi
chuyển cho kế toán trả tiền.
SAD

53

Illustrative example exercise (2)
Bước 8: MHH câu phát biểu thứ 1, sử dụng các biểu tượng của Jacobson.
“QTĐT bắt đầu khi người phụ trách đào tạo (PTĐT) nhận được một đề
nghị đi đào tạo từ một nhân viên (NV)”.
Chú ý các danh từ

QTĐT đã được xác định từ Bước 1 (của bài 5 – Phân tích chức năng) là một quy

trình nghiệp vụ, vậy không phải là lớp
Còn lại các danh từ: “người PTĐT”, “đề nghị ĐT”, “nhân viên” sẽ được mô hình
hóa thành các lớp
Nhân viên
1

Người PTĐT
1
gửi

nhận

1
Đơn xin ĐT

SAD

54

Illustrative example exercise (3)
Bước 9: MHH câu phát biểu thứ 2.
“Người PTĐT xem xét đề nghị này và đưa ra trả lời đồng ý hay không
đồng ý”.
Mở rộng mô hình trên, có chỉnh sửa vài chi tiết cho thích hợp hơn và thêm một
thực thể trừu tượng (Trả lời) cùng với 2 thực thể chuyên biệt (Đồng ý, Không
đồng ý)

xử lý

1
Người PTĐT

gửi

0..\*

0..1

Đơn xin ĐT

0..1

1
Nhân viên

1

Trả lời

Không đồng ý
SAD

Đồng ý
55

Illustrative example exercise (4)
Bước 10: MHH câu phát biểu thứ 3.
“Nếu đồng ý, người PTĐT tìm trong một danh sách các cơ sở đào tạo
(Catalô) một lớp đào tạo phù hợp”.

Catalô
1

0.._
0.._

Đơn xin ĐT

phù hợp với
0..1

SAD

Lớp đào tạo

56

Illustrative example exercise (5)
Bước 11: MHH câu phát biểu thứ 4.
“Người PTĐT thông báo nội dung của lớp đào tạo cho NV đã xin đi đào
tạo, cùng với một danh sách các kỳ học sẽ mở tới đây”.

Lớp đào tạo

1

1

1

Nội dung

SAD

mở theo
{ordered}
0..\*
Kỳ học

57

Illustrative example exercise (6)
Bước 12: MHH câu phát biểu thứ 5.
“Khi người NV đã chọn kỳ học, người PTĐT gửi một yêu cầu đăng ký cho
NV đó tới cơ sở đào tạo”.
tổ chức

1
Cơ sở ĐT

0..\*
Lớp đào tạo
1
mở theo
Đăng ký

học viên
0..\*
Nhân viên

0..\* {ordered}
0..1
Kỳ học

SAD

58

Illustrative example exercise (7)
Bước 13: MHH câu phát biểu thứ 6.
“Người PTĐT kiểm tra lại hoá đơn mà cơ sở đào tạo gửi tới, trước khi
chuyển cho kế toán trả tiền”.

Người PTĐT
1

gửi

kiểm tra
0..\*

0..\*

0..\* Hoá đơn
1

1 Cơ sở ĐT

về

xử lý

Kế toán
SAD

1
Đăng ký
59

Illustrative example exercise (8)

Bước 14: Tổng hợp các kết quả trên vào một biểu đồ lớp nghiệp vụ (lĩnh vực).
gửi

1
về
0..\*

Đăng ký

1

Kỳ học
0..\*
học viên

0..\*

xử lý

{ordered}

0..1

0..1

Hoá đơn
0..\*
kiểm tra

1

1

0..\*

Catalô
1

tổ chức

mở theo

0..\*

0..\*

phù hợp với 1
0..1
0.._
0.._
Lớp đào tạo
Đơn xin ĐT
1
1
0..1

gửi

Nhân viên
1
1

Cơ sở ĐT
1

xử lý

0..1

1

Người PTĐT
Trả lời

Nội dung
Kế toán

Không đồng ý
SAD

Đồng ý
60

Illustrative example exercise (9)

Bước 15: Chia cắt mô hình thành các gói theo các đơn vị nghiệp vụ và sửa lại
các liên kết cho nhẹ bớt sự phụ thuộc giữa các gói.
gửi

1

về
0..\*

0..1

1

{ordered}

0..1
Đăng ký

Kỳ học

Cơ sở ĐT
1

0..\*

tổ chức
mở theo

0..\*
học viên

Catalô
1

0..\*

0..\*

phù hợp với 1
0.._
1
0..1
gửi
0.._
Hoá đơn
Lớp đào tạo
0..
Nhân viên
0..\*
Đơn
xin
ĐT
1
1

- kiểm tra
  1
  1
  xử lý
  Catalô
  0..1
  Tài vụ
  xử lý
  1
  Đề nghị ĐT
  Người PTĐT
  1
  0..1

Trả lời
Nội dung
Kế toán
Không đồng ý
SAD

Đồng ý
61

Illustrative example exercise (10)

Biểu đồ gói thu được như sau (các phụ thuộc là một chiều):

Tài vụ
Đề nghị ĐT

Catalô ĐT

SAD

62

Illustrative example exercise (11)
Bước 16: Thêm các thuộc tính trường cửu (persistent) vào các lớp (vẽ
riêng cho từng gói)
Biểu đồ lớp của gói “Tài vụ”:
1
Người PTĐT
(từ gói Đề nghị ĐT)

gửi

kiểm tra

0..\*

0..\*

0..\* Hoá đơn
1

xử lý

ngàylập
hạntrảtiền
tổngtiền

Kế toán

tên
SAD

1 Cơ sở ĐT
(từ gói Catalô ĐT)

về
1
Đăng ký
(từ gói Đề nghị ĐT)
63

Illustrative example exercise (12)

Biểu đồ lớp của gói “Đề nghị ĐT”:
học viên
0..\*
Nhân viên

0..1

1

Kỳ học
gửi

0..\*

Đăng ký
ngày
họcphí

0..\*

0..\*

Đơn xin ĐT
ngàygửi
ngàyduyệt

xử lý

1
1
Người PTĐT

tên
email

phù hợp với

0..1

1

gửi

0..1

Lớp đào tạo
(từ gói Catalô ĐT)

0..\*
Trả lời
ngày

Không đồng ý
lýdo

Đồng ý

SAD

64

Illustrative example exercise (13)
Biểu đồ lớp

của gói
“Catalô ĐT”:

1

1

Catalô

tổ chức

nămhọc

0..\*

0..\*

1
1 Lớp đào tạo

1

mở theo

tênlớp
thờihạn
giá

Cơ sở ĐT
tên
địachỉ
điệnthoại
fax
email

0..\*
{ordered}

Nội dung
ngườihọc
mônhọctrước
mụctiêu
côngcụ
kếhoạch
SAD

Kỳ học
ngàybắtđầu
/ngàyKT
địađiểm

65

Illustrative example exercise (14)

Đến đây thì ta đã hoàn thành việc phát hiện các lớp lĩnh
vực (lớp thực thể) của ứng dụng

Việc phát hiện các lớp biên và các lớp điều khiển cho
mỗi ca sử dụng:
Xem đó là bài tập về nhà!

Việc phát hiện các lớp biên và các lớp điều khiển sẽ tiếp
tục được cập nhật khi chúng ta tiến hành việc Phân tích
hành vi (tương tác, ứng xử)
Sẽ được trình bày trong các bài học tiếp theo!
66
