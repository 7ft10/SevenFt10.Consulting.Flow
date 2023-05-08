# Intro to Architecture

When you create a software solution, its architecture must do two things:

* Provide an easy way to communicate with stakeholders
* Enable the team to see different levels of granularity

## Abstractions

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
