# Estimation Overview

{% hint style="success" %}
_**We use this to** properly plan, manage and understand the total efforts **so that we can** implement, test and deliver the desired product to the customers._
{% endhint %}

The two cornerstones of any piece of work are Planning and Estimation.&#x20;

In an agile project, estimation of the work/sizing of the work is done at various levels, with different stakeholders and using different techniques.

## Why Estimate?

1\. Improved Decision-Making\
With accurate, agile estimation, the development team will be able to conduct effective backlog grooming sessions, which will further help in precise sprint planning. When they make informed decisions and plan well, their user story delivery time will improve.

2\. Better Coordination\
Let’s say that the estimated effort for user story A is two weeks. On the other hand, the estimation effort for user story B is four weeks. Now, suppose both the user stories depend on each other and are connected. In that case, the team needs to prioritize work so that both user stories get completed simultaneously, thus leading to better coordination among teams.

3\. Better Risk Management\
Software projects often suffer from exceeding budgets and timelines. To lessen this risk, Agile project estimation is an ideal solution. Agile product estimation helps estimate story points and stick to budgets, estimates, and the project’s scope. The more accurate the estimates, the better the chances of on-time, quality delivery.

### **Project - Dream Home** <a href="#howtoguide-estimation-project-dreamhome" id="howtoguide-estimation-project-dreamhome"></a>

Let us try and understand the process of estimation with a sample project.

"Project - DREAM HOME"

When a major new idea is conceived, it is often a high-level “dream”. This idea needs to be broken down into epics, which are still at a very high level.

For instance, the big dream of a huge house may become epics like "CASTLE","VILLA","TOWNHOME". Neither of these ideas and epics should be estimated.

As time progresses with increasing level of granularity, themes develop around the Epics on the types of  houses followed by specific features. As we iterate the epics into themes and features, we  start working through the screening, decision and budget estimates iteratively.

So, the big house theme is broken down into duplex home, single level home etc. Since these are relatively better than the ideas and epics, the themes and features are estimated in T-Shirt sizes (Small, Medium, Large, X-Large) or Coffee-Cup sizes (Tall, Grande, Vente, Trenta).

These then get broken down further into user stories "Bedroom","Bathroom", "Backyard","alfresco" etc. The user story indicates the deliverable that needs to be built, and each story will have acceptance criteria which will have details or specifications of each room/area.

Like the project schedules in the project management framework, the deliverables are decomposed into the tasks or activities even in agile framework. User stories are estimated in story point, and the tasks are estimated in hours.

\
**Pre-requisites for estimation**

1. Prioritized backlog - Product Owner works closely with the BA's and the business to organize a prioritized backlog of user stories. Different forums like Refinement sessions are used to understand the requirements and prioritize them well.
2. User stories with acceptance criteria - Product Owner works with the BA's to create clear, precise and testable acceptance criteria along with the **TEAM**. Backlog grooming sessions are forums used to Groom the stories with the team
3. Understanding of estimation technique - Scrum Master works with the team to derive a common understanding of the estimation technique and the units of estimation

## **Techniques for estimation** <a href="#howtoguide-estimation-techniquesforestimation" id="howtoguide-estimation-techniquesforestimation"></a>

**Here are some very popularly used techniques for estimation, however there are different techniques that can be used based on the needs of the team**

1. Poker planning - is one of the most popular methods for story point estimation. This technique uses poker cards ( with fibonacci numbers) with numbers on it to estimate the relative size of stories&#x20;
   * There are a small number of items
   * Establishing mutual understanding among team members
   * Running late-stage estimations
   * The backlogs are highly prioritized
2. T-shirt sizing - is used when\

   * The team is new to Agile estimation
   * There are large backlogs
   * Running early-stage estimations
3.  Bucket system - This Agile estimation technique can be incorporated when estimating many items (50-500) and is better than planning poker. Here, different buckets (cards) are placed sequentially with values ranging from 0, 1, 2, 3, 4, 5, 8, 13, 20, 30, 50, 100, and 200 (and more, if required). Next, according to the estimators’ discretion, the user stories (items) are placed within the buckets.

    To start with, pick a random item and place it under a different bucket. Next, pick another user story, discuss all its features and requirements within the group, and place it in the bucket that suits the team’s understanding. Follow the same drill throughout.

    * Estimating a large number of items
    * Enabling quick estimations
    * The team is new to Agile estimation
    * Estimating long-term projects

**Poker planning resources**

**Not everything can be estimated..!**

There are scenarios where the team may not have all the details required to estimate or there may be uncertainties about technical implementation. In agile, the teams then use a time boxed activity called as a spike, to investigate further, gather more information about the user stories that they need to estimate.

These constructs are called as "SPIKE".&#x20;

## **Estimation Session**  <a href="#howtoguide-estimation-estimationsession" id="howtoguide-estimation-estimationsession"></a>

#### Purpose/Objective <a href="#howtoguide-estimation-purpose-objective" id="howtoguide-estimation-purpose-objective"></a>

* Story Point estimates include implementation, code review, unit testing, documentation and product hub testing.
* Team must be able to reach a consensus about the size of the story
* Try and break the stories to the smallest logical unit that can be delivered to business

#### Prompts <a href="#howtoguide-estimation-prompts" id="howtoguide-estimation-prompts"></a>

* Consider whether the _current_ team members have done a similar story.
* Consider the upper boundary it may take for a team member to complete the work (eg. experienced vs inexperienced person).
* Impact to financial areas?
* Development:
  * Consider obvious non-functional requirements including performance, the amount of regression testing required, security, compliance, obvious usability.
* Testing:
  * Do we require help from external teams for testing?
  * Testing across multiple brands?
  * Sourcing of data?
  * Would there be any ad-hoc testing (exploratory testing)
  * Cross team impact - splash effect

## **Challenges in estimating** <a href="#howtoguide-estimation-challengesinestimating" id="howtoguide-estimation-challengesinestimating"></a>

* Estimating as a dev, BA or as a tester
* Estimating without considering definition of done
* Estimating without clear understanding of dependencies

### POINTS & MEANING <a href="#fibonacciestimation-points-and-meaning" id="fibonacciestimation-points-and-meaning"></a>

#### 0 – VERY QUICK TO DELIVER AND NO COMPLEXITY. IN MINUTES <a href="#fibonacciestimation-0-veryquicktodeliverandnocomplexity.inminutes" id="fibonacciestimation-0-veryquicktodeliverandnocomplexity.inminutes"></a>

* I know exactly what needs to be done, and it’s going to be a quick Win
* Example: Change color in CSS, fix simple query

#### 1 – QUICK TO DELIVER AND MINIMAL COMPLEXITY. AN HOUR OR SO <a href="#fibonacciestimation-1-quicktodeliverandminimalcomplexity.anhourorso" id="fibonacciestimation-1-quicktodeliverandminimalcomplexity.anhourorso"></a>

* I know exactly what needs to be done, and it’s going to take me little time
* Example: Add placeholder text to a text box

#### 2 – QUICK TO DELIVER AND SOME COMPLEXITY. MULTIPLE HOURS. LITTLE COLLABORATION REQUIRED <a href="#fibonacciestimation-2-quicktodeliverandsomecomplexity.multiplehours.littlecollaborationrequired" id="fibonacciestimation-2-quicktodeliverandsomecomplexity.multiplehours.littlecollaborationrequired"></a>

* I mostly know what needs to be done, where improvements/changes need to be implemented, and it’s going to take me some time
* This might be a full stack story that hits all layers of the vertical, but simple use cases
* Example: Add parameter to form, validation, storage

#### 3 – MODERATE TIME TO DELIVER, MODERATE COMPLEXITY, POSSIBLE UNKNOWNS. SOME COLLABORATION REQUIRED <a href="#fibonacciestimation-3-moderatetimetodeliver-moderatecomplexity-possibleunknowns.somecollaborationreq" id="fibonacciestimation-3-moderatetimetodeliver-moderatecomplexity-possibleunknowns.somecollaborationreq"></a>

* I have a good idea what needs to be done, and it’s going to take me a bit of time
* I will need to collaborate with a team member or two
* Example: Migrate somewhat complex static CSS into a CSS pre-processor

#### 5 – LONGER TIME TO DELIVER, HIGH COMPLEXITY, LIKELY UNKNOWNS. FAIR DEGREE OF COLLABORATION <a href="#fibonacciestimation-5-longertimetodeliver-highcomplexity-likelyunknowns.fairdegreeofcollaboration" id="fibonacciestimation-5-longertimetodeliver-highcomplexity-likelyunknowns.fairdegreeofcollaboration"></a>

* I know what needs to be done at a high level, but there is a good amount of work due to complexity/amount of development, and there are big unknowns we’ll discover as we get into the work.
* Multiple team members including myself will be working on implementing this
* Example: Integrate with third-party API for pushing/pulling data, and link to user profiles in platform

#### 8 – LONG TIME TO DELIVER, HIGH COMPLEXITY, CRITICAL UNKNOWNS. HIGH DEGREE OF COLLABORATION, INTER-TEAM DEPENDENCIES <a href="#fibonacciestimation-8-longtimetodeliver-highcomplexity-criticalunknowns.highdegreeofcollaboration-in" id="fibonacciestimation-8-longtimetodeliver-highcomplexity-criticalunknowns.highdegreeofcollaboration-in"></a>

* I understand the concept and the goals, but it will take a while to deliver due to amount of work, complexity, and unknowns
* Multiple team members, some from other teams as well will be required to meaningfully complete this ticket&#x20;
* If we have an 8, we should breaking them into smaller tasks/issues with smaller point values and minimize the complexity
* This might require a Spike to architect/remove uncertainty, or be created as an epic with more granular stories within it
* Example: Overhaul the layout/HTML/CSS/JS of a web application

#### 13 – LONG TIME TO DELIVERY, HIGH COMPLEXITY, MANY CRITICAL UNKNOWNS <a href="#fibonacciestimation-13-longtimetodelivery-highcomplexity-manycriticalunknowns" id="fibonacciestimation-13-longtimetodelivery-highcomplexity-manycriticalunknowns"></a>

* Similar to an 8, and requires discussions around how to accomplish
* Possibly will not be completed within a sprint
* Example: Migrate application from an outdated data store to new DB technology and ORM

#### 21 – YOU’RE DOING THIS WRONG. 😉 <a href="#fibonacciestimation-21-youredoingthiswrong." id="fibonacciestimation-21-youredoingthiswrong."></a>

## **References** <a href="#howtoguide-estimation-references" id="howtoguide-estimation-references"></a>

[https://technology.amis.nl/agile/8-agile-estimation-techniques-beyond-planning-poker/](https://technology.amis.nl/agile/8-agile-estimation-techniques-beyond-planning-poker/)
