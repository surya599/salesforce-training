# Day 4 - Flow Builder

## 1. What is Flow Builder?

Flow Builder is a declarative automation tool in Salesforce used to automate business processes without writing code.

It helps users create workflows by using drag-and-drop elements to:

- Collect data
- Update records
- Send emails
- Create approvals
- Display screens
- Automate repetitive tasks

Flow Builder improves efficiency and reduces manual work in enterprise systems.

---

# 2. Types of Flows

## A. Screen Flow

A Screen Flow is used to collect input from users through screens.

### Features:
- Interactive user interface
- Collects user input
- Guides users step-by-step
- Can create or update records

### Example:
A student registration form where users enter:

- Name
- Email
- Course

The flow stores data automatically.

---

## B. Record Triggered Flow

A Record Triggered Flow runs automatically when a record is:

- Created
- Updated
- Deleted

### Features:
- Fully automated
- Runs in background
- No user interaction needed

### Example:
When a new Lead is created:

- Check matching account
- Notify account owner
- Send email to sales team

---

# 3. My Automation Ideas

## 1. Student Attendance Alert
When attendance drops below 75%, automatically send warning email.

---

## 2. Lead Assignment Automation
When a new lead is created, assign it to correct sales representative.

---

## 3. Library Due Date Reminder
Send automatic reminder email before due date.

---

## 4. Fee Payment Notification
Notify students when fee payment deadline approaches.

---

## 5. Support Ticket Escalation
If ticket is unresolved for 48 hours, escalate to manager.

---

# 4. My Flow Diagram

Flow Example: Lead Matching Automation

```plaintext
Start
   ↓
New Lead Created
   ↓
Check Matching Account
   ↓
Decision: Match Found?
   ↓ Yes
Update Account
   ↓
Post to Chatter
   ↓
Send Email Alert
   ↓
End

No → End
```



# 5. Manual vs Automated Process

| Manual Process | Automated Process |
|---------------|------------------|
| Takes more time | Fast execution |
| Human errors possible | Accurate results |
| Requires repeated effort | Runs automatically |
| Delayed notifications | Instant alerts |
| Hard to scale | Easy to scale |

---

# 6. Reflection: Why Automation Matters in Enterprise Systems

Automation is important because enterprise systems handle thousands of records daily.

Benefits:

- Saves time
- Reduces errors
- Improves productivity
- Ensures consistency
- Provides faster communication
- Helps organizations scale efficiently

Flow Builder makes automation simple and allows businesses to solve complex problems without coding.

It is a powerful tool for modern enterprise application development.

---

## Conclusion

Flow Builder is essential for Salesforce automation.

It helps automate repetitive business processes, improves efficiency, and makes enterprise systems smarter and faster.
