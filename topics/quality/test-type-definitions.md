# Test Type Definitions

## Unit Test (UT)&#x20;

* Low-level, focusing on a small part of the software such as a Java class or Angular component together with associated collaborators
* Usually written by developers or perhaps software engineers in test, using their regular IDEs and testing frameworks such as IntelliJ, JUnit, VS Code and JEST
* Run faster than any other kind of test, allowing a suite of thousands of unit tests to be run in a few seconds
* Very scalable
* Automatable
* The primary facilitating mechanism for refactoring

## **Integration Test (INT)**

* Determine if independently developed units of software work correctly when they are connected to each other.
* Focusing on larger groups of collaborating Java classes or Angular components together with I/O dependencies such as databases or network connections.
* I/O dependencies should not made at the expense of execution speed - for example a fast running in memory or local docker database can be leveraged over a hosted development database or a Contract Test to mock out an API endpoint
* Usually written by developers or perhaps software engineers in test, using their regular IDEs and testing frameworks such as IntelliJ and junit or VS Code and jasmine.
* Run fast allowing a suite of hundreds or thousands (depending on I/O dependencies) of integration tests to be run in a few seconds
* Very scalable
* Primary facilitating mechanism for refactoring

## **Contract Test (CT)**

* Similar to an integration test used specifically for the purpose of ensuring that a pair of applications will work correctly together by checking each application in isolation to ensure the messages it sends or receives conform to a shared understanding that is documented in a "contract”.
* The network dependency is mocked by the contract broker so contract tests run fast
* Usually written by developers or perhaps software engineers in test, using their regular IDEs and testing frameworks such as IntelliJ and junit or VS Code and jasmine.
* Run fast allowing a suite of hundreds or thousands of contract tests to be run in a few seconds
* Very scalable
* Primary facilitating mechanism for refactoring interdependent services independently of one another

## **Exploratory Test**

* An exploratory test is one which emphasizes a rapid cycle of learning, test design, and test execution. Rather than trying to verify that the software conforms to a pre-written test script, an exploratory test explores the characteristics of the software, raising discoveries that will then be classified as reasonable behaviour or failures.

## **Acceptance Test (AT)**

* Testing based on story card acceptance criteria to enable the tester (manual) or developer (automated) to determine whether or not the software is ready for consumption by the customer.
* Scoped to a particular story only
* Performed from the customer perspective - usually a UI (eg browser or DISC terminal) or an API client (eg CTM integration)
* Maximum context and value with respect to customer requirement - significant determining factor in confidence of story definition of done
* Slower than integration test as a local service together with supporting out of process collaborating services are necessary to exercise the code
* As such, these tests are harder to maintain and scale

## **System Test (ST)**

* Similar to an Acceptance Test but instead requires live versions of one or many deployed services in hosted environments, requiring test environment and network access
* Teams currently need to wait overnight before test subject is deployed to NXI or NXQ
* Exercises code paths through one or many services and dependent services
* Usually written by developers or perhaps software engineers in test, using their regular IDEs and testing frameworks such as IntelliJ and junit or VS Code and jasmine.
* Run duration is an order of magnitude slower and largely determined by the scope of the execution path through the dependent services. A single system test could take between one and several seconds to run.

## End to End Test (E2E)

* Confirming that full user journey processes can be completed throughout the entire value stream. E.g Establish customer, Create/amend/service or renew a policy and lodge and process a claim
* Scoped to a customer value stream
* Performed from the customer perspective - usually a UI (eg browser or DISC terminal) or an API client (eg CTM integration)
* Maximum context and value with respect to customer requirement - significant determining factor in level of confidence of working software
* Very slow to run - depending on scope of test, execution duration can minutes to tens of minutes
* Hard to maintain
* Does not scale
* Depending on implementation, can be repurposed for load testing
* Automated or Manual

## Penetration Test (PEN)

* Authorised simulated cyber attack on a computer system, performed to evaluate the security of the system.
* Automated or Manual

## Synthetic Test (SYN)

* Method of understanding how our call centre agents and customers experience our applications by proactively testing public production environment endpoints and 3rd party APIs such as payment gateways.
* Automated

## References

* [https://martinfowler.com/bliki/UnitTest.html](https://martinfowler.com/bliki/UnitTest.html)
* [https://martinfowler.com/bliki/IntegrationTest.html](https://martinfowler.com/bliki/IntegrationTest.html)
* [https://pactflow.io/what-is-contract-testing-page/](https://pactflow.io/what-is-contract-testing-page/)
* [https://martinfowler.com/bliki/ExploratoryTesting.html](https://martinfowler.com/bliki/ExploratoryTesting.html)
