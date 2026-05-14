# Day 6 – SOQL and Apex Triggers

## Salesforce Summer Program – Day 6

---

# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is Salesforce’s query language used to retrieve data from Salesforce objects.

It is similar to SQL but designed specifically for Salesforce.

SOQL helps developers fetch records from objects like:

- Students
- Courses
- Faculty
- Attendance
- Payments

### Why SOQL is Important

SOQL allows systems to:

- Retrieve specific records
- Filter data
- Access related records
- Generate reports
- Support automation logic

### Example

Find all students with attendance below 75%.

SOQL helps retrieve this information automatically.

---

# 2. What is an Apex Trigger?

An Apex Trigger is code that runs automatically before or after changes happen to Salesforce records.

Triggers respond to events like:

- Insert
- Update
- Delete
- Undelete

Triggers help automate actions whenever data changes.

### Why Triggers are Needed

Triggers allow Salesforce to:

- Validate business rules
- Update related records
- Send notifications
- Automate reactions to events
- Enforce system logic

---

# 3. Difference Between Flow vs Trigger

| Feature | Flow | Apex Trigger |
|---------|------|--------------|
| Type | Declarative (No-code) | Programmatic (Code) |
| Development Style | Drag-and-drop | Coding |
| Complexity Handling | Moderate | High |
| Flexibility | Limited | Very High |
| Maintenance | Easier | Requires testing/debugging |
| Best For | Simple automation | Complex event logic |

---

# Before Trigger vs After Trigger

| Trigger Type | Purpose |
|-------------|---------|
| Before Trigger | Modify or validate data before saving |
| After Trigger | Perform actions after record is saved |

### Example

**Before Insert**

Validate if student email exists before saving.

**After Insert**

Send welcome email after student record is created.

---

# 4. Trigger Use Cases in College Management System

## Use Case 1: Welcome Email After Registration

### Event

After Student Record Insert

### Action

Automatically send welcome email.

### Why

Confirms successful registration.

---

## Use Case 2: Notify Faculty When Course Becomes Full

### Event

After Course Update

### Action

Notify assigned faculty.

### Why

Faculty needs enrollment status updates.

---

## Use Case 3: Attendance Warning

### Event

After Attendance Update

### Action

Notify student if attendance < 75%.

### Why

Helps students stay eligible.

---

## Use Case 4: Block Invalid Registration

### Event

Before Course Registration Insert

### Action

Prevent save if seats are full.

### Why

Maintains seat limits.

---

## Use Case 5: Scholarship Eligibility Recheck

### Event

After Semester Result Update

### Action

Recalculate scholarship eligibility.

### Why

Keeps scholarship status accurate.

---

# 5. Query Examples (English Query Thinking)

## Student Queries

- Find all students enrolled in Course A
- Find students with attendance below 75%
- Find students with unpaid fees

---

## Course Queries

- Find courses with available seats
- Find courses assigned to Faculty X
- Find full courses

---

## Faculty Queries

- Find all faculty teaching Computer Science
- Find faculty assigned to Course A
- Find faculty handling more than 3 courses

---

## Attendance Queries

- Find students absent for more than 5 classes
- Find attendance records for Semester 2

---

## Scholarship Queries

- Find students eligible for scholarship
- Find rejected scholarship applications

---

# 6. Reflection: Why Enterprise Systems React Automatically to Data Changes

Enterprise systems handle large volumes of data.

Manual reactions are slow and unreliable.

Automatic event-driven behavior allows systems to:

- Respond instantly
- Reduce human error
- Maintain consistency
- Enforce business rules
- Improve efficiency

Triggers make Salesforce intelligent by reacting automatically whenever important changes happen.

This allows enterprise systems to scale efficiently.

