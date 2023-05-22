# Exercise 4

## 1. Identify testing estimation technique

1. Breaking down the test project into modules; sub-modules; functionalities; tasks and estimate effort/duration for each task.
2. Assumes that you already tested similar applications in previous projects and collected metrics from those projects.
3. Three types of estimations most likely/optimistic/pessimistic are calculated for each activity. 
4. Work breakdown structure is distributed to a team comprising of 3-7 members for re-estimating the tasks and final estimate is the result of the summarized estimates based on the team agreement.

>> 1. `work breakdown structure WBS`
>> 2. `experience based testing`
>> 3. `PERT estimation technique`
>> 4. `wideband delphi technique`

## 2. Identify Test Strategy Type

1. Tests rely on making systematic use of predefined set of tests/test conditions, such as taxonomy of common types of failures, list of important quality characteristics, or company-wide look-and-feel standards.
2. Tests are designed and implemented, and may immediately be executed in response to knowledge gained from prior test results rather than being pre-planned.
3. Tests are designed based on some required aspect of the product, such as function, business process, internal structure, non-functional characteristic.
4. Tests include reuse of existing test ware (especially test cases and test data) and test suites. 
5. Tests driven primarily by the advice, guidance, or instructions of stakeholders, business domain experts, or technology experts, who may be outside the test team or outside the organization itself.


>> 1. `methodical`
>> 2. `reactive`
>> 3. `model-based`
>> 4. `regressive-averse`
>> 5. `directed`

## 3. Identify testing life cycle phases and deliverable from each phase.

### 3.1 requirement analysis

- activities
  > - analyzing the (SRC)
  > - prepare (RTM)
  > - prioritizing the features
  > - analyzing the automation feasibility
- deliverables
  > - RTM
  > - automation feasibility report

### 3.2 test planning

> answers the question `what to test?`

- activities
  > - prepare test plan/strategy document
  > - test tool selection
  > - test effort estimation
  > - determine roles and responsibilities
- deliverables
  > - test plan/strategy document
  > - effort estimation

### 3.3 test case development

    >  creation and verification of test cases

- activities
  > - create test cases
  > - review the baseline testcases
  > - create test data
- deliverables
  > - test cases
  > - test data

### 3.4 environment setup

- activities
  > - prepare hardware and software
  > - setup environment
  > - perform smoke test
- deliverables
  > - environment ready
  > - smoke test result

### 3.5 test execution

- activities
  > - execute test cases
  > - document the test results
  > - map defects to test cases in RTM
  > - track defects to closure
- deliverables
  > - completed RTM
  > - testcases updated with results
  > - defect report

### 3.6 test cycle closure

> testing team meat, discuss and analyze the artifacts

- activities
  > - evaluate cycle completion criteria based on time, test coverage, cost, ...
  > - prepare test metrics
  > - prepare test closure
  > - find the defect distribution by type and severity
- deliverables
  > - test closure report
  > - test metrics

## 4. Mention three entry and three exit criteria.

>>  - `entry criteria`
>>   > - testing environment is available
>>   > - testable code is ready
>>   > - test data is ready
>>  - `exit criteria`
>>   > - test planned have been met
>>   > - not high severity defects
>>   > - high risk area are completely tested

## 5. Give an example on a test work product for each of the following test activities: test planning, monitoring, analysis, design, implementation, execution and completion.

> slides 30 

## 6. Explain three differences between test strategy and test plan.

1. **test strategy**
   > a high level document that capture the approach on how we go about testing and achieve the goal
   - `components`
     - scope
     - overview
     - test approach
     - testing tools
     - standards
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
     - staffing and training needs
   - by test lead or test manager
   - from the oriduct description (SRS), use case documents
   - dynamic document
   - at project level

## 7. What is meant by test procedure?

> the sequence of action for a test

## 8. Exercise: Specify scenario severity and priority (High Priority & High Severity , Low Priority & High Severity , High Priority & Low Severity , Low Priority & Low Severity)

1. Submit button is not working on a login page and customers are unable to login to the application.
2. Crash in some functionality which is going to deliver after couple of releases.
3. Spelling mistake of a company name on homepage.
4. FAQ page takes a long time to load.
5. Company logo or tagline issues.
6. On a bank website, an error message pops up when a customer clicks on transfer money button.
7. Font family or font size or color or spelling issue in the application or reports.

>> 1. High Priority & High Severity
>> 2. Low Priority & High Severity
>> 3. High Priority & Low Severity
>> 4. Low Priority & Low Severity
>> 5. High Priority & Low Severity
>> 6. High Priority & High Severity
>> 7. Low Priority & Low Severity

## 9. replace with key term

1. it is a management activity which approximates how long a task would take to complete.
2. estimating the test effort based on metrics of former similar projects or based on typical values.
3. estimating the test effort based on the experience of the owners of the testing tasks or by experts.
4. it is a quantitative measure of the degree to which a system, system component, or process possesses a given attribute.
5. minimum set of conditions that should be met (prerequisite items) before starting the software testing, used to determine when a given test activity should start.
6. it is concerned with summarizing information about testing effort, during and at the end of test activity/level.
7. they are the set of positive and negative executable steps of a test scenario which has a set of pre-conditions, test data, expected result, post-conditions and actual results.
8. ensure that users can perform appropriate actions when using valid data.
9. they are performed to try to “break” the software by performing invalid (or unacceptable) actions, or by using invalid data.
10. state the problem as clearly as possible so that developers can replicate the defect easily and fix it.
11. it can be defined as the impact/effect of the bug on the application. It can be Showstopper/Critical/High/Medium /Low.
12. it can be defined as an impact of the bug on the customers business. Main focus on how soon/urgent the defect should be fixed.
13. specifies the sequence of actions for a test, i.e. one or more Test Cases, list any initial preconditions and any activities following execution.
14. connects requirements to test cases throughout the validation process.
15. - It is a report that is created once the testing phase is successfully completed by meeting exit criteria defined for the project.
    - document that gives a summary of all the tests conducted.
    - gives a detailed analysis of the bugs removed and errors found.
    - presents the list of known issues.

>> 1. `Test Estimation`
>> 2. `Metrics based technique`
>> 3. `Expert based technique`
>> 4. `Metric`
>> 5. `Entry criteria`
>> 6. `Test reporting`
>> 7. `Test cases`
>> 8. `Positive test cases`
>> 9. `Negative test cases`
>> 10. `defect report`
>> 11. `Defect severity`
>> 12. `Defect priority`
>> 13. `test procedure`
>> 14. `Requirements Traceability Matrix (RTM)`
>> 15. `Test Closure Report`

## 10. Mention testing estimation techniques

1. PERT.
2. WBS (work breakdown structure).
3. wideband Delphi technique.
4. percentage distribution.
5. Expert-based technique.
6. metrics-based technique.

## 11. Mention Test strategy types

1. Analytical strategy.
2. Reactive strategy.
3. methodical strategy.
4. model-based strategy.
5. consultative strategy.
6. Regression averse strategy.
7. Process compliant strategy.

## 12. Mention the content of test procedure

1. Identifier.
2. Purpose.
3. Special requirements.
4. Procedure steps.
