# Software Architecture & Design

    "Design creates culture. Culture shapes values. Values determine the future." - Robert L. Peters

- [P1L1 Introduction](/courses/cs6310-software-architecture-&-design.md#p1l1-introduction)
- [P1L2 Text Browser Exercise](/courses/cs6310-software-architecture-&-design.md#p1l2-text-browser-exercise)
- [P1L3 Design Concepts](/courses/cs6310-software-architecture-&-design.md#p1l3-design-concepts)
- [P2L1 Review of UML](/courses/cs6310-software-architecture-&-design.md#p2l1-review-of-uml)
- [P2L2 Object Oriented Analysis Exercise](/courses/cs6310-software-architecture-&-design.md#p2l2-bbject-oriented-analysis-exercise)
- [P2L3 UML Class Models](/courses/cs6310-software-architecture-&-design.md#p2l3-uml-class-models)
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

                                                 OOA start with
                                                        |
                                    Textual Description (Requirement document)
                                      |           |           |            |
                                Nons(Classes)     | Adjectives(Attributes) |
                                                  |                        |
                                         Actions(Operations)   Stative verbs(Relationships)




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

## Resources

- [Class Resources PAge](https://www.udacity.com/wiki/saad/resources)
- [Virtual Machine Setup](https://www.udacity.com/wiki/saad/vm-setup)
- [ArgoUML](http://argouml.tigris.org/)
- [Eclipse IDE](https://www.eclipse.org/home/index.php)
- [OO Design Review Guidelines](https://s3.amazonaws.com/content.udacity-data.com/courses/gt-cs6310/notes/gt-sad-p1l3-design-validation.txt)
- [IEEE 1016 Working Group: Software Design Descriptions](http://www.iso-architecture.org/ieee-p1016/)
