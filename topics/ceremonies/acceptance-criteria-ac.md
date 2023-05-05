# Acceptance Criteria (AC)

{% hint style="success" %}
_**We use this to** .... **so that we can** ...._ &#x20;
{% endhint %}

These basically form the boundary or scope of your Story, if you will. Technically, anything that falls outside of the acceptance criteria is not to be built as part of the story.

ACs sometimes could have:

&#x20;\- Lo-Fi prototype (e.g. sketches, wireframes, etc.), Narrative, Context Diagram, Dependent Stories, Constraints.

And less often have:

&#x20;\- Technical Design, Data model, Consider points, Link to high-level scenarios, GUI design.

#### **The ABCs of Acceptance Criteria** <a href="#howtoguide-elicitationandelaboration-theabcsofacceptancecriteria" id="howtoguide-elicitationandelaboration-theabcsofacceptancecriteria"></a>

**Abstract**&#x20;

A test is readable as a document describing system behaviour. Amplify your test's essential elements, and bury its irrelevant details and clutter. **Anyone, including non-techies, should be able to follow the steps taken in the test and understand why it passes**.

**Bona fide**

To ensure continual customer trust, a test must always truly exercise a system **as close to production as possible**. Passing acceptance tests tells the customer that what they asked for is complete and working.

**Cohesive**

**A test expresses one goal** accomplished by interacting with the system. Don't prematurely optimize by combining multiple scenarios into a single test.

**Decoupled**

**Each test stands on its own,** not depending upon or being impacted by results of other tests. A failure caused by problems in another test can be difficult to decipher.

**Expressive**

A test is **comprehensible** as documentation, **not requiring research** to understand. Name it according to the goal it achieves. As with unit tests, refactor each test to improve the ability of a third party to understand its intent. You should always eliminate magic numbers, replacing them with constants as appropriate.

**Free of duplication**

**Eliminate duplication across tests** (and even within the same test) before it eliminates you! Duplication increases risk and cost, particularly when changes to frequently-copied behaviour ripple through dozens or more tests. Duplication also reduces the use of abstraction, making tests more dense and difficult to follow.

**Green**

Once a story is complete, its associated **ATs must always pass**. A failing AT should trigger a stop-the-line mentality. Don't allow your test suite to fall into disarray by allowing failures to be ignored

### **Types of Acceptance Criteria:** <a href="#howtoguide-elicitationandelaboration-typesofacceptancecriteria" id="howtoguide-elicitationandelaboration-typesofacceptancecriteria"></a>

#### **Gherkin Reference (Given When Then)** <a href="#howtoguide-elicitationandelaboration-gherkinreference-givenwhenthen" id="howtoguide-elicitationandelaboration-gherkinreference-givenwhenthen"></a>

* Used when Behaviour/Scenario driven

**Format**

Scenario: \<Name for the behaviour that will be described>

Given \<Beginning state of the scenario>

When \<Specific action the user makes>

Then \<Outcome of the action in "When">

And \<Used to continue any of the three previous statements>

E.g.

| User Story                                                                                                                                                                                                                                                                                                | Acceptance Criteria                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <p><strong>As a</strong> Motor claims consultant</p><p><strong>I want</strong> a TTD relating to fraud automatically generated against the claim lodged if claim could be fraudulent</p><p><strong>So that</strong> I know that the claim needs to undergo further investigation in relation to fraud</p> | <p><strong>AC01: When Motor claim is lodged via DISC and qualifies for fraud</strong></p><p>GIVEN a Motor claim is being lodged in DISC</p><p>WHEN the 'Auto Fraud Score’ switch is On</p><p>AND fraud score is >= 100</p><p>AND claim is submitted</p><p>THEN the Auto Fraud Score TTD will be generated</p><p><strong>AC02: When Motor claim is lodged via DISC and does not qualifies for fraud</strong></p><p>GIVEN a Motor claim is being lodged in DISC</p><p>WHEN the 'Auto Fraud Score’ switch is On</p><p>AND fraud score is &#x3C;100</p><p>AND claim is submitted</p><p>THEN the Auto Fraud Score TTD will be NOT generated</p> |

#### **Rule Orientated** <a href="#howtoguide-elicitationandelaboration-ruleorientated" id="howtoguide-elicitationandelaboration-ruleorientated"></a>

* Used when we don't need details of test scenarios

**Format**

Simple bullet list

#### **Custom** <a href="#howtoguide-elicitationandelaboration-custom" id="howtoguide-elicitationandelaboration-custom"></a>

* Used when the above formats don't cut it, we make up what makes sense and would be clear and useful for developers and testers

**Format**

E.g. Truth tables, wireframes, flow charts, etc.
