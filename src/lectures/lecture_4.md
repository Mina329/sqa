# Lecture 4

# 1. STLC (software testing life cycle)

## 1.1 requirement analysis

- activities
  > - analyzing the (SRC)
  > - prepare (RTM)
  > - prioritizing the features
  > - analyzing the automation feasibility
- deliverables
  > - RTM
  > - automation feasibility report

## 1.2 test planning

> answers the question `what to test?`

- activities
  > - prepare test plan/strategy document
  > - test tool selection
  > - test effort estimation
  > - determine roles and responsiblities
- deliverables
  > - test plan/strategy document
  > - effort estimation

## 1.3 test case development

    >  creation and verification of test cases

- activities
  > - create test cases
  > - review the baseline testcases
  > - create test data
- deliverables
  > - test cases
  > - test data

## 1.4 environment setup

- activities
  > - prepare hardware and software
  > - setup environment
  > - perform smoke test
- deliverables
  > - environment ready
  > - smoke test result

## 1.5 test execution

- activities
  > - execute test cases
  > - document the test results
  > - map defects to test cases in RTM
  > - track defects to closure
- deliverables
  > - completed RTM
  > - testcases updated with results
  > - defect report

## 1.6 test cycle closure

> testing team meat, discuss and analyze the artifacts

- activities
  > - evaluate cycle completion criteria based on time, test coverage, cost, ...
  > - prepare test metrics
  > - prepare test closure
  > - find the defect distribution by type and severity
- deliverables
  > - test closure report
  > - test metrics

# 2.1 testing estimation

> approximate how log a task would take

- techniques

  > - metrics-based
  > - expert-based technique

- estimation considerations
  > - Team skills
  > - Complexity of the application
  > - Historical data
  > - Resources availability
  > - System environment and downtime

## 2.1.1 PERT (three point estimation)

> three point estimation
>
> > test estimate = (O+(4xM)+P)/6
> > O = optimistic estimate
> > M = most likely estimate
> > P = passimistic estimate

## 2.1.2 work breakdown structure (WBS)

1. create WBS by breaking down into small pieces
2. divide modules into sub-modules
3. divide functionalities into sub-functionalities
4. figure out the number of tasks
5. estimate the number of tasks
6. estimate the effort for each task
7. estimate the duration for each task

## 2.1.3 wideband delphi

> WBS is distribute to a team of 3-7 members for re-estimating

- this technique speeks more on experience rather that statistical formula
- emphasizes on the group iteration to reach an agreement

## 2.1.4 percentage distribution

> all the phases of SDLC are assigend effort in %

## 2.1.5 experience-based testing estimation

> based on similarites and experts that already tested similar applications

# 3. software test metrics

> `metric`
>
> > a quatitive measure of degree to which a system processes a given attribute

## 3.1 examples of test metrics

- schedule slippage
  > (actual end date – estimated end date) / (planned end date – planned start date) x 100
- number of test per time period
- fixed defect percentage
- percentage test cases executed
- requirement creep
  > (total number of requirements added / number of initial requirements) x 100

# 4. entry criteria

> minimum set of condition that should be met before starting the testing

- testing environment is available
- testable code is ready
- test data is ready

# 5. exit criteria

> minimum set of condition that should be completed in order to stop the testing
>
> > - determine if the testing is completed or not
> > - defined in test plan

- test planned have been met
- not high severity defects
- high risk area are completely tested

# 6 test progress monitoring

- Test Progress Monitoring
  > provide feedback and visibility about test activities
- Test Reporting
  > summerizing information
  >
  > - `test progress/status report` is Test report prepared during a test activity
  > - `test summary report` is test report prepared at the end of a test activity
- Test Control

# 7 test work products

> help in estimating the testing efforts required

`examples`

- test planing work products
- test monitoring and control work products
- test analysis work products
- test design work products
- test implementation work products
  - test procedures
  - test suites
  - test execution schedule
- test execution work products
  - documentation
  - defect reports
- test completion work products
  - summary reports
  - finalized test ware

## 7.1 examples on Test Reports

- Summary of testing performed
- Information on what occurred
- Deviations from plan
- Status of testing
- Factors that have blocked or continue to block progress
- Metrics of defects, test cases, test coverage
- Residual risks
- Reusable test work products produced

# 8 test control

> any guiding or corrective actions taken as a result
> of information gathered and reported

`examples`

- re-prioritizing tests
- changing test schedules
- re-evaluating whether test item meets entry or exit criterion

# 9 test strategy vs test plan

1. **test strategy**
   > a high level document that capture the approach on how we go about testing and achieve the goal
   - `components`
     - scope
     - overview
     - test approach
     - testing tools
     - standartds
   - by project manager
   - from business requirement specification (BRS)
   - static document
   - at organization level
2. **test plan**
   > a document that contains the plan for all testing activities
   - `components`
     - test plan identifier
     - features to be tested
     - features not to be tested
     - pass/fail criteria
     - responsibilities
     - staffing and traning needs
   - by test lead or test manager
   - from the oriduct description (SRS), use case documents
   - dynamic document
   - at project level

# 10 test strategy types

- analytical
  > based on analysis of some factor (`ie risk based testing`)
- model-based
  > based on model of some required aspect of the product
- methodical
  > make systematic use of some predefined set of test conditions
- process-compliant
  > designing test based on external rules and standartds
- directed
  > by advice or instructions of stakeholders
- regression-averse
  > desire to avoid regression of existing capablities (reuse of existing test ware)
- reactive
  > reactive to system being testing and events

# 11 test plain

`master test plan`
it outlines test activities for development and maintenance projects.

`includes activities`

- determing the scope, objectives
- defining the approach
- making decision about what to test
- scheduling of test analysis
- selecting metrics
- selecting level of details

# 12 test scenario

> gives the idea of what we have to test

# 13. test case

> set of positive and negative executable steps of a test scenario

## 13.1 logical vs physical test case

**`logical`**

> describes what is tested and not how it is done

**`physical`**

> fill the details in the corresponding logical test

## 13.2 negative vs positive test case

**`negative`**

> try to break the software by performing invalid actions

**`positive`**

> ensure that the user can perform the appropriate actions by valid data

## 14 defect report

- state the problem
- defect severity
  > the impact of bug on application (showstopper/critical/high/medium)
- defect priority
  > the impact of the bug on customer business

**`includes`**

- identifier
- title
- description
- expected and actual result
- severity of defect
- priority to fix
- change history

# 15 test procedures

> specifies the sequence of action for a test

- identifier
- purpose
- special requirements
- procedure steps

# 16 requirement traceability matrix (RTM)

> connects requirements to test cases throughout the validation process

- `importace of traceability`
  > - Analyzing the impact of changes
  > - Making testing auditable
  > - Meeting IT governance criteria
  > - Improving the understandability of test progress reports

# 17 test closure report

> report that is created once the testing phase is succesfully completed by meeting exit criteria

- gives a summary of all the tests conducted
- gives detailed analysis of the bugs removed and errors found
- presents list of known issues
- created by test lead and reviewed by stakeholders
