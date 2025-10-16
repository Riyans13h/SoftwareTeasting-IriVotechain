# Test Plan for Student Attendance System

## 1. Objective
The objective of this test plan is to verify the functionality, reliability, and performance of the Student Attendance System. The system should allow teachers and administrators to mark attendance, generate reports, and manage student data efficiently.

## 2. Scope
This test plan covers the following features:
- Attendance marking (daily, bulk, and edit)
- Report generation (PDF, CSV, analytics dashboard)
- Notifications (email alerts for absentees)
- User management (role-based access for teachers and admins)
- System login and authentication
- Data backup and restore

## 3. Test Environment
- Operating System: Windows 10 / Linux / macOS
- Browser: Chrome / Firefox / Edge (latest versions)
- Internet connection required
- Database: MySQL or PostgreSQL

## 4. Test Cases

### 4.1 Login Functionality
| Test Case ID | Description | Expected Result | Status |
|--------------|-------------|----------------|--------|
| TC_LOGIN_01  | Login with valid credentials | User should be redirected to dashboard | Pending |
| TC_LOGIN_02  | Login with invalid credentials | Display error message | Pending |
| TC_LOGIN_03  | Forgot Password functionality | Reset link should be sent via email | Pending |

### 4.2 Attendance Marking
| Test Case ID | Description | Expected Result | Status |
|--------------|-------------|----------------|--------|
| TC_ATT_01    | Mark attendance for a single student | Attendance should be saved | Pending |
| TC_ATT_02    | Mark attendance for all students | All records updated | Pending |
| TC_ATT_03    | Edit attendance | Changes should be saved | Pending |

### 4.3 Report Generation
| Test Case ID | Description | Expected Result | Status |
|--------------|-------------|----------------|--------|
| TC_REP_01    | Generate daily report | Correct attendance data exported | Pending |
| TC_REP_02    | Generate monthly report | Report should summarize all attendance | Pending |
| TC_REP_03    | Export report as PDF | PDF file should download successfully | Pending |

### 4.4 Notifications
| Test Case ID | Description | Expected Result | Status |
|--------------|-------------|----------------|--------|
| TC_NOT_01    | Send email notification for absent students | Emails delivered | Pending |
| TC_NOT_02    | Disable notifications | No emails should be sent | Pending |

### 4.5 User Management
| Test Case ID | Description | Expected Result | Status |
|--------------|-------------|----------------|--------|
| TC_USER_01   | Add new student | Student record saved successfully | Pending |
| TC_USER_02   | Edit student information | Changes saved successfully | Pending |
| TC_USER_03   | Delete student | Student record removed | Pending |

## 5. Version Control Observations
- Multiple users can edit the document simultaneously in HackMD / CodeCollab.
- Real-time updates appear instantly.
- Version history allows reverting unwanted changes.
- Conflicts are handled automatically; the last edit is applied in case of simultaneous edits on the same line.

## 6. Notes
- Ensure proper backup of the test plan.
- Review all test cases before executing them.
- Update the test plan if new features are added to the system.
