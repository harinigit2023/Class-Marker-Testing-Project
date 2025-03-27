**Title Page**

* **Project Name:** *Online Exam & Proctoring System Testing*  
* **Document Version:** *V1.0*  
* **Created By:** ADURI N V S SAMRUTA LALITHA HARINI  
* **Date:** *March 2025*

***DOCUMENTATION:***

**Online Exam & Proctoring System Testing Document**  
**1\. Test Scenarios**  
**Functional Testing:**

* Verify user registration and login functionality.  
* Check OTP-based authentication for exam access.  
* Validate exam start, pause, and resume features.  
* Ensure questions load dynamically based on the selected subject.  
* Verify auto-submission of the exam upon time completion.  
* Ensure correct calculation of exam scores.  
* Validate exam result generation and report download.

Security Testing

* Test unauthorized access attempts.  
* Verify encryption of user credentials.  
* Check data privacy policies for user details.  
* Test webcam and screen recording security measures.

Database Testing

* Verify if exam responses are stored correctly in the database.  
* Ensure database integrity for registered users and exam results.  
* Validate query performance for large exam data.

API Testing

* Validate user authentication API.  
* Check API response time for exam submission.  
* Verify API security for fetching user data.

**Sample Test Scenarios:**

| Scenario ID | Test Scenario |
| :---- | :---- |
| **TS01** | Verify that a student can successfully register for an online exam. |
| **TS02** | Verify that a student can log in using valid credentials. |
| **TSO3** | Verify that the system sends an OTP for authentication when logging in. |
| **TS04** | Verify that a student cannot log in with invalid credentials. |
| **TS05** | Verify that a student can start the exam only after logging in successfully |
| **TS06** | Verify that the exam timer starts immediately after the test begins. |
| **TS07** | Verify that the student cannot switch tabs without being flagged. |
| **TS08** | Verify that the exam auto-submits when the timer reaches zero. |
| **TS09** | Verify that the questions are displayed in a random order for different users. |
| **TS10** | Verify that the student receives a warning if the webcam is turned off. |
| **TS11** | Verify that the exam is auto-submitted if the student gets disconnected. |
| **TS12** | Verify that the results are displayed only after exam submission. |
| **TS13** | Verify that the admin can create, edit, and delete questions. |
| **TS14** | Verify that students cannot retake the exam unless allowed**.** |
| **TS15** | Verify that students get a confirmation message before submitting the exam. |

**2\. Test Cases**

| Test Case ID | Test Scenario | Steps to Execute | Expected Result | Status |
| :---- | :---- | :---- | :---- | :---- |
| TC001 | Verify login with valid credentials | Enter email & password, click login | User logs in successfully | Pending |
| TC002 | Validate OTP authentication | Enter correct OTP after login | Redirects to dashboard | Pending |
| TC003 | Ensure the webcam is working before starting the exam | Click "Start Exam" | Webcam preview should appear | Pending |
| TC004 | Verify exam submission on time completion | Attempt exam, wait for timer to end | Exam auto-submits | Pending  |

**3\. Test Plan**  
**Objective:**  
To ensure the Online Exam & Proctoring System functions correctly, securely, and efficiently.  
**Scope:**

* Functional, Security, Database, API testing  
* In-Scope: User authentication, exam process, results  
* Out of Scope: Payment gateways, third-party integrations

**Roles & Responsibilities:**

* Test Engineer: Writing and executing test cases  
* Developer: Fixing bugs based on reports  
* Project Manager: Overseeing testing progress


**Testing Tools:**

* JIRA (Test Management)  
* Postman (API Testing)  
* MySQL (Database Validation)

**Schedule:**

| Activity | Start Date | End Date |
| :---- | :---- | :---- |
| Test Case Creation | March 18, 2025 | March 20, 2025 |
| Test Execution | March 21, 2025 | March 25, 2025 |
| Bug Reporting & Fixing | March 26, 2025 | March 28, 2025 |

**4\. Requirement Traceability Matrix (RTM):**

| Requirement ID | Test Case ID | Status |
| :---- | :---- | :---- |
| REQ001 (User Login) | TC001, TC002 | Pending |
| REQ002 (Exam Submission) | TC004 | Pending |
| REQ003 (Result Generation) | TC005 | Pending |

**5\. Test Strategy**  
Test Approach: Agile-based testing, with frequent bug fixes.  
Entry Criteria: Application is stable for testing, all test cases written.  
Exit Criteria: All high-priority test cases executed, critical bugs fixed.  
Risks & Assumptions: Users must have stable internet and webcam access.

**6\. Test Data:**

| Test Data Type | Sample Data |
| :---- | :---- |
| User Email | testuser@example.com |
| Password | Test@123 |
| OTP Code | 123456 |
| Exam Name | Java Programming |
| Exam Score | 80/100 |

**7\. Bug Report:**

| Bug ID | Description | Severity | Status |
| :---- | :---- | :---- | :---- |
| BUG001 | Login fails with valid credentials | Critical | Open |
| BUG002 | Webcam not detected on some browsers | high | open |
| BUG003 | Incorrect score calculation | High | Open |

**8\. Test Execution Report:**

| Test Case ID | Execution Status | Bug ID (If Any) |
| :---- | :---- | :---- |
| TC001 | Passed |  |
| TC002 | Failed | BUG001 |
| TC003 | Passed |  |
| TC004 | Failed | BUG003 |

