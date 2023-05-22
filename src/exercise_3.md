# Exercise 3

## 1. complete

1. Static review objectives include `......`, `.....`, and `......`
2. It is very useful that test basis has measurable coverage criteria to be used as `......`
3. An element of human psychology called `......` makes it difficult to accept information that disagrees with currently held beliefs.
4. Static testing types include `......`, `......`, `......`, and `......`.
5. Acceptance testing of system by administration staff is usually performed in a `......`
6. Finding defects is not the main focus of `......` testing, its goal is to build confidence in the software.
7. Maintenance testing involve planned releases and unplanned releases called `......`.
8. Triggers for software maintenance include `......`, `......` and `......`.
9. `......` testing is used by developers of commercial off-the-shelf (COTS) software who want to get feedback from potential/existing users, customers before the software product is put on the market.

>> 1. `finding defects - gaining understanding - educating participants`
>> 2. `key performance indicator (KPI)`
>> 3. `confirmation bias`
>> 4. `peer revuew - walkthrough - technical review - inspection`
>> 5. `(simulated) production environment`
>> 6. `user acceptance`
>> 7. `hot fixes`
>> 8. `modification - migration - retirement`
>> 9. `beta and alpha`

## 2. Explain the testing principles in details.

- testing shows the presence of defects
  > testing shows that defects are present but cannot prove that there are no defects
- exaustive testing is impossible
  > testing everything is impossible
- defect clustering
  > smaller number of modules usually is responsible for most of the perational failures
- early testing
  > to find defects early start testing as early as possible in SDLC
- pesticide paradox
  > repeated tests will no longer find more defects
- testing is context dependent
  > done differently in different contexts (safty-critical vs e-commerce system)
- abasence of error fallacy
  > fixing defects does not help if the system built is unusable

## 3. Identify three guidelines to successful conduct of review process.


- clear predefined objectives and measurable exit criteria
- the right people are involved
- testers a valued reviewers
- any checklists are up to date
- management supports a good review process

## 4. Clarify the tester role during each of SDLC phases. (`not answered`)

## 5. What should a tester do in case a component is not finished and he needs to conduct component integration testing?

> Use driver

## 6. Compare between regression and confirmation testing types.

- confirmation testing
  > part as defect fix verification
  >
  > - after the defect is detected and fixed, the software should be re-tested
- regression testing
  > testing the system to check that changes have not broken previously working code
  >
  > - re-run every time a change is made
  > - some fixes may preduced unintended side-effects that are called regressions

## 7. Illustrate steps of dynamic testing using a diagram.

![v model](images/v-model.png)

## 8. Specify Formal Review/Inspection Activity

1. Evaluating the review findings against the exit criteria to make a review decision 
2. Explaining the scope, objectives, process, roles, and work products to the participants 
3. Noting potential defects, recommendations, and questions 
4. Defining the entry and exit criteria

>> 1. Review meeting/issue communication and analysis
>> 2. Initiate review 
>> 3. Individual preparation 
>> 4. Planning 

## 9. Whose Responsibility in Review?

1. Document all the issues, problems, and open points that were identified during the meeting. With the advent of tools to support the review process, especially logging of defects/open points/decisions, there is often no need for a scribe
2. Decide on the execution of reviews, allocates time in project schedules and determines if the review objectives have been met
3. Lead, plan and run the review. May mediate between the various points of view and is often the person upon whom the success of the review rests

>> 1. scribe
>> 2. manager
>> 3. moderator/facilitator

## 10. Specify Review Technique

1. Reviewers are provided with structured guidelines on how to read through the work product based on its expected usage. 
2. Reviewers detect issues based on set of questions based on potential defects, which may be derived from experience.
3. Reviewers are provided with little or no guidance on how this task should be performed. It needs little preparation and is highly dependent on reviewer skills.
4. Reviewers take on different stakeholder viewpoints in individual reviewing.

>> 1. Scenario-based/dry run.
>> 2. Checklist-based.
>> 3. Ad hoc.
>> 4. Perspective-based reading.

## 11. In Which Testing Level Can Defect be Found?

1. Incorrect sequencing or timing of interface calls 
2. Incorrect in code logic
3. Failure of the system to work properly in the production environment(s) 

>> 1. Integration testing  
>> 2. Component testing
>> 3. System testing

## 12. Replace with Key Term(s)

1. Most formal review type, Led by the trained moderator, involves peers to examine the product, The defects found are documented in a logging list or issue log.
2. Testing without having any knowledge of the interior workings of the application.
3. is the detailed investigation of internal logic and structure of the code, also called: glass testing or open-box testing.
4. Tests that evaluate functions that the system should perform.
5. is the process of testing individual components in isolation.
6. focuses on interactions and interfaces between integrated components. It is generally automated. It is often the responsibility of developers.
7. focuses on interactions and interfaces between systems and packages. It is the responsibility of testers.
8. a level of testing that validates the complete and fully integrated software product.
9. is a stage in the testing process in which users provide input and advice on system testing.
10. Users of the software test the software in a lab environment at the developer’s site.
11. made available to users to allow them to experiment and to raise problems that they discover in their own environment.
12. is performed against a contract’s acceptance criteria for producing custom-developed software. 
Acceptance criteria should be defined when the parties agree to the contract.
13. is performed against any regulations that must be adhered to, such as government, legal, or safety regulations.
14. is the testing of “how well” the system behaves, It involves testing a software for the requirements which are non-functional in nature but important such as performance, security, scalability, etc.
15. It is a type of retesting that is carried out by software testers as a part of defect fix verification.
16. It is possible that a change made in one part of the code may accidentally affect the behaviour of other parts of the code, whether within the same component, in other components.


>> 1. `Inspection`
>> 2. `black-box testing`
>> 3. `White-box testing`
>> 4. `functional testing`
>> 5. `Component testing`
>> 6. `Component integration Testing`
>> 7. `System integration testing`
>> 8. `system testing`
>> 9. `user acceptance testing (UAT)`
>> 10. `Alpha testing`
>> 11. `Beta testing`
>> 12. `Contractual acceptance testing`
>> 13. `Regulatory acceptance testing`
>> 14. `Non-functional testing`
>> 15. `Confirmation testing`
>> 16. `Regression testing`
