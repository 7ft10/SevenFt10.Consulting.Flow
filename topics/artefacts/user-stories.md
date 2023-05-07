# User Stories

{% hint style="success" %}
_**We use this to** capture a user's want or need quickly and the benefit that they feel that implementing this will bring **so that we can** have a starting point for a conversation with the customer or Product Owner._&#x20;
{% endhint %}



<figure><img src="../../.gitbook/assets/image (32) (1).png" alt=""><figcaption></figcaption></figure>

## Template&#x20;

_As a \[type of user]_\
_I want \[some feature]_\
_so that \[some reason]_



## How to Guide

**Stories are..**

* A high-level placeholder for a conversation
* An atomic piece of business value
* A description of a desired outcome(s) of the system produced
* Ideally from a user’s perspective
* A planning and scheduling token
* When supported by conversation, acceptance criteria, and other supporting information, are a description of work to be built by the team

## Resources <a href="#howtoguide-writeastory-resources" id="howtoguide-writeastory-resources"></a>

* [Story Essentials](https://confluence.budgetdirect.com.au/download/attachments/350298983/story\_essentials\_quickref.pdf?version=1\&modificationDate=1624070152264\&api=v2)
* [Story Mapping](https://confluence.budgetdirect.com.au/download/attachments/350298983/story\_mapping.pdf?version=2\&modificationDate=1632630749951\&api=v2)

## Key Characteristics <a href="#howtoguide-writeastory-keycharacteristics" id="howtoguide-writeastory-keycharacteristics"></a>

When writing stories that are to be implemented by Scrum teams, consider whether the output produced is going to be software (implementing a new type of payment option, for instance) or a non-software system of some kind (for example, integration with a 3rd party SaaS application). Below are a general set of guidelines...

* Stories are written by someone who has **business context**
  * The BA along with the PO will work with business stakeholders in understanding and interpreting business requirements, to then create stories that capture the essence of the requirement(s) &#x20;
  * Scrum team should must also contribute to further development and evolution of the story
* Stories are **independent** of other stories, **small** enough to be coded and tested in one iteration
* Stories produce a **vertical slice** of working code
* Stories focus on the _**who** (role)_, _**what** (action)_ & _**why** (benefit)_
* Stories are **not prescriptive** (of the solution) or suggestive on _**how**_ the scrum team implements them

## Who should write User Stories? <a href="#howtoguide-writeastory-whoshouldwriteuserstories" id="howtoguide-writeastory-whoshouldwriteuserstories"></a>

Everyone! Everyone in the Scrum team should be able to / comfortable writing user stories. This does not mean everyone will stop developing / testing and focus on solely writing user stories.

Business analysts along with the Product Owner would work on creating user stories, being the most skilled people in Scrum teams to do that. BA's and PO's are usually ahead of the rest of the development team too - in their proximity to newly landing business priorities.

Being able to write user stories, though, is quite empowering, allowing the development team to think of features _NOT_ along technology layers - which is what naturally comes to a lot of development team members. This will also help identify use cases, dependencies etc. early on and encourage deep and meaningful conversations in the Scrum team.

Letting the teams write user stories will help bring alignment towards the business goals/objective to each and every member of the team and this motivates the team members as they are adding value to the organisation

## Common Techniques to Writing Good User Stories <a href="#howtoguide-writeastory-commontechniquestowritinggooduserstories" id="howtoguide-writeastory-commontechniquestowritinggooduserstories"></a>

Good user stories will have certain characteristics which will align with expectations set by one or more of the below techniques...

#### ROLE-ACTION-BENEFIT <a href="#howtoguide-writeastory-role-action-benefit" id="howtoguide-writeastory-role-action-benefit"></a>

This approach, also known as Role-Feature-Reason, Role-Goal-Benefit (RGB) looks at stories from the perspective of user roles.

> _As a \[type of user] I want \[some feature] so that \[some reason]._

Such short descriptions keeps the focus on _who_, _what_ and _why_. It's up to the development team to then determine how to implement the story.

**The Role (Who)**

The role describes _who_ will benefit from the feature. Identify the specific type of user that will benefit from the function.

**The Action (What)**

Briefly describe _what_ user functionality needs to be built.

**The Benefit (Why)**

Description of _why_ the feature is to be developed. Identifying and defining the why with clarity will...

1. Allow the PO to determine the true priority of the story
2. Help the scrum team understand the value of the feature that's to be built

#### INVEST <a href="#howtoguide-writeastory-invest" id="howtoguide-writeastory-invest"></a>

INVEST is an acronym that represents the following concepts that contributes to making high-quality user stories...

**Independent**

Stories can be developed easily if they are devoid of dependencies. Horizontally sliced stories - split across technology layers and built with key competencies of development team members in mind, are an anti-pattern. This is because even when such stories are _done_, they will not have delivered working software - due to dependencies on corresponding stories from other horizontals in the technology stack.

**Negotiable...and Negotiated**

A good story is negotiable and will capture the essence of the software function being built, not the details. The details will surface as the story evolves over discussions and elaboration amongst development team members.

**Valuable**

Story needs to represent value for the end user. The story on its own will represent value for the customer. The customer may be a member of the public who uses a certain feature; or it could be an internal customer who uses the same function and/or different functions.

**Estimable**

Good stories can be estimated with relative ease. To be able to estimate, development team should have understood the story. Being too big, having unknowns etc. prevents a development team from meaningfully estimating stories with a reasonable degree of certainty.

**Small**

The story should be small enough to be able to be completed in a short amount of time. This allows the team to continually make progress throughout the sprint, as well as receiving quick feedback.

**Testable**

Good stories can be tested on their own. They should have well defined acceptance criteria as well, but not to the point where the ACs are prescriptive. Good stories will validate end-user behaviour at a minimum, but development teams usually go beyond validation of _just_ end-user behaviour, and test contracts that are defined in each of the technology layers. Testing maybe done through a set of automated tests - unit, integration and acceptance tests.

#### 3 C's <a href="#howtoguide-writeastory-3cs" id="howtoguide-writeastory-3cs"></a>

Originating from XP, 3 C's talk to 3 critical aspects of user stories - Card, Conversation & Confirmation.

**Card**

High level user stories are written on index cards and may not have all the information related to the requirement (and this is OK). It's a token / nominal representation of the requirement. This is captured / identified through the customer - the PO in most scrum teams.

**Conversation**

The development team engages in a series of conversations with the customer to flesh out the story (on the index card from above) and it's requirements. This activity requires the development team to be having an open forum, where questions of all nature are encouraged. Such conversations, though largely verbal will lead the team to have a shared understanding of the story.

**Confirmation**

Development team will work towards an agreement on what to build. Identify and document this as a series of examples / scenarios - in the form of confirmation (acceptance) tests.

## Not everything is a story! <a href="#howtoguide-writeastory-noteverythingisastory" id="howtoguide-writeastory-noteverythingisastory"></a>

Not everything is a story and it's ok to have work items which do not follow the philosophies discussed above. Don’t try and fit these into the story format:

* Non-functional requirements, like performance
* System interface agreements
* Key milestones / dates
* Coding standards or system testing
* Technical debt or defects
* Retrospective action items
* Iteration or release definition of done tasks

## Notes <a href="#howtoguide-writeastory-notes" id="howtoguide-writeastory-notes"></a>

1. The technologies used in developing software at A\&G are primarily - RPG, Java, Angular and JSP. Including features developed in DISC, it's possible to vertically slice stories that fit INVEST criteria.
2. This is not an exhaustive list of techniques or approaches that can be taken when writing stories; however, this page and associated reading will give you a pretty good idea of how to go about writing good user stories.

## References <a href="#howtoguide-writeastory-originalreadings" id="howtoguide-writeastory-originalreadings"></a>

Role-Action-Benefit - [https://www.mountaingoatsoftware.com/blog/advantages-of-the-as-a-user-i-want-user-story-template](https://www.mountaingoatsoftware.com/blog/advantages-of-the-as-a-user-i-want-user-story-template)

The 3 C's - [https://ronjeffries.com/xprog/articles/expcardconversationconfirmation/](https://ronjeffries.com/xprog/articles/expcardconversationconfirmation/)

INVEST - [https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/](https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/)

[https://www.justinmind.com/blog/user-story-examples/](https://www.justinmind.com/blog/user-story-examples/)

[https://medium.com/tribalscale/writing-technical-user-stories-434bf96f1dd5](https://medium.com/tribalscale/writing-technical-user-stories-434bf96f1dd5)

[https://techbeacon.com/app-dev-testing/practical-guide-user-story-splitting-agile-teams](https://techbeacon.com/app-dev-testing/practical-guide-user-story-splitting-agile-teams)

[https://www.scaledagileframework.com/story](https://www.scaledagileframework.com/story/)
