# Intro to Architecture

The architecture of a system describes its major components, their relationships (structures), and how they interact with each other. Software architecture and design includes several contributory factors such as Business strategy, quality attributes, human dynamics, design, and IT environment.

<figure><img src="https://www.tutorialspoint.com/software_architecture_design/images/software_architecture_types.jpg" alt=""><figcaption></figcaption></figure>

We can segregate Software Architecture and Design into two distinct phases: Software Architecture and Software Design. In Architecture, nonfunctional decisions are cast and separated by the functional requirements. In Design, functional requirements are accomplished.

<figure><img src="../../.gitbook/assets/image (7) (1) (2).png" alt=""><figcaption></figcaption></figure>

[https://www.future-processing.com/blog/what-is-software-architecture-in-software-engineering/](https://www.future-processing.com/blog/what-is-software-architecture-in-software-engineering/)

## Software Architecture

Architecture serves as a blueprint for a system. It provides an abstraction to manage the system's complexity and establish a communication and coordination mechanism among components.

* It defines a structured solution to meet all the technical and operational requirements while optimizing common quality attributes like performance and security.
* Further, it involves a set of significant decisions about the organization related to software development. Each of these decisions can have a considerable impact on the quality, maintainability, performance, and overall success of the final product. These decisions comprise of −
  * Selection of structural elements and their interfaces by which the system is composed.
  * Behaviour is specified in collaborations among those elements.
  * Composition of these structural and behavioural elements into large subsystems.
  * Architectural decisions align with business objectives.
  * Architectural styles guide the organization.

## Software Design

Software design provides a design plan that describes the elements of a system and how they fit and work together to fulfil the requirement of the system. The objectives of having a design plan are as follows −

* Negotiate system requirements and set expectations with customers, marketing, and management personnel.
* Act as a blueprint during the development process.
* Guide the implementation tasks, including detailed design, coding, integration, and testing.

It comes before the detailed design, coding, integration, and testing and after the domain analysis, requirements analysis, and risk analysis.

<figure><img src="https://www.tutorialspoint.com/software_architecture_design/images/software_design.jpg" alt=""><figcaption></figcaption></figure>

## Goals of Architecture

The primary goal of the architecture is to identify requirements that affect the structure of the application. A well-laid architecture reduces the business risks associated with building a technical solution and builds a bridge between business and technical requirements.

Some of the other goals are as follows −

* Expose the structure of the system, but hide its implementation details.
* Realize all the use cases and scenarios.
* Try to address the requirements of various stakeholders.
* Handle both functional and quality requirements.
* Reduce the goal of ownership and improve the organization’s market position.
* Improve the quality and functionality offered by the system.
* Improve external confidence in either the organization or the system.

### Limitations

Software architecture is still an emerging discipline within software engineering. It has the following limitations −

* Lack of tools and standardized ways to represent architecture.
* Lack of analysis methods to predict whether architecture will result in an implementation that meets the requirements.
* Lack of awareness of the importance of architectural design to software development.
* Lack of understanding of the role of software architect and poor communication among stakeholders.
* Lack of understanding of the design process, design experience and evaluation of design.

## Creating a Solution

When you create a software solution, its architecture must do two things:

* Provide an easy way to communicate with stakeholders
* Enable the team to see different levels of granularity

{% file src="../../.gitbook/assets/1-s2.0-S0164121212001264-main.pdf" %}

<figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (8) (1) (1).png" alt=""><figcaption></figcaption></figure>

Enterprise architecture is the process of translating the business vision and strategy into effective enterprise change by creating, communicating and improving the key principles, standards and models that describe the enterprise's strategic IT architecture.

Having a defined strategic IT architecture alone is not enough; if the principles and standards are not adhered to, then the value of the enterprise is compromised. This leads to the need for governance, compliance and enforcement, i.e. a mechanism and process is required by which the strategic IT architecture can be governed and maintained. Such a mechanism has been created through the Architecture Forum and supporting governance processes and artefacts.

In framing the approach for IT architecture governance, consideration was given to establishing a multi-tiered framework to separate strategic/enterprise concerns from tactical/solution-oriented interests, but a single architecture forum has been chosen due to the relatively small size of A\&G and the desire to avoid an overly complex governance framework.

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

The noteworthy characteristics of software architecture include the following:

* Uninterrupted Functionality: The software system should perform as intended without any bugs or interruptions.
* Reliability: The software system should perform optimally, irrespective of the environment and input number.
* Maintainability: Your team should be able to introduce innovative changes to the software without interrupting the existing system’s functionality.
* Security: The software should be secure from all external or internal attacks.
* Minimal Technical Debt: The source code should be clean and organized rather than messy or full of anti-patterns. This reduces the [code refactoring](https://www.netsolutions.com/insights/what-is-code-refactoring/) efforts and corresponding technical debt.
* Testability: You should seamlessly conduct [software testing](https://www.netsolutions.com/quality-assurance-testing) for faster bug identification, thus reducing the time to market.
* Modularity: You should be able to divide the software system into smaller, more manageable modules. It proves helpful when introducing microservices architecture when scaling up operations.

{% embed url="https://www.netsolutions.com/insights/why-software-architecture-matters-to-build-scalable-solutions/" %}

Here are the software architecture best practices that software architects must follow to design scalable, maintainable, and reliable software system that meets your organization’s needs:

* Be clear about the business requirements of the software system before you start working on its design. It would ensure that the software meets stakeholders’ business goals and is what you had expected.
* Keep your software architecture simple, as managing and scaling it will be easier over time. Steer clear of any complexity or layer that may complicate things later.
* Follow the modular design practice (breaking down an extensive system into small modules) while laying out the architecture of your software system. They’re easier to scale, maintain, and reuse.
* Use design patterns in your software architecture as they offer a standardized approach to solving problems, letting you easily maintain and scale the software system.
* While considering functional requirements is essential, you must also consider non-functional requirements like performance, security, and reliability. Addressing them early in the design process would ensure you meet all the requirements.
* Don’t overlook documentation can help you communicate design decisions to stakeholders and fix issues, ensuring that design designs are understandable and maintainable over time.
* Test the software architecture early and often to ensure the software meets both the functional and non-functional requirements.

<figure><img src="../../.gitbook/assets/image (8) (3).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (6) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Abstractions

Keeping architecture diagrams up to date is difficult. Creating them is just as difficult. Architects spend most of their time gathering the right icons, drawing lines in Miro or Viso, making sure that they are the right type etc. etc. etc. What a waste of time.

Instead, architects should be focused on ensuring that the current state is correct and that proposed changes to the enterprise ecosystem have taken into account all other systems that may be impacted.

Architecture diagrams as code (ADAC) is a way of allowing architects to focus on the right things and stop wasting time. It can also help other areas of the business by creating or leveraging a configuration management database (CMDB).

ADAC can also be extended to include the personas that interact with the systems. This is an important part of the impact analysis and can be the starting point for other agile techniques, such as epic and story writing.

In order to create these maps of your code, we first need a common set of abstractions to create a ubiquitous language that we can use to describe the static structure of a software system. A software system is made up of one or more containers (applications and data stores), each of which contains one or more components, which in turn are implemented by one or more code elements (classes, interfaces, objects, functions, etc.). And people may use the software systems that we build.

### Context

A software system is the highest level of abstraction and describes something that delivers value to its users, whether they are human or not. This includes the software system you are modelling and the other software systems upon which your software system depends (or vice versa). In many cases, a software system is "owned by" a single software development team.

A Context diagram shows the relationship between the system that you're building and other actors, including humans and non-human systems, such as external systems. This diagram is above the level of the microservices. You can use it to be aware of the potential external dependencies that you must manage.

### Container (applications and data stores)

In the C4 model, a container represents an application or a data store. A container is something that needs to be running in order for the overall software system to work. In real terms, a container is something like:

* Server-side web application
* Client-side web application
* Client-side desktop application
* Mobile app
* Server-side console application
* Serverless function
* Database
* Blob or content store
* File system
* Shell script

A container is essentially a context or boundary inside which some code is executed, or some data is stored. And each container is a separately deployable/runnable thing or runtime environment, typically (but not always) running in its own process space. Because of this, communication between containers typically takes the form of inter-process communication.

A Container diagram shows the containers that your final system is deployed into and their relationship to each other. If you’re following the "one container per microservice" rule, you can use this diagram to see all your microservices and the services that they depend on at a glance.

### Component

The word "component" is a hugely overloaded term in the software development industry, but in this context, a component is a grouping of related functionality encapsulated behind a well-defined interface. If you're using a language like Java or C#, the simplest way to think of a component is that it's a collection of implementation classes behind an interface. Aspects such as how those components are packaged (e.g. one component vs many components per JAR file, DLL, shared library, etc.) is a separate and orthogonal concerns.

An important point to note here is that all components inside a container typically execute in the same process space. In the C4 model, components are not separately deployable units.

A Component diagram, which isn't always needed but is useful, provides a view within a container and a view of the interacting components.

### Code

The final "diagram" is the code, which includes all your tests and the code that implements the microservices and other components. Write your code so that it's easy to understand. Strive to create self-documenting code.

### Supporting Abstractions

#### Persona

A persona represents one of the human users of your software system (e.g. actors, roles, persona, etc.).
