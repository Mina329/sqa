# Lecture 7

# 1. continuous integrations

integrating all changed components regularly, at least once a day

## 1.2 components integrations automated activities

1. static code analysis
2. compile
3. unit tests
4. deploy
5. integration tests
6. reports (dashboard)

- post results of all activities

## 1.3 CI chanllenges

- CI tools have to be introduced and maintained
- CI process must be defined and established
- test automation requires additional resources and may be complex to establish
- test coverage is essential
- teams sometimes over-rely on unit tests and ignore system and acceptance tests

# 2. release planning vs iteration planning

| release planning                                          | iteration planning                   |
| --------------------------------------------------------- | ------------------------------------ |
| defines and re-defines product backlog                    | concerned with the iteration backlog |
| high level                                                | low level                            |
| nvolve refining larger user stories                       |                                      |
| establish and prioritize the user stories for the release | concerned with the iteration backlog |
| provides the basis for a test approach                    |                                      |

- release planning
  - `Defining testable user stories`, including acceptance criteria
  - Participating in project and `quality risk analyses`
  - `Estimating testing effort` associated with the user stories
  - Defining the `necessary test levels`
  - Planning the testing for the release
- iteration planning

  - Participating in the `detailed risk analysis of user stories`
  - Determining the `testability of the user stories`
  - Creating `acceptance tests` for the user stories
  - `Breaking down user stories` into tasks (particularly testing tasks)
  - `Estimating testing effort` for all testing tasks
  - `Identifying functional and non-functional` aspects of system to be tested
  - Supporting and `participating in test automation` at multiple levels of testing

> `Test oracle`:
>
> - compare expected output with actual mechanism that determines whether software executed correctly for a test case

# 3. agile principles

> - `stablization iterations`
>   - occur periodically to resolve any remaining `defects` and any other form of `technical debt`
> - `fix bug first`
>   - address defects remaining from the previous iteration
> - `Pairing`
> - automation test at all levels
>   - involve testers working together in twos to test a feature
> - Developers focus on creating unit tests.
> - Testers should focus on creating automated integration,
> - Lightweight work product documentation
> - Changes to existing features has regression testing implications

# 4. test activities during iteration

during an iteration, any given user story will typically progress
sequentially through the following test activities

- unit testing
- feature acceptance testing
  - feature verification testing
    - automated
    - by tester or developer
    - against user's story acceptance crieteria
  - feature validation testing
    - manual
    - determines if the feature is fit for use and to get feedback from the business stakeholders

# 5. project work products

caegories

- business-oriented work products
  - what is needed (ie requirements, specification/user stories)
- development work products
  - how the system is built (databases, erd, code or test cases)
- test work products
  - how the system is tested (test strategies and plans, manual and automated tests)

> `Configuration management system` allow the CI of new software with the system, with the static analysis and unit tests run repeatedly as new software is checked in

# 6. orgaizational options for independent testing

1. embedded tester(s) witthin the team
   - risk of loss of independence and loss of objective evaluation
2. fully independent seperate test team during the final days of each sprint
   - provide unbaised evaluation
   - time preasures, lack of understanding lead ot problems with this approach
3. independent seperate test team assigned to agile team on al long-term basis at the beginning of the project

# 7. test status and progress

communication is done by `wiki dashboards`, `dashboard style emails`, `stand-up meetings`

- `burndown charts`
  - represents the amount of work left to be done against time allocated to the release

# 8. benefits of automated tests

- provide rapid feedback on product quality
- provide a living document of system functionality
- run before source code is checked into mainline to ensure not breakage on the build
- automated unit test results provide immediate feedback on code and build quality, but not on product quality.

# 9. automated Acceptance Tests

- run regularly as part of CI
- run against a complete system
- test results provide feadback on product quality with respect to regression

`smoke test` (build verification tests)

- an initial subset of automated tests to cover critical system functionality and integration points

# 10. agile testing techniques

- test-driven development
- behaviour-driven development
- acceptance-driven development

## 10.1 TDD

- concenred primarily with thes testing of a component as a unit
- suited for component testing

- benefits
  - code coverage
  - regression testing
  - simplified debugging
  - system documentation

## 10.2 BDD

- functional/feature test of expected behaviours of an application as a whole
- concerned primarily with the specification of the behaviour of the
  system under test as a whole
- suited for acceptance and regression testing

- its results used by developers to develop test cases
- format
  - given
  - when
  - then

## 10.3 acceptance test-driven development ATDD

- involves cooperative stakeholders using plain language to write acceptance tests
- written from the user’s external point of view.
- is more in tune with the user story
- focus on defining the requirements of a feature
