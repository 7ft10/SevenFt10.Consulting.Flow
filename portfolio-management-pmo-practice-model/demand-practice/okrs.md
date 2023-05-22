# OKRs

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

## **OKRs at a Glance**

* Objectives are ambitious and may feel somewhat uncomfortable
* Key results are measurable and should be easy to grade with a number (Google uses a scale of 0 – 1.0) (100%? increments of 10 or 1 or 0.1? Why not 0-10)&#x20;
* OKRs are public so that everyone in the organization can see what others are working on
* The “sweet spot” for an OKR grade is 60% – 70%; if someone consistently fully attains their objectives, their OKRs aren’t ambitious enough, and they need to think bigger
* Low grades should be viewed as data to help refine the next OKRs
* OKRs are not synonymous with employee evaluations
* OKRs are not a shared to-do list

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (32) (2).png" alt=""><figcaption></figcaption></figure>

````python
```notebook-python
#@title OKRs
## !pip install diagrams &> /dev/null 
from diagrams import Cluster, Diagram
from diagrams.programming.flowchart import Document

with Diagram("OKRs", show=False) as diagram:

    with Cluster("Company"):
      company_obj = Document("Objective") 
      company_kr = Document("Key Result")
      company_group = [ company_obj, company_kr ]

      company_obj >> company_kr

    with Cluster("Division"):
      div_obj = Document("Objective") 
      div_kr = Document("Key Result")
      div_group = [ div_obj, div_kr ]

      div_obj >> div_kr

    with Cluster("Team"):
      obj = Document("Objective") 
      kr = Document("Key Result")      
      tm_group = [ obj, kr ]

    init = Document("Initiative")

    company_obj >> div_obj >> obj

    obj >> kr >> init

diagram
```
````

## Objectives

An Objective describes an outcome you’d like to achieve in the future. An Objective sets the direction — think of it like a destination on a map.&#x20;

An Objective answers the question: “Where do I want to go?”

To ensure they’re inspirational and can be understood by everyone, they shouldn’t be technical and shouldn’t contain a metric.

Objectives should be:

* **Ambitious** - More than just "business as usual" or incremental change, an objective describes an aspirational yet attainable transformation, growth, and improvement that significantly improves the current situation.&#x20;
  * For example, introduce disruptive innovations, establish differences between the company and competitors, or be recognized as an industry leader in a category.
* **Meaningful** - A top priority that advances the company's strategy and greater mission; provides direction to departments, teams, and individuals about where we are going and how we are getting there.
* **Inspirational** - By providing an aspirational yet meaningful target, empower teams to reprioritize work to focus on what makes the most progress against an objective; to accomplish this, the objective should also be easy to remember.
* **Align Teams & Individuals** - Need to be broad enough to be relevant to at least more than one department, team, or individual one level down, but also specific enough that the objective can be measurable by up to three key results; if associated Key Results are satisfied, Objective should be achieved.
  * For example, a product-related OKR at the CEO level, such as increasing users by 100%, would have the Product leader as responsible. Still, every other function would also need to contribute to achieving that KR.
* **Clear, Responsible Party** - While aspirational objectives will often require collaboration and teamwork, they should have one responsible person to ensure the completion of the objective.&#x20;
* **Focused** - A person or team should have no more than 3 Objectives in order to focus on only the highest priority items; this also provides clarity on **what we will not do** in order to remain focused.
* **Transparent** - Allow individuals, teams, and departments to see how their work contributes to the overall goals of the company. By sharing OKRs, individuals, teams, and departments are able to spell out their priorities and avoid having others disrupt focus with non-priority items.

Categorising the Objective will begin to shape the objective (See [#monitoring-and-grading](okrs.md#monitoring-and-grading "mention")). For example, Committed Goals do not need to be inspirational or ambitious; however, most of the other attributes are applicable.&#x20;

## Key Results

A Key Result is a measurable outcome required to achieve the Objective. They help you measure progress toward the Objective — like a signpost that shows how close you are to your destination.

Key Results answer the question: “How do I know if I’m getting there?”

Key Results encourage you to be ambitious yet realistic. And they must contain a start and target value.

A KR differs from a KPI as it can be measured in a number of ways; for example, “assess and document” can be with polls, NPS surveys, direct feedback, etc. If there is a simple, quantifiable measure of the KR, then it can also be a KPI.&#x20;

Key Results should be:

* **Incremental** - A Key Result should focus on a number of incremental or steps on the way to an outcome instead of just the outcome.&#x20;
* **Aspirational** - Ambitious but realistic stretch goals; if it feels uncomfortable, it's a good KR.
* **Linked** - Be aligned to an Objective and be relevant to teams one level down; this alignment also allows KRs to roll down to become objectives one level down easily.
  * KRs should not be too specific that the KR needs to be rolled more than one level down.
* **Clear, Responsible Party** - one single person or team responsible for Key Result.
* **Influenceable** - the Key Result owner (department, team, or individual) should be able to impact Key Result through the owner's actions.
  * **Example**: an individual KR to change company-wide net retention is too broad; there are too many other conflating factors for an individual to determine impact. However, net retention could be appropriate KR for an entire department.
* **Time Bound** - has a due date usually within the quarter.
* **Measurable** - As Key Results provide the milestones for how we’ll complete the objective, KR should be either a _qualitative_ (i.e. completed Y/N or a number of steps of the project completed) or _quantitative_ (increased a metric by x) measure that can prove we accomplished the Key Result. _Quantifying Key Results is strongly preferred._
* **Mutually Exclusive** - Measure one component of progress for an objective without overlapping with progress represented by other Key Results. Progress for one Key Result shouldn’t count towards another Key Result.
  * **Example**: A Key Result for a number of transactions and a Key Result for the average dollar amount of transactions are an example of mutually exclusive Key Results: one KR measures _volume_ while the other Key Result measures the _quality_ of volume. On the other hand, a Key Result for a total number of transactions and a Key Result for a number of transactions from North America is an example of an overlap: progress gets ‘double-counted’ for both Key Results.
* **Collectively Exhaustive** - Key Results should fully account for what’s required to achieve an objective. If all Key Results are achieved, then, by default, the Objective must also be achieved.
* **Few Words and Ubiquitous Language** -&#x20;

## Initiatives

Initiatives are all the projects and tasks that will help you achieve a Key Result. They set the overall direction and describe how you’ll reach your destination.&#x20;

Initiatives answer the question: “What will I do to get there?”

These are the actions. They need an owner (responsible). The accountable owner is the owner of the KR.&#x20;

## Monitoring & Grading

Each KR should be categorised in order to measure it against the best scale. Once the scale has been decided, then the starting point must be defined.&#x20;

### Committed Goal (Must hit 100%)

The business-as-usual target is one that you’d expect to hit 100%. Anything other than 100% would be considered a failure. Given what we went through earlier about goals being hard, these are the exception, not the rule.

<figure><img src="../../.gitbook/assets/image (31) (1).png" alt=""><figcaption></figcaption></figure>

Binary goal. Either it is done, or it is not.&#x20;

### Stretch Goal (70% to 100% is Success)

Part of the OKR planning process is to agree on what a hard stretch target would be.&#x20;

Hard goals are sometimes called stretch or committed goals as well. Achieving 100% of the target would be amazing, and 70% would be good.&#x20;

![](https://zokri.com/wp-content/uploads/2021/04/Hard-Stretch-Commitment-Goal-Default.png)

The engine room of OKR is conversation and debate around what your Objective should be, what you should measure, and what ‘good’ and ‘amazing’ would look like.

### BHAG (Some progress is Success)

It’s been shown that what is considered ‘visionary’ companies often also set highly aspirational, Big Hairy Audacious Goals (BHAG). They are set to inspire greatness, new ways of doing things, new approaches to problems and genuine innovation. You need to choose when and where to set them, obviously, but their value is clear. Calibrating the success of a BHAG is harder, but 30% to 100% for many would be seen as a great result.

![](https://zokri.com/wp-content/uploads/2021/04/Moonshot-BHAG-Aspirational-Goal.png)

## Reporting&#x20;

When reporting on OKRs during the quarter, there are a couple of elements to take note of:

### Progress and Difficulty

Together the % progress and the level of difficulty show how the goal is progressing. This is a key part of the reporting - a conversation!

### **Confidence**

Where progress looks backwards, confidence levels look forwards and benefit from what you know about the execution of the goal and the likelihood of making good progress going forward.

### Trends & Averaging

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

Averaging an OKR looks like this:

&#x20;    Key result #1: 0.5\
&#x20;    Key result #2: 0.7\
&#x20;    Key result #3: 0.3

&#x20;     **Objective: 1.5 ÷ 3 = 0.5**&#x20;
