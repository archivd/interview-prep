# LLD Topics

<details>
  <summary>Design Restful APIs</summary>
</details>

----

<details>
  <summary>Design Tables - SQL/NoSQL</summary>
</details>

----

<details>
  <summary>SOLID Principles</summary>

  - [Baeldung - SOLID Principles](https://www.baeldung.com/solid-principles)
  - [Baeldung - Liskov's Substitution Principle](https://www.baeldung.com/cs/liskov-substitution-principle)
  - [Thorben - stackify.com](https://stackify.com/solid-design-principles/)
  - [[PDF] Robert C. Martin - Design Principles and
Design Patterns](/resources/pdfs/Robert_Martin-Principles_and_Patterns.pdf)
  - [Robert C. Martin (Uncle Bob) - SOLID Principles](https://www.youtube.com/watch?v=TMuno5RZNeE)
  - [Youtube playlist](https://www.youtube.com/playlist?list=PL6n9fhu94yhXjG1w2blMXUzyDrZ_eyOme)
  - [[PDF] Software Design Patterns - Florian Rappl](https://github.com/sothers/Rep1/blob/master/Books/Design%2BOOPS/designpatterns.pdf)
  - SOLID is composed of:
    1. SRP (Single Responsibility Principle) - "A class should have only a single responsibility." - reduces complexity
    2. OCP (Open Closed Principle) - "Software entities... should be open for extension, but closed for modification." - open for extension (e.g., via inheritance) and closed for modification of original purpose
    3. LSP (Liskov Substitution Principle) - "Objects in a program should be replaceable with instances of their subtypes
without altering the correctness of that program."
    4. ISP (Interface Segregation Principle) - "Many client-specific interfaces are better than one general-purpose interface."
    5. DIP (Dependency Inversion Principle) - "Depend upon Abstractions. Do not depend upon concretions."
  - To put it into one sentence: Classes should be decoupled, reusable, closed
yet extendable and only responsible for a single task
</details>

----

<details>
  <summary>Design Patterns</summary>
  
  - [Youtube playlist](https://www.youtube.com/playlist?list=PLrhzvIcii6GNjpARdnO4ueTUAVR9eMBpc)
</details>

----

<details>
  <summary>Best coding practices</summary>
</details>


## LLD Important Topics

<details>
  <summary>Q1. What is Object-Oriented Design? Explain in detail.</summary>

----
Object-Oriented Design (OOD) is a method of designing software systems by modeling them as collections of interacting objects that encapsulate data and behavior[1][2].

### Core Concepts
- **Objects:** Instances of classes that hold data (attributes) and perform actions (methods).
- **Classes:** Blueprints for objects, defining attributes and behaviors.
- **Encapsulation:** Hiding internal state and exposing only necessary interfaces.
- **Inheritance:** Reusing and extending existing classes.
- **Polymorphism:** Different objects responding to the same message in different ways.
- **Abstraction:** Simplifying complex reality by modeling relevant details only.

### Design Approach
- Identify core entities and responsibilities.
- Define classes with clear interfaces.
- Establish relationships: associations, aggregations, compositions, inheritance.
- Focus on low coupling and high cohesion for maintainability.
- Use design principles and patterns for solving common design challenges.

### Benefits
- Modular, reusable, and easy to maintain.
- Provides a clear blueprint for implementation.
- Facilitates communication among stakeholders.

### Use in Software Development
- Design APIs, modules, and system architecture.
- Model real-world entities intuitively.
- Enable scalable and adaptable systems.

Sources  
[1] Object-Oriented Design Principles https://geeksforgeeks.org/object-oriented-design-principles/  
[2] Introduction to Object-Oriented Design https://www.tutorialspoint.com/object_oriented_analysis_design/index.htm  
</details>

----

<details>
  <summary>Q2. What are Design Patterns? Explain in detail.</summary>

----
Design Patterns are proven, reusable solutions to common software design problems that arise during object-oriented development[1][3].

### Purpose
- Promote code reuse and robustness.
- Improve communication among developers via common vocabulary.
- Influence system structure for flexibility and scalability.

### Types of Design Patterns
- **Creational Patterns:** Deal with object creation mechanisms.
  - Singleton, Factory Method, Abstract Factory, Builder, Prototype.
- **Structural Patterns:** Deal with object composition.
  - Adapter, Bridge, Composite, Decorator, Facade, Proxy.
- **Behavioral Patterns:** Deal with object interaction and responsibility.
  - Observer, Strategy, Command, State, Visitor, Chain of Responsibility.

### Example: Singleton Pattern
- Ensures a class has only one instance, providing a global access point.
- Used for configuration objects, database connections.

### Benefits
- Simplifies system architecture.
- Facilitates code maintainability and extension.
- Encapsulates best practices.

### Usage
- Select patterns based on design problem.
- Adapt the pattern to fit specific system requirements.

Sources  
[1] Design Patterns Explained https://refactoring.guru/design-patterns  
[2] Gang of Four Book https://en.wikipedia.org/wiki/Design_Patterns:_Elements_of_Reusable_Object-Oriented_Software  
[3] Pattern Use Cases https://sourcemaking.com/design_patterns  
</details>

----

<details>
  <summary>Q3. What are SOLID Principles? Explain in detail.</summary>

----
SOLID principles are a set of five design principles that promote maintainable, flexible, and scalable object-oriented systems[1][3].

### 1. Single Responsibility Principle (SRP)
- A class should have only one reason to change.
- Encapsulates a specific responsibility, improving modularity and testability.

### 2. Open/Closed Principle (OCP)
- Software entities (classes, modules) should be **open for extension** but **closed for modification**.
- Use abstraction to add new functionality without altering existing code.

### 3. Liskov Substitution Principle (LSP)
- Subtypes must be substitutable for their base types without altering correctness.
- Ensures derived classes extend base classes without changing behavior.

### 4. Interface Segregation Principle (ISP)
- Clients should not be forced to depend on interfaces they do not use.
- Promote specific, granular interfaces over large, general ones.

### 5. Dependency Inversion Principle (DIP)
- High-level modules should not depend on low-level modules; both should depend on abstractions.
- Abstractions should not depend on details, but details on abstractions.

### Benefits
- Increased code reusability and flexibility.
- Easier testing and maintenance.
- Clearer, more understandable system architecture.

### Example
- Use interfaces to decouple modules.
- Apply SRP to refactor large classes.

Sources  
[1] SOLID Principles Explained https://blog.codinghorror.com/s-o-l-i-d-the-first-5-principles-of-object-oriented-design/  
[2] Design Principles in OOP https://en.wikipedia.org/wiki/SOLID  
[3] SOLID Principles in Practice https://refactoring.guru/design-principles/solid  
</details>

----

<details>
  <summary>Q4. What is Domain-Driven Design? Explain in detail.</summary>

----
Domain-Driven Design (DDD) is an approach to software development that emphasizes modeling the core business domain and aligning the system architecture to the domain's complexity[1][3].

### Core Concepts
- **Domain:** The core area of the business or problem space.
- **Ubiquitous Language:** A common language shared by developers and domain experts.
- **Bounded Contexts:** Divisions within the system with clear boundaries, each having its own model and language.
- **Entities:** Objects with a unique identity that persists over time.
- **Value Objects:** Immutable objects defined by attributes.
- **Aggregates:** Cluster of associated objects treated as a unit of consistency.
- **Repositories:** Abstractions for retrieving and storing aggregates.

### Process
- Collaborate closely with domain experts.
- Identify core domain concepts and patterns.
- Use models that reflect real-world processes.
- Continuously evolve models to better fit business needs.

### Benefits
- Focused development on business value.
- Better communication via ubiquitous language.
- Modular architecture with clear boundaries.

### Use Case
- Complex systems such as ERP, CRM, or financial platforms.
- When domain complexity is high, and accurate modeling is critical.

Sources  
[1] Domain-Driven Design Overview https://domainlanguage.com/ddd/  
[2] Eric Evans Book https://www.camdencore.com/book/domain-driven-design/  
[3] DDD Patterns https://dddcommunity.org/  
</details>

----

<details>
  <summary>Q5. What are Class Diagrams? Explain in detail.</summary>

----
Class diagrams are a type of UML diagram that visualizes the static structure of a system by showing classes, their attributes, operations, and relationships[1][3].

### Core Elements
- **Classes:** Rectangles divided into three sections:
  - Name
  - Attributes (properties)
  - Methods (functions)
- **Relationships:**
  - **Association:** Link between classes.
  - **Inheritance (Generalization):** "is-a" relationship.
  - **Aggregation:** "whole-part" relationship with lifecycle independence.
  - **Composition:** Stronger "whole-part" with lifecycle dependency.
  - **Dependency:** Uses relationship.

### Usage
- Model system structure during design.
- Show inheritance hierarchies.
- Define interfaces and interactions.
- Document class responsibilities.

### Example
- A `Customer` class associated with `Order`.
- An `Employee` class inheriting from `Person`.

### Benefits
- Clarity in system architecture.
- Communication amongst teams.
- Basis for generating code or database schemas.

Sources  
[1] Class Diagrams Overview https://www.uml-diagrams.org/class-diagram.html  
[2] UML Class Diagram Guide https://www.tutorialspoint.com/uml/uml_class_diagram.htm  
[3] Modeling with UML https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-class-diagram/  
</details>

----

<details>
  <summary>Q6. What are Sequence Diagrams? Explain in detail.</summary>

----
Sequence diagrams are UML interaction diagrams illustrating how objects communicate with each other through sequential message exchanges to complete a specific use case or behavior[1][3].

### Core Elements
- **Objects/Lifelines:** Vertical dashed lines representing entities involved in the interaction.
- **Messages:** Horizontal arrows showing method calls, responses, or signals.
- **Activation Bars:** Thin rectangles indicating active processing on a lifeline.
- **Return Messages:** Dashed lines representing responses.

### Purpose
- Visualize the flow of logic in a system.
- Define object interactions over time.
- Clarify communication, protocols, and sequences.

### Usage
- Model scenarios like login, order processing.
- Document interactions across multiple layers.
- Identify potential concurrency issues or bottlenecks.

### Example
- User sends login request → Auth Service validates → Response sent back.

### Benefits
- Clear sequence of interactions.
- Better understanding of system behavior.
- Useful for designing message-driven or event-driven systems.

Sources  
[1] Sequence Diagrams Overview https://www.uml-diagrams.org/sequence-diagram.html  
[2] UML Sequence Diagram Guide https://www.tutorialspoint.com/uml/uml_sequence_diagram.htm  
[3] Sequence Diagram in Software Design https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-sequence-diagram/  
</details>

----

<details>
  <summary>Q7. What are Design Reviews? Explain in detail.</summary>

----
Design reviews are structured meetings where stakeholders evaluate a proposed or existing system design for quality, correctness, and alignment with requirements[1][3].

### Purpose
- Ensure the design meets functional and non-functional requirements.
- Identify potential flaws or improvements early.
- Promote shared understanding among team members.

### Types of Reviews
- **Peer Review:** Intra-team review to catch issues.
- **Formal Design Review:** Stakeholders and experts assess the design comprehensively.
- **Walkthroughs:** Developer-driven presentation for feedback.
- **Inspections:** Structured, defect-focused review process.

### Process
- Present design artifacts (diagrams, UML, documentation).
- Discuss design principles, trade-offs, and constraints.
- Collect feedback and document issues.
- Iterate and refine the design.

### Best Practices
- Define clear objectives and scope.
- Use checklists and standards.
- Encourage open, respectful feedback.
- Track action items and follow-up.

### Benefits
- Improves design quality.
- Reduces technical debt.
- Ensures stakeholder alignment.

Sources  
[1] Design Review Principles https://www.cse.msu.edu/~cse470/Projects/DesignReviews.pdf  
[2] Effective Design Reviews https://insights.sei.cmu.edu/software-engineering/2014/07/what-is-a-design-review.html  
[3] Software Design Process https://www.geeksforgeeks.org/software-design-review/  
</details>

----

<details>
  <summary>Q8. What is UML? Explain in detail.</summary>

----
UML (Unified Modeling Language) is a standardized visual language used to model, specify, design, and document software systems[1][3].

### Purpose
- Provide a common language for developers, architects, and stakeholders.
- Facilitate understanding of system structure and behavior.
- Support system documentation, analysis, and design.

### Types of UML Diagrams
- **Structural Diagrams:** Show static aspects.
  - Class Diagram
  - Object Diagram
  - Component Diagram
  - Deployment Diagram
  - Package Diagram
- **Behavioral Diagrams:** Describe dynamic aspects.
  - Use Case Diagram
  - Sequence Diagram
  - Collaboration Diagram
  - State Diagram
  - Activity Diagram.

### Features
- Standardized notation and semantics.
- Supports both detailed and high-level views.
- Extensible for domain-specific modeling.

### Usage
- Model system architecture.
- Visualize workflows and interactions.
- Generate code or documentation.

### Benefits
- Enhances communication.
- Reduces misunderstandings.
- Promotes reusable design artifacts.

Sources  
[1] UML Overview https://www.uml.org/  
[2] UML Diagrams Types https://www.visual-paradigm.com/guide/uml-unified-modeling-language/  
[3] UML Use Cases and Diagrams https://www.tutorialspoint.com/uml/uml_use_case_diagram.htm  
</details>
