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
_**Testing**_ can show failures which are caused by defects in the software. _**Debugging**_ is a defelopment activity which finds, analyses and fixes defects.

### 1.2 Why is Testing Necessary?
### FL-1.2.1 (K2) Exemplify why testing is necessary
Testing is necessary because it's a form of quality control. It helps achieve test objectives within constraints like scope, time, quality, and budget. While the test team performs many testing activities, anyone can use testing skills to help a project succeed. Testing components, systems, and documentation helps identify defects.

Testing contributes to project success in several ways:
* **Testing helps detect defects early and cost-effectively.** By identifying issues in requirements, design, or code, testing reduces the overall cost of fixing defects and improves the quality of the final product.
* **Testing provides insight into the quality of the system at different stages of development.** This information supports management decisions, such as whether to proceed to the next phase or to release the product.
* **Testing represents the users' perspective.** Testers help ensure that user needs are considered throughout development, especially when it’s not feasible to include real users directly in the process due to the high costs and lack of availability of suitable users.
* **Testing helps meet contractual, legal, or regulatory requirements.**

### FL-1.2.2 (K1) Recall the relation between testing and quality assurance
Testing and quality assurance (QA) are often confused but are not the same.

**Testing** is product-oriented and corrective. It's a major form of quality control, focusing on activities that support achieving quality levels. Other quality control methods include formal methods, simulation, and prototyping.

**QA** is process-oriented and preventive. It focuses on implementing and improving processes based on the idea that a good process produces a good product. QA applies to both development and testing processes and is everyone's responsibility.

Test results are used in both testing (to fix defects) and QA (to provide feedback on process performance).

### FL-1.2.3 (K2) Distinguish between root cause, error, defect, and failure
* **A root cause** is the fundamental reason a problem (like an error) occurred. Root cause analysis is used to identify these underlying reasons, aiming to prevent similar future errors or defects.
* **Errors (mistakes)** are made by humans.
* Errors produce **defects (faults, bugs).** Defects can be in documentation, code, or other work products.
* Defects, when executed, may result in **failures.** Failures occur when the system doesn't do what it should or does something it shouldn't.

Not all defects will cause a failure every time; some only fail in specific circumstances or may never fail. Failures can also be caused by environmental factors, not just defects.

Important Note: Defects found early in the SDLC, if not fixed, can lead to more defective work products later.

### 1.3 Testing Principles
### FL-1.3.1 (K2) Explain the seven testing principles
**1.	Testing shows the presence, not the absence of defects.** <br>
**2.	Exhaustive testing is impossible** – testing everything in feasible.<br>
**3.	Early testing saves time and money** – defects that are removed early in the process will not cause subsequent defects in derived work products. The cost of quality will be reduced since fewer failures will occur later in the SDLC.<br>
**4.	Defects cluster together** – a small number of system components usually contain most of the defects discovered or are responsible for most of the operational failures. This phenomenon is an illustration of the Pareto principle.<br>
**5.	Tests wear out** – if the same tests are repeated many times, they become increasingly ineffective in detecting new defects. To overcome this effect, existing tests and test data may need to be modified, and new tests may need to be written.<br>
**6.	Testing is context dependent** – there is no single universally applicable approach to testing. Testing is done differently in different contexts.<br>
**7.	Absence-of-defects fallacy** – thoroughly testing all the specified requirements and fixing all the defects found could still produce a system that does not fulfil the users’ needs and expectations.

### 1.4 Test Activities, Testware and Test Roles
### FL-1.4.1 (K2) Explain the different test activities and related tasks
* **Test planning.** Defines test objectives and selects the test approach based on the context and constraints.
* **Test monitoring and test control.** Monitors test progress and takes corrective actions to stay on track.
* **Test Analysis.** Identifies testable features and test conditions from the test basis; answers what to test.
* **Test Design.** Transforms test conditions into test cases and other testware, defines test data, and designs the test environment; answers how to test.
* **Test Implementation** – prepares and organizes the testware and sets up the test environment for execution.
* **Test Execution** – runs the tests, logs results, compares actual vs. expected outcomes, and analyzes anomalies.
* **Test Completion** – finalizes testing activities, reports remaining issues, archives useful assets, and captures lessons learned.

### FL-1.4.2 (K2) Explain the impact of context on the test process
Testing doesn't happen in isolation; it's part of the overall development process. The way testing is done is influenced by various contextual factors:
* **Stakeholders** (needs, expectations, cooperation)
* **Team members** (skills, knowledge, experience, availability)
* **Business domain** (criticality, risks, market needs, regulations)
* **Technical factors** (software type, architecture, technology)
* **Project constraints** (scope, time, budget, resources)
* **Organizational factors** (structure, policies, practices)
* **Software development lifecycle** (methods, practices)
* **Tools** (availability, usability)

These factors affect aspects like the test strategy, test techniques, test automation level, testware detail, and test reporting.

### FL-1.4.3 (K2) Differentiate the testware that supports the test activities
Testware refers to the work products created from the test activities. Examples of testware include:
* **Test planning work products:** test plan, test schedule, risk register, entry criteria and exit criteria.
* **Test monitoring and test control work products:** test progress reports, control directives documentation, risk information.
* **Test analysis work products:** (prioritized) test conditions (e.g., acceptance criteria), defect reports for defects in the test basis.
* **Test design work products:** (prioritized) test cases, test charters, coverage items, test data requirements, test environment requirements.
* **Test implementation work products:** test procedures, manual and automated test scripts, test suites, test data, test execution schedule, test environment items (e.g., stubs, drivers, simulators, service virtualizations).
* **Test execution work products:** test logs, defect reports.
* **Test completion work products:** test completion report, action items for improvement, documented lessons learned, change requests.

### FL-1.4.4 (K2) Explain the value of maintaining traceability
To effectively monitor and control testing, it's crucial to maintain traceability between elements in the test basis (e.g., requirements, user stories), associated testware (test conditions, risks, test cases), test results, and defects.

Good traceability is valuable because it:

* Supports coverage evaluation, especially if measurable coverage criteria are defined in the test basis. These criteria act as KPIs for achieving test objectives. For example, tracing test cases to requirements shows coverage of requirements.
* Helps evaluate the level of residual risk by tracing test results to risks.
* Makes it possible to determine the impact of changes.
* Facilitates audits and meeting IT governance criteria.
* Makes test progress and completion reports easier to understand for stakeholders by showing the status of test basis elements.
* Provides information to assess product quality, process capability, and project progress against business goals.

### FL-1.4.5 (K2) Compare the different roles in testing
This syllabus covers two main roles in testing: a test management role and a testing role. The tasks assigned to these roles depend on the project context, team skills, and organization.

* **The test management role** has overall responsibility for the test process, team, and leadership. They focus on test planning, monitoring, control, and completion. In Agile, some tasks may be done by the team, while others (spanning multiple teams or the organization) may be done by test managers outside the team.
* **The testing role** is responsible for the engineering/technical aspects of testing, focusing on test analysis, design, implementation, and execution.

These roles can be performed by different people or one person, depending on the context. For example, a team leader, test manager, or development manager could fill the test management role.

### 1.5 Essential Skills and Good Practices in Testing
### FL-1.5.1 (K2) Give examples of the generic skills required for testing
While many skills are valuable, some are particularly important for testers:
* **Testing knowledge:** Using test techniques effectively.
* **Thoroughness, carefulness, curiosity, attention to details, being methodical:** Finding defects, especially hard-to-find ones.
* **Good communication skills, active listening, being a team player:** Interacting effectively with stakeholders, conveying information, reporting defects constructively.
* **Analytical thinking, critical thinking, creativity:** Increasing testing effectiveness.
* **Technical knowledge:** Increasing testing efficiency (e.g., using tools).
* **Domain knowledge:** Understanding and communicating with users/business representatives.

Testers often deliver bad news, making communication skills critical. Information about defects should be communicated constructively to avoid defensiveness and confirmation bias.

### FL-1.5.2 (K1) Recall the advantages of the whole team approach
In the **whole team approach** any team member with the necessary knowledge and skills can perform any task, and everyone is responsible for quality. The team members share the same workspace (physical or virtual), as co-location facilitates communication and interaction.

Benefits include improved team dynamics, enhanced communication/collaboration, and synergy.

### FL-1.5.3 (K2) Distinguish the benefits and drawbacks of independence of testing
A certain level of **independence of testing** can make testers more effective at finding defects due to different cognitive biases than the author. However, independence doesn't replace familiarity; developers can efficiently find defects in their own code.

Degrees of independence:
No independence: Tested by the author.
Some independence: Tested by peers from the same team.
High independence: Tested by testers from outside the author's team but within the organization.
Very high independence: Tested by testers from outside the organization.
For most projects, multiple levels of independence are best (e.g., developers doing component testing, test team doing system testing, business representatives doing acceptance testing).

**Benefits of independence:**
Independent testers are more likely to find different types of defects due to different backgrounds, perspectives, and biases.
Independent testers can challenge assumptions made during specification and implementation.

**Drawbacks of independence:**
Isolation from the development team can lead to poor collaboration, communication problems, or adversarial relationships.
Developers might lose a sense of responsibility for quality.
Independent testers can be seen as a bottleneck or blamed for delays.

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
