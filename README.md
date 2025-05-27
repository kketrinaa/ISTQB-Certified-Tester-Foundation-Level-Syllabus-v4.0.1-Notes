# ISTQB Certified Tester Foundation Level Syllabus (v4.0.1) Notes

## 1. Fundamentals of Testing
### 1.1 What is Testing?
### FL-1.1.1 (K1) Identify typical test objectives
The typical test objectives are:
* Evaluating work products such as requirements, user stories, designs, and code
* Causing failures and finding defects
* Ensuring required coverage of a test object
* Reducing the risk level of inadequate software quality
* Verifying whether specified requirements have been fulfilled
* Verifying that a test object complies with contractual, legal, and regulatory requirements
* Providing information to stakeholders to allow them to make informed decisions
* Building confidence in the quality of the test object
* Validating whether the test object is complete and works as expected by the stakeholders
### FL-1.1.2 (K2) Differentiate testing from debugging
Testing can show failures which are caused by defects in the software. Debugging is a defelopment activity which finds, analyses and fixes defects.

### 1.2 Why is Testing Necessary?
### FL-1.2.1 (K2) Exemplify why testing is necessary
* _**Testing helps detect defects early and cost-effectively.**_ By identifying issues in requirements, design, or code, testing reduces the overall cost of fixing defects and improves the quality of the final product.
* _**Testing provides insight into the quality of the system at different stages of development.**_ This information supports management decisions, such as whether to proceed to the next phase or to release the product.
* _**Testing represents the users' perspective.**_ Testers help ensure that user needs are considered throughout development, especially when it’s not feasible to include real users directly in the process due to the high costs and lack of availability of suitable users.
* _**Testing helps meet contractual, legal, or regulatory requirements.**_

### FL-1.2.2 (K1) Recall the relation between testing and quality assurance
_**Testing**_ is a product-oriented, *corrective* activity that focuses on finding defects and verifying software quality. _**Quality Assurance (QA)**_ is a process-oriented, *preventive* activity that focuses on improving and following development and testing processes. QA applies to both the development and testing processes, and is the responsibility of everyoneon a project. In testing test results are used to fix defects, while in QA to improve processes.
### FL-1.2.3 (K2) Distinguish between root cause, error, defect, and failure
* _**Root Cause:**_ A source of a defect. If it's removed, the defect happens less often or disappears.
* _**Error (Mistake):**_ A human action that results in a defect.
* _**Defect (Bug, Fault):**_ A flaw in a work product that makes it not meet requirements or affects how it's supposed to function.
* _**Failure:**_ System event triggered by a specific defect (not all defects may always cause failure).

### 1.3 Testing Principles
### FL-1.3.1 (K2) Explain the seven testing principles
_**1.	Testing shows the presence, not the absence of defects.**_ <br>
_**2.	Exhaustive testing is impossible**_ – testing everything in feasible.<br>
_**3.	Early testing saves time and money**_ – defects that are removed early in the process will not cause subsequent defects in derived work products. The cost of quality will be reduced since fewer failures will occur later in the SDLC.<br>
_**4.	Defects cluster together**_ – a small number of system components usually contain most of the defects discovered or are responsible for most of the operational failures. This phenomenon is an illustration of the Pareto principle.<br>
_**5.	Tests wear out**_ – if the same tests are repeated many times, they become increasingly ineffective in detecting new defects. To overcome this effect, existing tests and test data may need to be modified, and new tests may need to be written.<br>
_**6.	Testing is context dependent**_ – there is no single universally applicable approach to testing. Testing is done differently in different contexts.<br>
_**7.	Absence-of-defects fallacy**_ – thoroughly testing all the specified requirements and fixing all the defects found could still produce a system that does not fulfil the users’ needs and expectations.

### 1.4 Test Activities, Testware and Test Roles
### FL-1.4.1 (K2) Explain the different test activities and related tasks
* _**Test planning.**_ Defines test objectives and selects the test approach based on the context and constraints.
* _**Test monitoring and test control.**_ Monitors test progress and takes corrective actions to stay on track.
* _**Test Analysis.**_ Identifies testable features and test conditions from the test basis; answers what to test.
* _**Test Design.**_ Transforms test conditions into test cases and other testware, defines test data, and designs the test environment; answers how to test.
* _**Test Implementation**_ – prepares and organizes the testware and sets up the test environment for execution.
* _**Test Execution**_ – runs the tests, logs results, compares actual vs. expected outcomes, and analyzes anomalies.
* _**Test Completion**_ – finalizes testing activities, reports remaining issues, archives useful assets, and captures lessons learned.

### FL-1.4.2 (K2) Explain the impact of context on the test process
Testing is not performed in isolation. Testing is also funded by stakeholders and its final goal is to help fulfill the stakeholders’ business needs. The way the testing is carried out will depend on a number of contextual factors including:
* Stakeholders (needs, expectations, requirements, willingness to cooperate, etc.)
* Team members (skills, knowledge, level of experience, availability, training needs, etc.)
* Business domain (criticality of the test object, identified risks, market needs, specific legal regulations, etc.)
* Technical factors (type of software, product architecture, technology used, etc.)
* Project constraints (scope, time, budget, resources, etc.)
* Organizational factors (organizational structure, existing policies, practices used, etc.)
* Software development lifecycle (engineering practices, development methods, etc.)
* Tools (availability, usability, compliance, etc.)

These factors will have an impact on many test-related issues, including: test strategy, test techniques used, degree of test automation, required level of coverage, level of detail of testware, test reporting, etc.

### FL-1.4.3 (K2) Differentiate the testware that supports the test activities
Testware refers to all work products produced during test activities. Each test activity creates specific testware:
* _**Test planning work products**_ include: test plan, test schedule, risk register, entry criteria and exit criteria. Risk register is a list of risks together with risk likelihood, risk impact and information about risk mitigation. Test schedule, risk register, entry criteria and exit criteria are often a part of the test plan.
* _**Test monitoring and test control work products**_ include: test progress reports, documentation of control directives and information about risks.
* _**Test analysis work products**_ include: (prioritized) test conditions (e.g., acceptance criteria), and defect reports regarding defects in the test basis (if not fixed directly).
* _**Test design work products**_ include: (prioritized) test cases, test charters, coverage items, test data requirements and test environment requirements.
* _**Test implementation work products**_ include: test procedures, manual and automated test scripts, test suites, test data, test execution schedule, and test environment items. Examples of test environment items include: stubs, drivers, simulators, and service virtualizations.
* _**Test execution work products**_ include: test logs, and defect reports.
* _**Test completion work products**_ include: test completion report, action items for improvement of subsequent projects or iterations, documented lessons learned, and change requests (e.g., as product backlog items).

### FL-1.4.4 (K2) Explain the value of maintaining traceability
Maintaining traceability throughout the test process provides a clear link between the _test basis_ (e.g., requirements, risks), the related _testware_ (test conditions, test cases), _test results_, and _defects_.

In addition to evaluating coverage, good traceability makes it possible to determine the impact of changes, facilitates audits, and helps meet IT governance criteria. Good traceability also makes test progress reports and test completion reports more easily understandable by including the status of test basis elements. This can also assist in communicating the technical aspects of testing to stakeholders in an understandable manner.

Traceability ensures transparency, improves control, and supports better decision-making throughout the test process. Traceability provides information to assess product quality, process capability, and project progress against business goals.

### FL-1.4.5 (K2) Compare the different roles in testing
_**1.	The test management role**_ takes overall responsibility for the test process, test team and leadership of the test activities. The test management role is mainly focused on the activities of test planning, test monitoring, test control and test completion.

_**2.	The testing role**_ takes overall responsibility for the engineering (technical) aspect of testing. The testing role is mainly focused on the activities of test analysis, test design, test implementation and test execution.

Different people may take on these roles at different times. For example, the test management role can be performed by a team leader, by a test manager, by a development manager, etc. It is also possible for one person to take on the roles of testing and test management at the same time.

### 1.5 Essential Skills and Good Practices in Testing
### FL-1.5.1 (K2) Give examples of the generic skills required for testing
While being generic, the following skills are particularly relevant for testers:
* Testing knowledge (to increase effectiveness of testing, e.g., by using test techniques)
* Thoroughness, carefulness, curiosity, attention to details, being methodical (to identify defects, especially the ones that are difficult to find)
* Good communication skills, active listening, being a team player (to interact effectively with all stakeholders, to convey information to others, to be understood, and to report and discuss defects)
* Analytical thinking, critical thinking, creativity (to increase effectiveness of testing)
* Technical knowledge (to increase efficiency of testing, e.g., by using appropriate test tools)
* Domain knowledge (to be able to understand and to communicate with end users/business representatives)

### FL-1.5.2 (K1) Recall the advantages of the whole team approach
In _the whole team approach_ any team member with the necessary knowledge and skills can perform any task, and everyone is responsible for quality. The team members share the same workspace (physical or virtual), as co-location facilitates communication and interaction.

The whole team approach improves: team dynamics, enhances communication and collaboration within the team, and creates synergy by allowing the various skill sets within the team to be leveraged for the benefit of the project.

### FL-1.5.3 (K2) Distinguish the benefits and drawbacks of independence of testing
Work products can be tested by their author (no independence), by the author's peers from the same team (some independence), by testers from outside the author's team but within the organization (high independence), or by testers from outside the organization (very high independence).

_**Benefits of independent testing:**_
* Independent testers are more likely to uncover different defects due to their different perspectives and cognitive biases.
* They can challenge assumptions made during development and provide an objective view of the system.
* Multiple levels of independence (e.g., developers testing components, testers testing the system) can improve overall test effectiveness.

_**Drawbacks of independent testing:**_
* Independent testers may become isolated from the development team, reducing collaboration and creating communication issues.
* It can lead to an adversarial mindset, where developers and testers are seen as being in opposition.
* Developers might lose a sense of ownership over product quality.
* Independent testers may be viewed as bottlenecks or even blamed for delays in delivery.

<br>

## 2. Testing Throughout the Software Development Lifecycle
### 2.1 Testing in the Context of a Software Development Lifecycle
### FL-2.1.1 (K2) Explain the impact of the chosen software development lifecycle on testing
### FL-2.1.2 (K1) Recall good testing practices that apply to all software development lifecycles
### FL-2.1.3 (K1) Recall the examples of test-first approaches to development
### FL-2.1.4 (K2) Summarize how DevOps might have an impact on testing
### FL-2.1.5 (K2) Explain shift left
### FL-2.1.6 (K2) Explain how retrospectives can be used as a mechanism for process improvement
<br>

### 2.2 Test Levels and Test Types
### FL-2.2.1 (K2) Distinguish the different test levels
### FL-2.2.2 (K2) Distinguish the different test types
### FL-2.2.3 (K2) Distinguish confirmation testing from regression testing
<br>

### 2.3 Maintenance Testing
### FL-2.3.1 (K2) Summarize maintenance testing and its triggers 
<br>

## 3. Static Testing
### 3.1 Static Testing Basics
### FL-3.1.1 (K1) Recognize types of work products that can be examined by static testing
### FL-3.1.2 (K2) Explain the value of static testing
### FL-3.1.3 (K2) Compare and contrast static testing and dynamic testing
<br>

### 3.2 Feedback and Review Process
### FL-3.2.1 (K1) Identify the benefits of early and frequent stakeholder feedback
### FL-3.2.2 (K2) Summarize the activities of the review process
### FL-3.2.3 (K1) Recall which responsibilities are assigned to the principal roles when performing reviews
### FL-3.2.4 (K2) Compare and contrast the different review types
### FL-3.2.5 (K1) Recall the factors that contribute to a successful review
<br>

## 4. Test Analysis and Design
### 4.1 Test Techniques Overview
### FL-4.1.1 (K2) Distinguish black-box test techniques, white-box test techniques and experience-based test techniques
<br>

### 4.2 Black-box Test Techniques
### FL-4.2.1 (K3) Use equivalence partitioning to derive test cases
### FL-4.2.2 (K3) Use boundary value analysis to derive test cases
### FL-4.2.3 (K3) Use decision table testing to derive test cases
### FL-4.2.4 (K3) Use state transition testing to derive test cases
<br>

### 4.3 White-box Test Techniques
### FL-4.3.1 (K2) Explain statement testing
### FL-4.3.2 (K2) Explain branch testing
### FL-4.3.3 (K2) Explain the value of white-box testing
<br>

### 4.4 Experience-based Test Techniques
### FL-4.4.1 (K2) Explain error guessing
### FL-4.4.2 (K2) Explain exploratory testing
### FL-4.4.3 (K2) Explain checklist-based testing
<br>

### 4.5. Collaboration-based Test Approaches
### FL-4.5.1 (K2) Explain how to write user stories in collaboration with developers and business representatives
### FL-4.5.2 (K2) Classify the different options for writing acceptance criteria
### FL-4.5.3 (K3) Use acceptance test-driven development (ATDD) to derive test cases 
<br>

## 5. Managing the Test Activities
### 5.1 Test Planning
### FL-5.1.1 (K2) Exemplify the purpose and content of a test plan
### FL-5.1.2 (K1) Recognize how a tester adds value to iteration and release planning
### FL-5.1.3 (K2) Compare and contrast entry criteria and exit criteria
### FL-5.1.4 (K3) Use estimation techniques to calculate the required test effort
### FL-5.1.5 (K3) Apply test case prioritization
### FL-5.1.6 (K1) Recall the concepts of the test pyramid
### FL-5.1.7 (K2) Summarize the testing quadrants and their relationships with test levels and test types
<br>

### 5.2 Risk Management
### FL-5.2.1 (K1) Identify risk level by using risk likelihood and risk impact
### FL-5.2.2 (K2) Distinguish between project risks and product risks
### FL-5.2.3 (K2) Explain how product risk analysis may influence thoroughness and test scope
### FL-5.2.4 (K2) Explain what measures can be taken in response to analyzed product risks
<br>

### 5.3 Test Monitoring, Test Control and Test Completion
### FL-5.3.1 (K1) Recall metrics used for testing
### FL-5.3.2 (K2) Summarize the purposes, content, and audiences for test reports
### FL-5.3.3 (K2) Exemplify how to communicate the status of testing
<br>

### 5.4 Configuration Management
### FL-5.4.1 (K2) Summarize how configuration management supports testing
<br>

### 5.5 Defect Management
### FL-5.5.1 (K3) Prepare a defect report
<br>

## 6. Test Tools
### 6.1 Tool Support for Testing
### FL-6.1.1 (K2) Explain how different types of test tools support testing
<br>

### 6.2 Benefits and Risks of Test Automation
### FL-6.2.1 (K1) Recall the benefits and risks of test automation
