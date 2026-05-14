# Day 5 – Apex Introduction

## Salesforce Summer Program – Day 5

---

# 1. What is Apex?

Apex is Salesforce’s object-oriented programming language used to write custom business logic on the Salesforce platform.

It is similar to Java and runs on Salesforce servers.

Apex is used when declarative tools like Flows and Process Builder are not enough to solve complex business requirements.

### Why Apex is Needed

Apex helps developers:

- Create custom automation
- Write advanced business rules
- Perform database operations
- Integrate with external systems
- Process large amounts of data efficiently

### Example

Apex can:

- Automatically calculate scholarship eligibility
- Prevent invalid course registration
- Connect Salesforce with payment systems
- Handle complex approval workflows

---

# 2. Difference Between Flow vs Apex

| Feature | Flow | Apex |
|---------|------|------|
| Type | Declarative (No-code/Low-code) | Programmatic (Code-based) |
| Development Style | Drag-and-drop | Writing code |
| Best For | Simple automation | Complex custom logic |
| Ease of Use | Easier for admins | Requires coding skills |
| Flexibility | Limited | Highly flexible |
| Maintenance | Easy | Requires testing/debugging |

## Configuration vs Coding

### Configuration

Uses built-in Salesforce tools:

- Flow Builder
- Validation Rules
- Formula Fields
- Process Automation

Best for:

- Standard business automation
- Quick development
- Low maintenance

---

### Coding

Uses Apex classes and triggers.

Best for:

- Advanced calculations
- External integrations
- Complex business logic
- Bulk data processing

---

# 3. Real Examples Where Apex is Needed

## Example 1: Complex Fee Calculation

A college fee depends on:

- Category reservation
- Scholarship percentage
- Hostel fees
- Late payment penalties
- Attendance discounts

Flow becomes difficult to manage.

Apex handles this efficiently.

---

## Example 2: External Payment Integration

Connecting Salesforce with payment systems like:

- Razorpay
- Stripe

Requires:

- API callouts
- Error handling
- Secure processing

Apex is required.

---

## Example 3: Advanced Eligibility Validation

A student can register only if:

- Attendance ≥ 75%
- No pending fee dues
- Seats are available
- Required prerequisite course completed

This requires complex conditional checks across multiple objects.

Apex handles this easily.

---

# 4. Integrated College Management System Design

## CRM

Salesforce manages:

- Student admissions
- Course registration
- Faculty records
- Fee tracking
- Notifications

---

## Objects

Custom Objects:

- Student
- Course
- Faculty
- Attendance
- Payment
- Scholarship
- Department

---

## Relationships

- Student ↔ Course (Many-to-Many)
- Faculty → Course (One-to-Many)
- Student → Attendance (One-to-Many)

---

## Validation Rules

Examples:

- Student email is required
- Roll number must be unique
- Admission date cannot be future date

---

## Formula Fields

Example:

Remaining Seats

```formula
Total_Seats__c - Enrolled_Students__c
```

---

## Flow Automation

Examples:

- Send admission confirmation email
- Notify fee due reminders
- Attendance warning alerts

---

## Apex Logic

Custom logic includes:

- Scholarship calculation
- Registration eligibility checking
- Bulk semester promotion
- Complex reporting automation

---

# 5. Pseudocode Examples

## Example 1: Seat Availability

```text
IF remainingSeats <= 0
THEN block registration
ELSE allow registration
```

---

## Example 2: Attendance Warning

```text
IF attendance < 75%
THEN notify student
```

---

## Example 3: Scholarship Approval

```text
IF CGPA >= 8.5 AND familyIncome < limit
THEN approve scholarship
ELSE reject
```

---

# 6. Reflection: Why Enterprise Systems Eventually Need Programming

Declarative tools are excellent for common automation tasks.

However, enterprise systems become complex because they involve:

- Unique business rules
- Large-scale data processing
- External integrations
- Advanced calculations
- Performance optimization

No-code tools solve standard problems.

Programming solves custom business complexity.

That is why Apex exists in Salesforce.

Developers should always prefer declarative solutions first.

Apex should be used only when business requirements cannot be solved efficiently using clicks and configuration.

This approach keeps systems scalable, maintainable, and efficient.

---

