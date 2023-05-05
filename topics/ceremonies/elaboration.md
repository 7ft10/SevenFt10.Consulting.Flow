# Elaboration

{% hint style="success" %}
_**We use this to** .... **so that we can** ...._ &#x20;
{% endhint %}

### **Purpose** <a href="#howtoguide-elicitationandelaboration-purpose" id="howtoguide-elicitationandelaboration-purpose"></a>

Whole team to have an aligned understanding and intent behind each feature/function (broken up into Stories) that is to be implemented.  Fundamentally create a shared understanding of each Story across the team in order to draw on the collective mindset, transfer knowledge across the team.

### **Planning for Elaboration** <a href="#howtoguide-elicitationandelaboration-planningforelaboration" id="howtoguide-elicitationandelaboration-planningforelaboration"></a>

* PO/BA have their backlog groomed, prioritised
* PO/BA have identified the Stories that the team will be working on the next sprint
  * Have clear understanding of the business's need for these stories
  * Stories ought to be high level
    * Acceptance Criteria/Notes written out to aid the discussion
    * Acceptance Criteria/Notes to help set the boundary of story
    * Acceptance Criteria/Notes to aid with aspects the story to cover
* Stories brought into elaboration are big-ish, to be broken down by team (vertical slice)
* Let team know in advance of the stories the team will be elaborating on in the next session. &#x20;
  * Gives team a chance to understand/investigate before elaboration, resulting in a more useful session

Note: Acceptance Criteria will essentially be written/contributed by the whole team after the team has broken down the stories.

### **Running Elaboration session** <a href="#howtoguide-elicitationandelaboration-runningelaborationsession" id="howtoguide-elicitationandelaboration-runningelaborationsession"></a>

* New project/Epic
  * Explain what the new project and Epic is about
    * confirm the scope with the team
    * business problem that we are trying to solve
    * reasons
* For a new Project\

  * Go over the Story map;
* For a new Epic,&#x20;
  * Go over the high level Story breakdown
* Start with the highest priority Story
  1. PO/BA will talk to the story to the team&#x20;
     * Business requirement/need the story is address
     * Go over wireframes, flowcharts, system flow, etc. to help explain the business need
     * Make sure the delivery team understands the issue
       * Get team to confirm their understanding
  2. Team to discuss solution
  3. Team to breakdown story
     * And subtasks where needed
  4. Team to contribute to Acceptance Criteria
  5. If team is ready, then proceed to estimate the stories in the same session

### **Approaches to elaboration** <a href="#howtoguide-elicitationandelaboration-approachestoelaboration" id="howtoguide-elicitationandelaboration-approachestoelaboration"></a>

#### **Prototyping/Code and See** <a href="#howtoguide-elicitationandelaboration-prototyping-codeandsee" id="howtoguide-elicitationandelaboration-prototyping-codeandsee"></a>

* Present the business's need to the team (Dev/Test/PO/BA); at minimum the 3 Amigos (BA/DEV/Test)
* Team can decide to put something together quickly for a quick feedback
* Be mindful of scope creep
* Effective when
  * Stakeholders are available anytime for feedback, usually it'd be frequent
  * Developers are in direct contact with product decision makers
  * Non hierarchical culture, i.e. everyone is equal
  * Great for UI related work, much less rework and feasibility quite quickly determined too.

#### **Decomposition of Story** <a href="#howtoguide-elicitationandelaboration-decompositionofstory" id="howtoguide-elicitationandelaboration-decompositionofstory"></a>

* Common practice; Writing User stories with Acceptance Criteria (AC)
  * Discussion of context and purpose with the team for a collective understanding of the real needs
    * Encourage team challenging the needs
  * Think about outcomes before writing code
  * Be mindful of scope creep
* User Stories
  * Include context/Intent
  * Include Acceptance Criteria
  * Include Other useful info
    * Wireframes/Sketches
    * Link to similar stories
    * Link to information on AS-IS, if relevant
    * Affected business rules, if applicable
    * Style guide
    * Associated stories
    * Links to dependencies
    * Flow chart
    * Data model
  * Should
    * Use **clear**, **simple**, and concise language.
    * Use **commonly** understood **terminology**.
    * Explicitly state the need.
    * Have only **one interpretation.**
    * Use direct, active statements.
    * Express only **one idea** per statement.
    * Articulate a unique point (is not redundant).
    * Maintain consistently across the story/AC.
    * Have a means of verification. (testing/AC)
    * **Specify a need and not design.**
  * Avoid
    * Implementation details.
    * Multiple directives or functions.
    * Negative specification/outlining what it shouldn’t do.
    * Subjective, vague, or undefined descriptors. (Fast, flexible, user-friendly.)
    * **Ambiguities such as “as appropriate” or “if needed.”**
    * Speculation. Users may want. Probably should. **No wishy-washy statements!**
    * **Asking for the impossible**. (Asking for it to be 100% reliable is as realistic as saying it will satisfy all users.)
  * Stories should be business needs/requirement.  They should NOT be design/solution (most of the time).
    * The delivery team as a whole should come up with a solution during elaboration
    * Whole delivery team to contribute Story breakdown and Acceptance Criteria and other details&#x20;
      * PO/BA/SME/Dev/Test; at minimum the 3 Amigos (BA/Dev/Test)
      * Tasks
        * Not all work need to be broken down into User Stories
          * E.g. technical tasks like building framework&#x20;
        * Consider Triggers
        * Consider conditions
  * Bring bigger Story to team for elaboration session and work with team to break it down to smaller stories. Not the other way round
    * Encourage the team to **slice the story vertically** (**Video**: [Slicing Story](https://youtu.be/EDT0HMtDwYI))
    * Breaking story down to sub tasks (under Stories/Tasks), if necessary

## Using Models <a href="#howtoguide-elicitationandelaboration-usingmodels" id="howtoguide-elicitationandelaboration-usingmodels"></a>

It is possible to use stories with UML and similar modelling languages. It is also possible to create simple user interface sketches or even wire-frames as a way to elaborate the story.\
These models can then be used to generate acceptance tests or they can be used as the basis for development. Do not hesitate to use models where they are useful as long as they:

* are useful to the developer, rather than being more an obligation than a useful tool
* are consistent
* support, rather than replace conversations about development needs
* can be understood by business users, testers, developers and anyone expected to be relying on them.

## **EXAMPLE**

| Epic                                                                                                                                                   | Initial Story                                                                                                                                                                                                                   | Stories broken down by team                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Acceptance Criteria                                                                                                                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Epic                                                                                                                                                   | Initial Story                                                                                                                                                                                                                   | Stories broken down by team                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Acceptance Criteria                                                                                                                                                                                                                                                                                                      |
| <p>Notify client of claim lodgment</p><ul><li>Email</li><li>SMS (potentially separate Epic)</li><li>Social Media (potentially separate Epic)</li></ul> | <p><strong>Initial Story for Email Epic</strong></p><p>As a Claim Consultant</p><p>I want to easily send an email to client who has successfully lodged a claim</p><p>So that the client is assured of their claim lodgment</p> | <p><strong>Solution</strong>: Automatic sending of email to client after successfully submits a claim lodgment</p><p><strong>Story 1</strong>: <strong>Client Receiving email</strong></p><p>As a client</p><p>I want to receive an email with relevant details of my claim lodgment</p><p>So that I am assured that my claim lodgment status</p><p><strong>Story 2</strong>: <strong>Claim Consultant viewing email status</strong> </p><p>As a claim consultant</p><p>I want see on the claim that an acknowledgement email is sent</p><p>So that I know an email has been sent to the client</p><p><strong>Story 3</strong>: <strong>Creating claim lodgment email template</strong></p><p>As a system administrator</p><p>I want to create a template that I can use</p><p>So that I can set know the format and data I need to send out to the client</p><p><strong>Story/Task 4: Autocreation and sending of email</strong></p><p><strong>Sub Task 1</strong>: Building the trigger framework to auto send email</p><p><strong>Sub Task 2:</strong> Minimum email content</p><p><strong>Sub Task 3:</strong> Auto send email to client with correspondence email address</p> | <p>Acceptance Criteria for <strong>Story 1:</strong></p><p>AC01: When client successfully lodged claim</p><p>AC02: When claim lodgment platform crashes halfway through lodgment</p><p>AC03: System error when client was submitting claim</p><p>AC04: When client has not registered a correspondence email address</p> |

### **Inputs & Outputs**  <a href="#howtoguide-elicitationandelaboration-inputs-and-outputs" id="howtoguide-elicitationandelaboration-inputs-and-outputs"></a>

**Template:**

* Acceptance Criteria Reference
* Functional Decomposition
* Assumption
* Pre-conditions
* &#x20;“Item Under Test” (IUT): e.g. System, Component
* Inputs: e.g. Button press, Data
* Outputs: e.g. Report, Successful Transaction
* Test Type(s) – Re: Agile Quadrant
* Tools: e.g. Manual, MS Test, SoapUI

**Discuss**

Identify the “Item Under Test” (IUT) usually these are the nouns, and examples of correctness and incorrectness. For each decision or component consider the following:

* What is the input?
* Where does the input come from?
* What happens to the input?
* What is the output?
* Who is the customer of the output?
* What makes the output complete?
* What makes the output good?
* How much is good “enough”?
* What information is needed?
* What is the architecture?
* How can the information be gathered?
* When can we find the information?
* Who do we need to find the information?
* What is fed into the events/activities in the story?
* Where does the information/data come from?
* What happens within the story?
* What is passed onto the next step/stage from the story?
