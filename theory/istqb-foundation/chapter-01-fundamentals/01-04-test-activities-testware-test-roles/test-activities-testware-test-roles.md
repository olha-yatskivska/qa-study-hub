# 📋 Test Process: Activities, Testware and Roles
(Based on ISTQB v4.0 & ISO/IEC/IEEE 29119-2)

Although these activities may appear to follow a logical sequence, they are often implemented iteratively or in parallel (especially in Agile). 


| **Test Stages** | **Core Activity (Goal)** | **Testware** (Work Products) | **Test roles** |
| :--- | :--- | :--- |:--- |
| 📍 **Test planning**| Defining the test objectives and selecting an approach to achieve them | 📄 Test Plan, Test Schedule, Risk Register, Entry/Exit Criteria.  | 👤Test Management |
| 📊 **Test monitoring and control**| Checking progress against the plan (Monitoring) and taking corrective actions (Control). In Agile: repeated every sprint| 📈 Test Progress Reports (Daily in Agile), documentation of Control Directives and Risk updates| 👤 Test Management |
| 🔍 **Test analysis**| **What to test?** Analyzing the test basis to identify testable features. Define and  prioritize **Test Conditions**, together with the related risks and risk levels. Static testing for test basis. Activity supported by the use of test techniques | 📑Prioritized Test Conditions (e.g., Acceptance Criteria), Defect Reports regarding defects in the test basis (if not fixed directly) | 🛠️ The Testing Role |
| 🎨 **Test design**| **How to test?** Elaborating the test conditions into test cases and other testware (decision table, diagram, test charter), identification of coverage items, which serve as a guide to specify test case inputs. Test techniques can be used. Includes defining the test data requirements, designing in test enviroment and identifying any other required infrastucture and  tools  | Prioritized Test Cases, Test Charters, Coverage Items, Test Data & Test Environment requirements | 🛠️ The Testing Role   |
| ⚙️ **Test implementation**| **Is everything ready?** Creating the testware necessary for test execution (test data). Test cases can be organized into test procedures and are often assembled into test suites. Manualand automated test scripts are created. The test enviroment is built and verified to be set up correctly. Test procedures are prioritized and arranged within a test execution schedule for efficient test execution | 🏗️ Test Procedures, Automated Test Scripts, Test Suites, Test Data, Test Execution Schedule, Test Enviroment Elements (e.g., stubs, drivers, simulations, and service virtualizations).  | 🛠️ The Testing Role   |
|🚀 **Test execution**| Running the tests (manual or automated) in accordance with the test execution schedule (test runs). Actual test results are compared with the expected results. the test results are logged. Anomalies are analyzed to identify their likely causes.| 📓 Test logs, Defect reports (Bugs)|  🛠️ The Testing Role   |
| 🏁 **Test completion**|Occurs at project milestone (e.g, release, end of iteration, test level complition) for any unresolved defects, change requests or product backlog items created. The test enviroment is shut down to an agreed state. The test activities are analyzed to identify lessons learned and improvements for future iterations, releases, or projects. A Test complition report is created and communicated to the stakeholders. For Scrum team: retro, demo, sprint review, * demo = test summary report as meeting. | 🏁 Test Completion Report, Action Items for improvement of subsequent projects or iterations, Documanted Lessons Learned, and Change Requests (e.g., as product Backlog Items) | 👤 Test Management |

---
## 🎓 Why this is critical for a Test Analyst
* **Early Value (Analysis):** You prevent "bugs in requirements" by performing static testing during the Analysis phase. Identifying a flaw in a User Story is significantly cheaper than finding it during execution.

* **Strategic Coverage (Design):** You ensure that High-level Test Cases cover all test conditions. Your expertise in test techniques (like Decision Tables or Boundary Value Analysis) ensures maximum coverage with minimum test cases.

* **Efficiency (Implementation):** By prioritizing Test Procedures and organizing Test Suites, you ensure that the most critical tests are run first, providing fast feedback to the team.

* **Traceability:** You bridge the gap between "Business Requirements" and "Technical Execution," making sure that the final Test Completion report actually proves the software is ready for the user.

* **Agile Context:** Demo sessions act as a "live" Test Summary Report for stakeholders.

* **Static Testing:** Happens primarily during the Test Analysis phase when you review the Test Basis.

* **Testware Archiving:** During Test Completion, ensure that automated scripts and data are saved for future regression.
