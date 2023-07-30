# Software Architecture


**Definitions of Software Architecture**

There are various (correct) definitions of software architecture.

- *ISO/IEC/IEEE 42010 definition of “architecture”*: Fundamental concepts or properties of a system in its environment embodied in its elements, relationships, and in the principles of its design and evolution.
- *IEEE 1471 definition of “software architecture”*: The fundamental organization of a system embodied in its components, their relationships to each
other, and to the environment, and the principles guiding its design and evolution.
- *SEI / [Bass+2012] definition of “software architecture”*: The software architecture of a system is a set of structures needed to reason about the system which comprise software elements, relations among them and the properties of both.     

What do some of the terms mean:

- _Component_: Building block of system.
- _Structure_: A collection of related elements that do a common task together.
- _Relationships/dependencies_: The coupling of elements allowing them to cooperate or exchange data.
- _Architecture decision_: A decision that helps in the evolution of an architecture.
- _Cross-cutting concerns_: Rules valid at several locations or points throughout the system and its development.
- _Decomposition of larger things into smaller things_: If a problem is too large to handle all at once, break it down into more manageable units.  


**Goals and benefits of Software Architecture**

Following are the main goals and/or benefits that a software architect should target.

- Support the design, implementation, maintenance and operations of systems.
- Achieve quality requirements such as reliability, maintainability, changeability, security etc.
- Achieve functional requirements.
- Ensure system structure is understood by all relevant stake holders.
- Systematically reduce complexity.
- Specify architecturally relevant guidelines for implementation and operation.

Essentially, what is software architecture good for.

- How can a software architect achieve **quality** goal? By taking _global_ design decisions which spans several components or parts of the system.

- A software architect normally do not predefine or prescribe every little detail of every component or technical concept, but rather focus on important elements of the system.

- What is **conceptual integrity** and why is it important for a software architect to achieve? _Conceptual integrity_ means the design/architecture of a system follows a consistent set of rules or decisions (e.g. in UNIX mostly everything is a file, or in LISP everything is a list).     

Conceptual integrity (or  consistency) is a necessary prerequisite for _understandability_ and _maintainability_ and it is a substitute or synonym for _appropriate standardization_.


**Software architecture in the software life cycle**

- Determine the affects of changes in functional requirement, quality requirement, technologies or system requirement in relation to software architecture.  
- Make know the affects between IT-systems and the supported business and operational processes.

- _The software lifecycle_
The software life cycle describes all phases of a software product, starting with its planning, through its development and use, and ultimately its retirement.



 


References:
- [1](Post the link here): Post the description of the link here
