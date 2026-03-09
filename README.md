# Leave Management System - Power Apps

A leave management solution built using Microsoft Power Apps and Power Automate within the Microsoft 365 ecosystem.

The application allows employees to submit leave requests, managers to approve or reject requests, and administrators to manage leave balance and company holidays. 

## Technologies
- Microsoft Power Apps (Canvas)
- Power Automate ([See full Power Automate flow here](screenshots/all-flow.png))
- SharePoint
- Microsoft 365

## Key Features
- Leave request submission with automatic duration calculation
- Weekend and public holiday exclusion
- Overlap validation for leave requests
- Manager approval workflow
- Email notifications for approvals, rejections, and adjustments
- Leave balance tracking and automatic balance restoration

## Screenshots
### Dashboard
![Dashboard](screenshots/dashboard-overview.jpg)
The main dashboard displays the employee’s leave balances and a list of submitted leave requests. Each request includes options to **view detailed information or cancel the request**. Cancellation is only allowed if the leave has been approved and the start date is more than 48 hours away.
### Leave Request Form
![Form](screenshots/date-validation.jpg)
The leave request form automatically calculates the **leave duration while excluding weekends and public holidays.** The system also detects overlapping requests and displays a notification if the selected dates already have an existing request with the status **Pending (Level 1), Pending (Level 2), or Approved.**
### Team Calendar
![Calendar](screenshots/team-calendar.jpg)
This page shows a weekly leave calendar for employees within the same department, allowing team members to quickly see who is on leave. On the **administrator view**, the calendar displays leave schedules for **all employees across departments.**
### Approval Workflow & Conflict Awareness
![Approval](screenshots/approval-flow.jpg)
When an employee submits a leave request, the system checks whether the dates overlap with other employees’ leave within the same department. This information is shown as **FYI context for the approver** in the Microsoft approval interface. Once approved, the leave entry is automatically **added to the Microsoft Teams calendar.**
### Approval History
![Approval HIstory](screenshots/approval-history.jpg)
Managers can review all leave requests that have been sent to them through the **approval history page**. The records can also be **exported as a PDF file for documentation or reporting purposes.**
