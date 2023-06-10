# Lecture 5

# 1. test case design and techniques

- blackbox
  - based on requirements
  - techniques
    1. equivalcence partitioning
       - valid partitions
       - invalid partitions
    2. boundary value analysis (only for ordered numeric or sequential partitions)
    3. decision tables
       - `minimum coverage standard` is to have at least one test case per decision rule in the table.
       - different combinatiosns of conditions result in different outcomes
       - good for recording complex business rules
    4. state transition testing
       - `state table` shows the relationship between states and inputs and highlights invalid transitions
    5. pairwise testing
    6. use case testing
       - useful for designing acceptance testings with customer participation
- white
  - based on code and the design of the system
  - ability to derive caoverage of the whole application
  - techniques
    1. statement caoverage
       - `coverage` is the # of executable statements executed by the test divided by the total # of statement
    2. branch caoverage
    3. decision caoverage
       - `coverage` is the # of decision outcomes executed by the test divided by the total # of decision outcomes
- expericed
  - based on the knowledge of the tester with similar applications
  - techniques
    1. error guessing
       - enumerate al list of possible defects
    2. exploratory testing (informal tests)
       - informal (not pre-defined) tests
       - the test results are used to create tests for the areas that may need more testing
       - conducted using session-based testing
       - useful where
         - there are few specifictaion
         - severe time pressure

> `Decision coverage` is stronger than `statement coverage`,
> 100% decision coverage guarantees 100% statement coverage,
> but not vice versa.

# 2. choosing a test technique **(slides 21)**

depends on some factors

- type of the system
- level of risks
- type of risks
- knowledge of the testers
- time and budgets

# 3.1 tester role

- review and contribute to test plans
- analyze, review requirements and user stories
- identify test conditions
- design test environment
- implements test cases
- prepaire test data
- execute tests and evaluate the result
- automate the testing

# 3.2 testing role based on level

| level                  | resposibility (done by)                             |
| ---------------------- | --------------------------------------------------- |
| component itegration   | developer                                           |
| system integration     | independent test team                               |
| operational acceptance | operations/systems administration staff             |
| user acceptance        | business analyst , subject matter experts and users |

# 4. independent tester

- benefits
  - testers are unbiased and see other and different defects
  - testers can verify assumptions made by people during specification and implmentation of the system
- drawbacks
  - isolation from development team
  - developers may lose sense of responsibility for quality
  - testers may be seen as bottleneck for release

# 5. configuration management

- the purpose is to
  1. maintain integrity of work products throught the life cycle
  2. maintain traceability throughout the test process
  3. for the testers, it helps uniquely identifing the tested item, test documents, ...

# 6.1 risks and testing

> `risk`
>
> > the chance of an event, threat occurring and resulting in undesirable problem

> `level of risks`
> depends on
>
> - likelihood/probability of an event happening
> - impact/harm resulting from event

> `risk-based testing` used to
>
> 1. focus effort required during testing
> 2. decide where/when to start testing and identify areas that need more attention.
> 3. reduce the probability of an adverse event occurring, or to reduce its impact.

> `Resulting product risk information is used to guide test activities`
>
> - determine the test techniques to be employed.
> - determine the extent of testing to be carried out.
> - prioritize testing to find the critical defects as early as possible.
> - determine whether any non-testing activities could be employed to
>   reduce risk (e.g., providing training to inexperienced designers).

## 6.2 risk types

> `project risks`
>
> > have negative effect on project's ability to achieve its objectives
> > examples
>
> - organizational factors
>   - skill, training & staff shortages
>   - personal issues
>   - political issues
>   - improper attitude such as not appreciating the value of finding defects during testing
> - technical issues
>   - problem identifing the right requirements
>   - requirements can't be met
>   - environment not ready
>   - low code design
> - supplier issues
>   - contractual issues

> `pruduct risks`
>
> > the possibility that a work product may fail to satisfy the needs of users/stakeholders
> > examples
>
> - may not perform intended functions
> - may not support some non functional requirements
> - bad response time
> - bad user experience

## 3.1 bug life cycle

> `defect age`: time gap between date of detection & date of closure

- `new` posted for the 1st time
- `assigned` assign bugs to the developing team
- `open` developer started working on the defect fix to be added to (duplicate, deffered or not a bug)
- `fixed` bug is fixed and is passed to testing team
- `pendeing retest`
- `retest` do the retesting on of the changed code
- `verified` the bug is verified to be fixed
- `reopen` bug is still remains after is fixed
- `closed` the bug no longer exists on the software

## 3.2 bug status by the developer

- `duplicate`
- `rejected`
- `deffered` to be fixed in the next releases, or its priority is low
- `not a bug`

## 4. testing tools

> `benefits of using testing tools`
>
> - reduction in repetivive manual work
> - greater consistency and repeatability
> - easier access to information about testing (metrics, graphs, ...)

> `risks of using testing tools`
>
> - expectations for the tool may be unrealistic
> - time and cost for the initial introduction of the tool
> - vendor may provide a poor response for support, defect fixes, and upgrades
> - may be relied on too much
> - new tehcnology may not be support by the tool
> - open source project may be suspended

# 5. test execution tools

execute test objects using automated test scripts

> `approuches`
>
> - data-driven testing
>   - separating the “data set” from the actual “test case” (code)
>   - the same test can be run with many input avaiable to get better coverage
> - keyword-driven testing
>   - framework has all instructions written in an external execl file
>   - generic script processes keywords describing the actions to be taken to perform a specific step
> - model-based testing (**MBT**)
>   - use system's models (UML diagrams) to generate test caes

# 6. principles for Tool Selection

- `Identification of opportunities for an improved` test process supported by tools
- Understanding of technologies used by test objects (`select tool compatible with technology`)
- Check used build and CI tools within organization, to `ensure tool compatibility and integration`
- `Evaluation of the tool against clear requirements` and objective criteria
- Consideration of whether or not the `tool is available for a free trial period` (and for how long)
- Evaluation of the vendor (`including training/commercial aspects/support after sale`)
- Identification of `internal requirements for coaching and mentoring in the use of the tool`
- Evaluation of `training needs and skills` of those who will be working directly with the tool(s)
- Consideration of `pros and cons of various licensing models` (e.g., commercial or open source)
- `Estimation of a cost-benefit` ratio based on a concrete business case (if required)

# 7. pilot Projects for introducing a Tool

> `objectives`
>
> - gain in-depth knowledge about tool strengths and weaknesses
> - evaluate how the tool fits with existing processes
> - decide on standard ways of using, managing, storing it
> - Assess whether the benefits will be achieved
> - Understand the metrics that you wish the tool to collect and report

# 8 success Factors for Tools

- `Rolling out the tool` to the rest of the organization incrementally
- Adapting and improving processes to fit with the use of the tool
- `Providing training, coaching,` and mentoring `for tool users`
- `Defining guidelines` for the use of the tool (e.g., internal standards for automation)
- `Gathering usage information` from the actual use of the tool
- Monitoring tool use and `benefits`
- `Providing support` to the users of a given tool
- `Gathering lessons` learned from all users
