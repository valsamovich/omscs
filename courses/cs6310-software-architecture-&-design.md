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

## Resources

- [Class Resources PAge](https://www.udacity.com/wiki/saad/resources)
- [Virtual Machine Setup](https://www.udacity.com/wiki/saad/vm-setup)
- [ArgoUML](http://argouml.tigris.org/)
- [Eclipse IDE](https://www.eclipse.org/home/index.php)
- [OO Design Review Guidelines](https://s3.amazonaws.com/content.udacity-data.com/courses/gt-cs6310/notes/gt-sad-p1l3-design-validation.txt)
- [IEEE 1016 Working Group: Software Design Descriptions](http://www.iso-architecture.org/ieee-p1016/)
