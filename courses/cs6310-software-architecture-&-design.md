# Software Architecture & Design

    "Design creates culture. Culture shapes values. Values determine the future." - Robert L. Peters

- [P1L1 Introduction](/courses/cs6310-software-architecture-&-design.md#p1l1-introduction)
- [P1L2 Text Browser Exercise](/courses/cs6310-software-architecture-&-design.md#p1l2-text-browser-exercise)
- [P1L3 Design Concepts](/courses/cs6310-software-architecture-&-design.md#p1l3-design-concepts)
- [P2L1 Review of UML](/courses/cs6310-software-architecture-&-design.md#p2l1-review-of-uml)
- [P2L2 Object Oriented Analysis Exercise](/courses/cs6310-software-architecture-&-design.md#p2l2-bbject-oriented-analysis-exercise)
- [P2L3 UML Class Models](/courses/cs6310-software-architecture-&-design.md#p2l3-uml-class-models)
- [P2L4 Design Studies](/courses/cs6310-software-architecture-&-design.md#p2l4-design-studies)
- [P2L6 Formal Specification Exercise](/courses/cs6310-software-architecture-&-design.md#p2l6-formal-specification-exercise)
- [P2L7 OCL](/courses/cs6310-software-architecture-&-design.md#p2l7-ocl)
- [P2L9 Behavior Modeling](/courses/cs6310-software-architecture-&-design.md#p2l9-behavior-modeling)
- [P3L2 Overview of Artchitectural Styles](/courses/cs6310-software-architecture-&-design.md#p3l2-overview-of-artchitectural-styles)
- [P3L3 Artchitectural Views](/courses/cs6310-software-architecture-&-design.md#p3l3-artchitectural-views)
- [P3L4 Text Browser Exercise](/courses/cs6310-software-architecture-&-design.md#p3l4-text-browser-exercise)
- [P3L5 Non-Functional Reqs & Arch Styles](/courses/cs6310-software-architecture-&-design.md#p3l5-non-functional-reqs--arch-styles)
- [P3L6 Connectors](/courses/cs6310-software-architecture-&-design.md#p3l6-connectors)
- [P3L7 Acme](/courses/cs6310-software-architecture-&-design.md#p3l7-acme)
- [P3L8 Refinement](/courses/cs6310-software-architecture-&-design.md#p3l7-refinement)
- [P3L9 Middleware](/courses/cs6310-software-architecture-&-design.md#p3l7-middleware)
- [Resources](/courses/cs6310-software-architecture-&-design.md#resources)

## P1L1 Introduction

- **Objectives**
    - Express the **analysis and design**  of an application using the [**Unified Modeling Notation (UML)**]().
    - Specify **functional semantics** od an application using the [**Object Constraint Language (OCL)**]().
    - Specify and evaluate **software architectural styles**
    - Select and use appropriate **architectural styles**
    - Understand and apply **object-oriented design** techniques
    - Select and use appropriate **software design patterns**
    - Understand and participate in a **design review**

## P1L2 Text Browser Exercise

- Define **GUI elements** (based on Swing or SWT): FileNamger, ViewPort, and ScrollBar.
- Constract the **Analysis Model** with UML class-model diagram (rectangles for classes/components).
    - Each rectangle is divited vertically(from top to buttom): ClassNmame, Attributes(percepts), Operations.
- Add **Relationships** between the components: Associations, Aggregations, Generalization.
- Think about **Subtleties** which include special cases and uniques situations...

![alt text](/images/cs6310-display-diagram.png "UML Diagram")

## P1L3 Design Concepts

    "Design is the most creative part of software development..." - Prof. Spencer Rugaber

- **Design** is a deliberative, purposive planning.
- **Engineering** is a skilful or artful contrivance applying scientific and mathematical principles
- **Software Design** is a process of building a program while satisfying a problem's functional requirements and not violating its non-functional constraints. Contains two phases.

**Phases** 

- **Architectural design** is a process of identifying and assigning the responsibility for aspects of behavior to varios modules or components of a software.
- **Detail deisgn** is a process of specifying the behavior of each of the system components that you're identified during architectural design. 
    - **Psedo code; Program Design Language (PDL)** (keywords, data delcaration, syntax).
    - **Structure programming** (sequence, condidtion, repetitions).
    - **Flowcharts; call graphs** (directed graphs, computational units).
    - **Desicion tables** (rules, conditions, actions).
        
**Concepts**

- **Approaches** to Software Design. It's include 3 aspects: *method, representational, and validation.*
- **Design Documentation** is key concept in Software Design with *Subcomponents, Control Flow, Performance, Resources.*
- Low **Coupling** is good (Java packages) and high **Cohesion** good.
- **Information Hiding** is an encapsulating the capabilities of the module begidn the abstract interface.
- **Abstraction** & **Refinement** is *Declarative, Aggregation, Generalization, Parameterization, and Non-determinism.*
- **Aesthetics** includes *completeness, consistency, and conceptual integrity.*
- **Design Philosophy** includes *anlysis, models, user-centered design, IDEs, tools, language and games*

## P2L1 Review of UML

- **Diagram** is a simplified drawing showing the appearance, structure, or workings of something; aschematic representation.
- **Object Management Technique (OMT)** includes Class MOdel Diagram, Statechart Diagram, and Dataflow Diagram.
- **Unified Modeling Language (UML)**  is a general-purpose, developmental, modeling language in the field of software engineering, that is intended to provide a standard way to visualize the design of a system.

![alt text](/images/cs6310-diagrams-as-class-model-dagram.png "UML Diagrams as Class Model diagram")

**Diagrams**

- **Structural** diagrams give you the pieces of the system that are always there and the relationship among them.
    - **Class Diagram** - components and structurak properties).
    - **Object Diagram** - statis structure at a particular time.
    - **Composite Structure** - internal structure and possible interactions.
    - **Component Diagram** - organization of physical software components.
    - **Deployment Diagram** - components and structural properties.
    - **Package Diagram** - logical grouping and dependencies
    - **Profile Diagram** - extension to the UML meta model.
- **Behavior** diagrams are concerned with the execution(s) of the system.
    - **Use Case Diagram** - system functionality provided to external actors.
    - **State Diagram** -  dynamic behavior in response to stimuli.
    - **Activity Diagram** flow of control from activity to activity.
    - **Interaction Overview Diagram** synthesis of lower-level Activity Diagrams.
    - **Sequence Diagram** interaction of classes of message exchange.
    - **Communication Diagram** (Communication Diagram) object interaction of numbered messages.
    - **Timing Diagram** - rotated sequence diagram.
 
**Class Diagram**
![alt text](/images/cs6310-uml-classes-&-relationships.png "UML Classes & Realtionships")

**Features**

- **Object Constraint Language** (OCL) is a textual extension to UML's visual notation. Applicable to Class and Statechart diagrams. Enables more prcise specifications.
- **Meta Model** is the definition of UML in UML. UML Meta model is UML description of the UML language. It's can be extended by a modeler using profiles. Those extensions are more stereotypes, more tag values and constraints.

## P2L2 Object Oriented Analysis Exercise

    "The process of understanding a problem is called Analysis" - Prof. Spencer Rugaber
    
**Object Oriented Analysis** (OOA) is a requirments analysis technique developed by Abbott and Booch in the 1980s. Its's based on modeling real-world objects based on their descriptions to produce Object Analysis Model. It's pays primary attention to objects.

    Quote: "Objects are moste stable then functions, over the lifetime of a system"

    OOA Steps:
        1. Locate Nouns (Classes)
        2. Candidate Classes (basen on Noun list)
        3. Locate Adjective (Attributes)
        4. Locate Operations (Action verbs)
        5. Identify Relationships
            - Generalizations (... is generalization of ...)
            - Aggregations (... consists of ...)
            - Associations (... is associated with ...)
            - General(NO LINE)
   
                                                 OOA start with
                                                        |
                                    Textual Description (Requirement document)
                                      |           |           |            |
                                     Nons         |       Adjectives       |
                                   (Classes)      |      (Attributes)      |
                                             Action verbs            Stative verbs
                                             (Operations)           (Relationships)
      
    Kinds of verbs:
        - Operations correspands to action verbs
        - Linking verbs are related to attributes
        - Stative verbs are indicative of a relationship among objects

**Relationships**

![alt text](/images/cs6310-relationships.png "Relationships")

## P2L3 UML Class Models

- The **Class Model Diagram** is the most popular and  most complex type of diagram.
- It's contains representations for *classes, interfaces, objects, relationshis, etc*.

**Compartments**

- **Name Compartment** 
    - Name should me a nown. 
    - It be an *Abstact Class* 
    - Affordances: stereotypes.
- **Attributes Compartment**
    - Symbols for Visibility: `+` Public, `-` Private, `#` Proptected, `~` Package.
    - Must be name, type, optional multiplicity and ordering, optinal initial value, optional derivation, properties.
    - Additional properteis: `{frozen}`
- **Operations Compartment**
    - Optinoal visibility: `+` Public, `-` Private, `#` Proptected, `~` Package.
    - Parameters List: name, type, default value, kind(in, out, inout)
    - Additional properties: `{query}`, `{concurency}`, `{abstract}`, and Class scope

**Avanced Features**

- **Interfaces** Icons for requires and provides.
- **Parameterized classes** Describe collection classes.
- **Nested classes** Suitable for inner classes.
- **Composite objects** Class diagrams within class rectangles.

**Relationships**

- **Association** Example: people drive vehicles.
    - Roles: Name, association classes, aggregation or composition.
    - It can have qualifiers and links.
    - It can express Navigability, multiplicity, and constraints.
- **Generalizartion** Example: that car is kind of vehicle.
    - Instances of the subclass must have all properties of instances of the parent class 
    - Supports both multiple parent classes for a given class, and multiple child classes for a given parent class.
- **Dependencies** Example: cars and pollution laws.

## P2L4 Design Studies

    "Design is all about making desicions" - Prof. Spencer Rugaber
    
- **Design Studies** is series of scale models. It's a rigorous and systematic evaluation of the factors that influence a design. It should begin with determination of relevat criteria, metrics, & threshold. Design must be learned.
    - **Design Spaces** It's help to explore a space of possibilities.
    - **Projects** Each of the project involes solving a design problem in several ways.
    - **Experiments** Design study is an empirical scientific experiment.
    
**Report** 

The design study itself is presnted in a report. It's contain several sections.

1. **Context** It's provides background and motivation for the study.
2. **Research Questions** Design study examines the tradeoffs between various nonfunctional requirments.
3. **Subject** A design study compares multiple subjects.
4. **Exxperimentals Conditions** A software design study noramlly means running several versions of a program.
5. **Variables** They must be identified and appropriate metrics specified.
6. **Method** It's include number of trials, tools, technique, etc. 
7. **Results** The point of cunducting a design study is to produce data
8. **Discussion** It's opportunity to interpret the data and provide a discussion of its implications.
9. **Conclusions** It's a place to summarize reults and draw conclusions.

![alt text](/images/cs6310-design-study-summary.png "Design Study Summary")

**Deliverables**

1. **Source Code** solving a specific problem in several ways.
2. **Project report** containing project-specific content.
3. **Design Study** 

## P2L6 Formal Specification Exercise

- **Specification** need to know what a program is supposed to do before you begin to write in.
- **Notations**
    - **Mathematical logic** or **First Order Logic (FOL)** Enables to precisely express propositions, combonie them, and quality them.
    - **Object Constraint Language (OCL)** which is part of UML. It's provides a syntax for FOL that can be used to annotate UML diagrams.
- **Sorting** 

**What to consider?**

        Exercise: y equals the sort(ascending order) of x
        
- **Input Type** Did specification state what the input looked like?
- **Output Type** Did specification state what the output looked like?
- **Ordering** Did specification indicate any order?
- **Sensitivity to Input** Like size of x == y

Process of conversion from **Specification** to **Mathematical Specification**

- **Signature** Gives the name of the program, the name and types of the input arguments and the name and type of the results.
    - For sort it'a looks like this: `Vector<int> Y = SORT(Vector<int> X)`
- **Preondition** What must be true about the input used by a function.
- **Postcondition** What must be true about the output produced by a function.

## P2L7 OCL

- **Object Constraint Language (OCL)** (constraints, navigation, collections).    
    - Official part of UML
    - Strongly typed, declarative specification of system properties.
    - It's consist **constraints** + collection classes + UML diagram navigation.
    - It's **Declarative** not **procedural**.
    - It's pure expressnion language.
- Why do we need OCL?
    - UML diagrams are limited in what they can express.
    - Structural relationships, behavioral descriptions.
    - Mechanism for specifying precise semantics.
    - OCL extends UML with:
        - Class invariants
        - Operation pre and post condidtions
        - Guards on state machine transitions

**Syntax**

    context <identifier> <constraintType>: <Boolean expression>

    context              - The context is where you are in a diagram. Usually it a name of the class.
    <identifier>         - Give a name for the context. Context is where you are in a diagram.
    <constraintType>     - Type of constraints
    <Boolean expression> - It's an actual constraint that the statement is expressing.

**Invariants**

        context LargeCompany int: numberOfEmployees > 50

- Statement of a property that is always true
- Express key system requirements
- `inv` keyword
- Role of Invariants (aka concept of integrity constraints)

**Pre and Post Condidtions**

    context Real::squareRoot() : Real
    pre: self >= 0
    post: self = result * result
    
    contect Account::deposit(Real : amount)
    pre: amount > 0
    post: balance = balance@pre + amount

- Used to express Meaning of UML Operations
- `pre` condidtion what must be true for the operation to meaningfully take place.
- `post` condidtion waht is guaranteed to be true after the operation completes.

**OCL Keywords**

![alt text](/images/omscs6310-ocl-keywords.png "OCL Keywords")

**OCL Build-in Primitive Types**

![alt text](/images/omscs6310-ocl-build-in-primitive-types.png "OCl Build-in Primitive types")

## P2L9 Behavior Modeling

- **Structural Models** Express properties that are always true.
- **States** Abstract description of system values at a given time.
- **Events** Single, instantaneous, noticeable occurance
- **State Charts** (Developed by David Harel)
    - Address the issue of complexity
    - Part of UML
    - Extensions To FSMs
        - Depth (Nesting)
        - **Concurrency** Separate dash line
        - Broadcast Event
        - Conditional transitions
        - Entry/exit actions/activities
        - History
        - Default States

## P3L2 Overview of Artchitectural Styles

**Software architecture** refers to the fundamental structures of a **software system**, the discipline of creating such structures, and the documentation of these structures. These structures are needed to reason about the **software system**.  - *It's all about dicisions*.

- "Organization of a system into **component subsystems of modules**" - Informal Definition
- **Iteratively refined** into multiple layers
- Often makes use of **stereotypical architectural styles**

A **software architect** is a software expert who makes high-level design choices and dictates technical standards, including software coding standards, tools, and platforms. The leading expert is referred to as the chief architect.

**Ultimate GOAL** is to **Increase the quality** of delivired systems and **reduce the cost** of producing them. The way of doing that is the early detection of problems. And the key way of detecting things early is to layout in advance how the system will look like.

**Representing Architectures**

- **Component** is a computational or data element plus interface to the rest of the system
    - Selecting Components
        - Required functionality
        - Exisiting reusable componenets
        - Physical machine arthitecture
        - Expertise of staff
        - Projected evolution trajectories
    - APIs (Application Programming Interface)
        - Names if access ports, argumnets, types
        - Can be described in a programmming language; language binding
        - Might be described in OCL
        - To describe API - ADLs (Architectural Description Languages)
- **Connector** is a communication protocol or between components
    - Examples
        - Procedure call/return
        - Pair of messages
        - Asymmetric, synchronous
- **Configuration** is a specific associations between components and connector

**Architecture Styles**

**Architectural Styles** is a named collection of architectural desgin decisions.

- Standard
    - Abstract data types (ADT, hide representation)
    - Batch sequential (validate, edit, update cycle)
    - Blackboard (repository, opportunistic control, cooperating agents)
    - Big ball of mud (Monolithic)
    - Client Server (transactional processing, multi-tiers)
    - Component-based (reusable modules communicating through well-defined interfaces)
    - Coroutines(symmetric, interaction)
    - Data centric (use of stored database procedure)
    - Domain Driven Design (DDD) (business-oriented, domain model)
    - Implicit invocation (events, callbacks, registration-broadcast)
    - **Layered** (virtual/abstract, machines, limited visibility)
    - Master control (hierachical call and return)
    - Message Bus (asynchronous message passing a common bus)
    - Mobile code (code on demand, remote evaluation, mobile agent)
    - Object-oriented (asynchronous message passing, independent threads of control)
    - Peer-to-peer (equal partners sharing responsibility)
    - Plugins (registry plus third-party add-ons)
    - Pipe and filter (one-way, sequential, stdin-stout, ASCII streams)
    - Process control (with feedback loop)
    - Production systems (rule base, conditional firing)
    - **Representational state transfer (REST)** (client-server, layered, stateless, cacheable, distributed hypermedia)
    - **Service-Oriented (SOA)** (loosely coyupled, stateless, discoverable, contract-specified)
    - Shared Nothing (Shared) (distributed database with no sharing across nodes)
    - State-transition systems (reactive, real-time)
    - Shared-memory (with locks for synchronization)
    - Table-driven interpreter (parse and dispach)
- Specific
    - If system have more than one style it's **Heterogeneous**
    - **Domain-specific software architecture (DSSA)** (reference architecture) dublicate with some differences.
    - Can be named differently based on **semantics**

**ADL**

**Architectural Description Languages** is a notations for describing architectures. It's provide **formality** and **precision**. Examples are: [**Acme**](http://www.cs.cmu.edu/~acme/), Wright Rapide, ArTek, Demeter, CODE, Modechart, PSDL/CAPS, Resolve, UniCon

**Evaluations**

Architecture **Evaluations** is a process of estimation of correctness, completeness, consistency and other aspects of quality of architecture.

- **Systematic assessmnet** of architecture properties
- **Architecture review boards**
- **Software Architecture Assessment Method** (SAAM)
- **Architecture Tradeoff Analysis Method** (ATAM)

## P3L3 Artchitectural Views

    "An architecture is NOT a diagram . It is a set of decisions." - Prof. Spencer Rugaber

- Kruchten's Views
    - **Logical View** Structural breakdown of computational, communicational and behavioral responsibilities.
    - **Developmental View** Units of source code: packages, classes, libraries. Diagrmas: UML Package, Diagram, CVS.
    - **Proces View** Processes and threads into which execution is divided. UML Deploymnet Diagram.
    - **Physical View** Machines used for system  execution and how processes are allocated to them. UML Deployment diagram.
    - **Use Case View** Important execution sequences from the external actors' of view. UML Use Case Diagram.
- Non-Kruchten's Views
    - **Feature View** Conceptual units from the user's point of view. Feature diagram.
    - **Nonn-Functional View** How non-functional requirements affetcs the software architecture. Explicit tradeoffs.

## P3L4 Text Browser Exercise

- **Summary of Process** To summarize the overall architectural design process looks like the following:
    - **Phase 0: Specify Properties**
        - Construct a context diagram.
        - Indicate external actors but only one activity, the system itself.
        - Indicate external stimili (events) that can effect the system.
        - Indicate how the system communicates its results back to the external actors(percepts).
        - Specify the behaviors of the system.
    - **Phase 1: Componetize**
        - Decompose the system into components.
        - Allocate responsibilities to them.
        - Handling of events.
        - Delivery of percepts.
        - Provision of the property guarantees.
    -  **Phase 2: Determine Architectural Style**
        - Determine how the cmponents will interact.
        - For layered architecture.
        - Assign the components to layers.
        - Determine the dependencies between the layers.
        - Update the guarantees.
        - Select an invariant maintenance strategy.
        - Assign responsibility for invariant maintenance.

## P3L5 Non-Functional Reqs & Arch Styles

- **Performance** 
    - Definition: Attribute of a computer system that characterizes the timeleness of the service delivired by the system. 
    - Measures: Response time, throughput, capacity, utilization.
    - Devices: Caching, Concurency, Memory management.
- **Maintainability**
    - Definition: Extent to which enhancements can be readily added to a system. Also called flexibility, etc.
    - Measures: Coupling, Cohesion.
    - Devices: Encapsulation, Published Interfaces, Subclassing, Indirection, and wrapping.
- **Reliabity**
    - Definition: Likehood of failure in a given time period; continuity of service.
    - Measures: Mean Time To Failure (MTTF).
    - Devices: Redundancy, fault tolerance, Recovery blocks.
- **Safety**
    - Definition: Extent to which system protects against injury, loss of file or property damage; absence of catastrophic consequences.
    - Measures: Interaction complexity, time coupling, fault-tree analysis.
    - Devices: Hardware interlocks, Fault containment.
- **Security**
    - Definition: Extent to which syste protects against unauthorized intrusion; cnfidentiality.
    - Measures: Levels (confidential, top secret); formal proof.
    - Devices: Authentication/authorization, Security kernels, Encryption, Auditing and logging, Access control.

Other: Resourse utilization, Precision, Usability, Availability, etc. 

    Each Architectural style have plusses and minuses. 

## P3L6 Connectors

**Connectors** is mediate interactions among omponents: that is, thay establish the rules that govern component interaction and specify any auxiliary mechanisms required.

- **Simple Connectors**
    - **Procedure Call Connectors** (to) - Remote procedure calls
    - **Event Connecors** (to)
    - **Data Access Connectors** (tx) - SQL
    - **Linkage Connectors** (f) - Shared library configuration
    - **Stream Connectors** (t) - Buffers
    - **Arbitrators Connectors** (fo) - Schedulers
    - **Adaptor Connectors** (x)
    - **Distributor Connectors** (f)
- **Composite Connectors**
    - Science data servers, a form of publish-subscribe middleware
        - Constituent connectors: event, data access, stream, distributor
        - Multiple procedures and consumers
        - Data transformation
        - Public or private access
    - FTP applications: Globus, bbFTP, GribFTP
        - Constituent connectors: Procedure call, data access, stream distributor
        - Hierachically or flatly name
        - Synchronous
        - Authentification
    - Clien0server based distribution connectors: HTTP/REST, SOAP, FTP
        - Constituent connectors: Procedure calls, data access, stream
        - Persistent and transient data
        - Naming registry

Notes: *Connector design, Validation Rules, Atomic Elements, Linux Case Study*.

## P3L7 Acme

- **ACME** is an extensible ADl developed at CMU and USC-ISI specifically designed to facilitate the interchanhe of architecture descriptions.
    - AcmeStudio - Graphical editor
    - AcmeLib - API
    - AcmeWeb - document genearator
- Features
    - defines a vocaburary for taking about architectures
    - extension mechanism enabling tool-specific sublanguages to be embedded.
    - features generics, families and types for defining architectural styles
- Vocaburary
    - Components
    - Connectors
    - **Ports** Component Interface 
    - **Roles** Connector Interface
    - System
    - **Representations**
        - Levels of abstactions
        - Each view is called representations
    - **Re-maps** Binding mechanism for vertical compostition
    
**Keywords** beyond *Vocaburary*

- **Decomposition** For software architectural descriptions there are two kinds of decompositions:
    - **Horisontal**
    - **Vertical**
- **Properties** Name-value pairs for export to external tools
    - Identifier
    - Name-value pairs
    - Values
- **Families** Means of defining architectural styles
- **Open semantic framework** Export format for use by automated resoners

## P3L8 Refinement

- **Complexity** & **Abstraction** implies thinking at different levels 
- **Proper Refinements** 
    - **Property 1** Holds for any program that we want to implement (Solve the problem)
    - **Property 2** Each level in a design must be internally consistent (Test the program)
    - **Property 3** Each lowel level in a refinement must faithfully represent the level above it
- **Criterion**    
    - Abequate Representation
    - Total Representation
    - Models

**Refinement guarantee**

- The top level specification matches the requirements document
- Operations at each level preserve invariants
- Each refinement is adequate
- Each refinement is total
- Concrete Operation preconditions and post conditions model their abstract counterparts 

## P3L9 Middleware

## Resources

- [Class Resources PAge](https://www.udacity.com/wiki/saad/resources)
- [Virtual Machine Setup](https://www.udacity.com/wiki/saad/vm-setup)
- [ArgoUML](http://argouml.tigris.org/)
- [OO Design Review Guidelines](https://s3.amazonaws.com/content.udacity-data.com/courses/gt-cs6310/notes/gt-sad-p1l3-design-validation.txt)
- [IEEE 1016 Working Group: Software Design Descriptions](http://www.iso-architecture.org/ieee-p1016/)
- [ACME](http://www.cs.cmu.edu/~acme/)
