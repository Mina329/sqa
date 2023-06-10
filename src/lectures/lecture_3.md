# Lecture 3

# 1. software systems context

- defects occur due to:
  > - human beings are imperfect
  > - time presure
  > - complex code
  > - infrastructure complexity
- can lead to
  > - loss of money
  > - loss of time
  > - loss of business reputation
  > - injury or death

> > Error -> Defect -> Failure

> error:
>
> > a human action that produces an incorrect result
>
> defect:
>
> > a flaw in a system that can cause to failure
>
> failure
>
> > deviation of the system

# 2. testing objectives

- evaluate work products
- verify whether all specified requirements have been fulfilled
- build confidence
- prevent and find defects
- provide info to stakeholders
- reduce risks
- comply with legal standards

# 3. testing principles

## 3.1 testing shows the presence of defects

> testing shows that defects are present but cannot prove that there are no defects

## 3.2 exaustive testing is impossible

> testing everything is impossible

## 3.3 defect clustering

> smaller number of modules usually is responsible for most of the perational failures

## 3.4 early testing

> to find defects early start testing as early as possible in SDLC

## 3.5 pesticide paradox

> repeated tests will no longer find more defects

## 3.6 testing is context dependent

> done differently in different contexts (safty-critical vs e-commerce system)

## 3.7 abasence of error fallacy

> fixing defects does not help if the system built is unusable

# 4. testing's contributions to success

should be applied with in at the appropriate level of expertise, points in SDLC

# 5. key performance indicator (KPI)

very useful if the test basis has measurable coverage criteria defined

# 6. testing througout SDLC

- waterfall
  > after all
- incremental
  > built and tested in pieces
- iterative
  > groups are built and tested together

# 7. V-Model

- static testing
  - user/business requirements
  - system requirements
  - techinal specification
  - program specification

> coding

- dynamic testing
  - unit test
  - integration test
  - system test
  - acceptance test

## 7.1 static testing

> manual examination of work products (without code execution)

- applied with tools to evaluate work written in natural language
- most maintability defects can only be found by static testing
- enable early detection of defects before dynamic testing

### 7.1.1 static testing reviews

- formal
- informal

### 7.1.3 static reviews objective

- finding defects
- gaining understanding,
- educating participants

### 7.1.2 static testing types

- peer review
- walkthrough
- technical review
- inspection
  - most formal review type
  - by team moderator
  - specified entry and exit criteria
  - documented defects by logging list
  - formal follow-up

# 8. reviews

## 8.1 formal review roles and responsibilities

| rele                  | responsibility                        |
| --------------------- | ------------------------------------- |
| manager               | dcides on the execution of reviews    |
| moderator/facilitator | lead, plan and run the review         |
| author                | the writer                            |
| reviewers             | with techinal and business background |
| scribe                | documents all the issues              |

## 8.2 activities of formal review/inspection

- `planing`
  > - defining the scope
  > - estimating effort and timeframe
  > - identifying review characteristics
  > - selecting the people
  > - definning the entry and exit criteria
- `initiate review`
  > - distributing work product
  > - explaining the scope, objectives, ..
  > - ansering any questions
- `individual review`
  > - reviewing all or part of product
  > - nothing potential defect, recommnedation
- `review meeting/issue communication and analysis`
  > - communicating identified defects
  > - evaluating and documenting quality characteristics
- `fixing and reporting`
  > - creating defect reports
  > - fixing defects (by author)
  > - recording updated status

### 8.2.1 review techinques

- ad hoc
  > - reviewers are provided with little guide
- checklist-based
- scenarios and dry runs
- prespective-based reading
  > - take on different stakeholder viewpoints

### 8.2.2 success factors of reviews

- clear predefined objectives and measurable exit criteria
- the right people are involved
- testers a valued reviewers
- defects found are welcomed and expressed objectively
- any checklists are up to date
- management supports a good review process

# 9. static analysis by tools

# 10 limitation of static analysis

- can check conformance with specification but not customers' real requirements
- cannot check non-functional characteristics

# 11. testing methodologies

- white testing
- black testing

## 11.1 black box testing

> testing without knowledge of the interior workings of the application

- tester is unaware
- user stories are used as test basis
- deviations for the requirements are checked

## 11.2 white box testing (glass testing)

> detailed investigation of internal logic and structure

- may be proformed at all test levels

# 12 testing types

- functional
- nonfunctional
- structural/white box
- change-related (Re-testing regression)

## 12.1. functional

> evaluate function that the system should perform

- component/unit/module testing
  > testing individual components in isolation
- integration testing
  > integrate all unit tests
  >
  > - component integration testing
  >   - interaction between integrated components
  >   - done by developer
  > - system integration testing
  >   - interaction between system packages
  >   - done by tester
  - driver
    > calls the component to be tested
  - stub
    > is called from the software component

## 12.2 system testing

> complete and fully integrated software product

- end-to-end evaluation
- non-functional
- by independent testers

## 12.3 acceptance testing

- user acceptance testing `UAT`
  > users provides inputs and advice
- operational
  > by operations/admins staff in simulated production environment
  >
  > - backup and restore
  > - installing, upgrading
  > - disaster recovery
  > - user management
- alpha and beta
  > used by developer of commercial of-the-shelf (cots)
- contractual acceptance testing
  > - by contract's acceptance criteria
  > - by users or independent tester
- regularity acceptance testing
  > performed against any regulations

## 12.4 non-functional testing

> testing of `how well` the system behaves for non-functional requirements

- reliability
- usability
- efficiency
- maintainability
- security
- load
- stress
- volume
- baseline
  > referes to the validation of the documents and specifications
- interoperability
  > the ability to interact with specified system

## 12.5 structural testing

> based on the system's internal structure

- interested in what is happening `inside the system/application`
- often referred to as white box
- performed at all test levels
- testers require the knowledge of software implementation

## 12.6 change-related testing

> should be done to confirm that the changes have corrected the defect

- confirmation testing
  > part as defect fix verification
  >
  > - after the defect is detected and fixed, the software should be re-tested
- regression testing
  > testing the system to check that changes have not broken previously working code
  >
  > - re-run every time a change is made
  > - some fixes may preduced unintended side-effects that are called regressions

## 12.7 debuging

> identifies and fixes the source of defects

## 12.8 maintenance testing

> focuses on testing the changes to the working system

- involve planned releases or unplanned releases (`hot fixes`)
- triggers for maintenance
  - modification
  - migration
  - retirement

> `impact analysis` is useful for regression testing during maintenance testing.
