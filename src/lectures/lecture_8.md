# Lecture 8

# 1. test automation pyramid

`unit -> integration -> system -> acceptance`

`lower  ---> higer`

| lower                                         | higher                          |
| --------------------------------------------- | ------------------------------- |
| automated using api-based tools               | automated using gui based tools |
| lower cost                                    | higher cost                     |
| faster                                        | slower                          |
| more reliable                                 | less reliable                   |
| less integration required in test environment | more integration                |

# 2. automating api tests

- ensure data flow and integration points are working as expected.
- help execute non-functional requirements
- using tools like `postman, soapUI`

# 3. testing quadrants

- apply to `dynamic testing` rather thant static testing

|                | quandrant Q1                                               | quandrant Q2                                                              | quandrant Q3                                                                   | quandrant Q4                          |
| -------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ------------------------------------- |
| about          | unit level, technology facing, and supports the developers | system level, business facing, and confirms product behaviour.            |                                                                                |
| in what level? | unit                                                       | system                                                                    | system or user acceptance                                                      | system or operational acceptance      |
| automation?    | should be automated                                        | manual or automated                                                       | manual and user-oriented                                                       | often automated                       |
| contains?      |                                                            | functional acceptance tests, examples, story test, prototypes, simulation | tests that critique the product, exploratory testing, scenarios, process flows | qualities test (ie performance, load) |

# 4. agile tester skills

- Competent in `test automation, test-driven development, acceptance test-driven`
  development, .. etc.
- Plan and `organize their own work`
- Collaborate, `work in pairs` with programmers
- Respond to `change quickly`
- Actively `acquire information from stakeholders`
- Accurately evaluate and `report test results/progress` and product quality
- Work effectively to `define testable user stories`
- `Be positive and solution-oriented`

# 5. agile tester role

- Understanding, implementing, and `updating test strategy`
- `Reporting defects` and working with the team to resolve them
- Measuring and `reporting test coverage`
- Ensuring `proper use of testing tools`
- Configuring, using, and `managing test environments and test data`
- `Coaching other team members`
- Ensuring the `appropriate testing tasks are scheduled`
- Actively `collaborating with developers`
- `Participating proactively`

# 6. tester role in scrum projects

> includes activities that generate and provide feedback not
> only on test status, test progress, and product quality

- **Cross-functional**: brings a `different set of skills` to the team and `The team works together` on test strategy, planning,
- **Self-organizing**
- **Co-located**: `Testers sit together with the developers`
- **Collaborative**: `collaborate with team members`
- **Empowered**: `Technical decisions are made by the team as a whole`
- **Committed**: `committed to question and evaluate the product’s behaviour`
- **Transparent**: `testing progress is visible on the Agile task board.`
- **Credible**: `ensure the credibility of the strategy for testing`
- **Open to feedback**: `Retrospectives allow teams to learn from successes and from failures`.
- **Resilient**: `respond to change`

# 7. Tester Role in Scrum Projects Sprint Zero

> `sprint zero` is the first iteration of the project where many preparation activities take
> place.

**activities during this iteration**

- Identify the `scope of the project` (i.e., the product backlog)
- Create an `initial system architecture and high-level prototypes`
- Plan, acquire, and `install needed tools`
- Create an `initial test strategy`
- Perform an `initial quality risk analysis`
- Define test `metrics`
- Specify the `definition of “done”`
- Create the `task board`
- Define `when to continue or stop testing`

# 8. quality risks in agle projects

> agile teams determine an acceptable number of test cases to execute using `risk identification, analysis, and risk mitigation strategies`

|      | quality/product risks                                     | project risks                                             |
| ---- | --------------------------------------------------------- | --------------------------------------------------------- |
| when | primary effect of potential problem is on product quality | primary effect of potential problem is on project success |

quality risks analysis take place at 2 places

- release planning
  - high-level view of risks
  - by `business representatives`
- iteration planning
  - by `whole team`

## 8.1 quality risk analysis during iteration planning

1. gather the team together including the tesrers
2. list all backlog items
3. itentify the quality risks with each item
4. access each identified risk
   - categorizing the risks
   - determining the risk level based on `impact` & `likelihood of the defect`
5. determine the extent of testing proportional to the level of risk.
6. select the appropriate test techniques
7. then design, implements, and execute the tests

# 9. estimating testing effort based on content and risk

- techniques
  - planning pokering
  - t-shirt sizing

# 10. acceptance criteria

- addresses the following topics
  - `functional behaviour` observable behaviour with user actions
  - `quality characteristics` How the system performs the specified behaviour
  - `scenarios (use cases)` sequence of actions between an external actor
  - `business rules` Activities that can only be performed in the system under certain conditions
  - `external interafaces` between the system the outside world
  - `constraint` like embedded hardware, ... etc
  - `data difintions` format, data type, ... etc

## 10.1 defintion of done

1. for unit testing
   - 100% decision coverage where possible
   - static analysis is performed
   - no unresolved major defect
   - no known unacceptable debt remaining
   - all code, unit test, and result reviewed
   - all unit tests automated
2. for integration testing
   - all `functional requirements tested`
   - all `interfaces tested`
   - all quality rikss covered
   - no unresolved major defect
   - all defects are reported
   - all `regression test automated`
3. for system testing
   - `end-to-end` of user stories
   - all `user personas covered`
   - import `quality characteristics covered`
   - testing done `in a production-like environment`
   - all quality risks covered
   - all `regression tests automated`
   - all defects found and fixed
4. done for user stories
   - `user stories selected for iteration are complete` (have testable acceptance criteria)
   - all `elements reviewed`
   - all `tasks identified`
5. for feature
   - all `user stories approved by customer`
   - the `design is complete`
   - `the code the complete`
   - `performed unit, component, and system tests`
   - no major defects remaining
   - feature `docs are complete`
6. for iteration `(not all iteration result in a release)`
   - all `features for iteration are complete and tested`
   - any `non-critical defects` that cannot be fixed within the constraint of the iteration `is added to the product backlog and prioritized`
   - features integration completed
   - `docs written, approved`
7. for release
   - `coverage` by testing
   - `quality` defect intensity, defect density, risks are understood and acceptable
     - **defect intensity**: how many defects are found per day and transaction
     - **defect density**: number of defects found compared to number of user stories, effort, and/or quality attributes
   - `time` delivery date has been reached
   - `cost`

# 11. exploratory testing

important in agle due to

- limited time available for test analysis
- limited details of user stories

> guided by `test charter`
>
> - provides the test conditions to cover during a
>   time-boxed testing session (guides the exploratory testing, design and execution)
> - includes
>   - charter
>   - areas
>   - environment
>   - start date
>   - tester name
>   - duration
>   - task breakdown
>   - testing notes
>   - data files
>   - bugs
>   - issues
>   - session startup time
>   - design and execution

# 12. session based test management

- manages exploratory test
- last from 60-120 mins
- includes
  - survay (learn how it works)
  - analysis (evaluation of the functionality)
  - deep coverage (corner cases, scenarios, ...)

# 13. tools in agile

some agile teams uses all-inclusive tool (Application Lifecycle Management `ALM`) that provide features relevet to agile (ie task boards, burndown charts, user stories)

# 14. task management and tracking tools

agile use physical story/task boards to

- record stories
- capture team members' estimates on there task and calculate efforts
- provide a visual representation
- integrate with configuration management tools

# 15. communication and information sharing tools

- wikis
- instant messaging
- desktop sharing

> `should not` replace, face-to-face communication in Agile teams

## 15.1 wikis

share an online knowledge base on tools and techniques including

- product feature diagrams
- tools and techniques
- metrics, charts
- conversations

## 15.2 desktop shareing and capturing tools

- used for distributed teams, product demonstrations, code reviews, and even pairing
- capturing product demonstrations at the end of each iteration,

# 16. configuration management tools

- used to store source code, automated tests in the same repository
- provide traceability between which versions
- allow for rapid change without losing historical information
- includes
  - centralized version control system `VCS`
  - distributed `VCS`

# 17. test Design, Implementation, and Execution Tools

- test design tools
- test case management tools
- `test data preparation and generation tools` generate data to populate an application’s database
- `test data load tools` are available to make the process reliable and efficient
- `automated test execution tools` allow testers and business staff to express the expected system behaviour in tables or natural language
- `exploratory test tools` capture and log activities performed on an application during an exploratory test session
