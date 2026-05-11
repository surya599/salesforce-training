# Day 3 - Data Modeling in Salesforce

## 1. Difference Between App, Object, Record, and Field

### App
An app is a collection of tabs, objects, and features designed for a specific business process.

**Example:** College Management App

---

### Object
An object is like a database table that stores related data.

**Example:** Student Object

---

### Record
A record is a single entry inside an object.

**Example:**  
Student Name: Surya Reddy  
Roll No: 23PA1A0502

---

### Field
A field stores specific information inside a record.

**Example:**  
- Name  
- Email  
- Department  
- GPA

---

# 2. Standard vs Custom Objects

## Standard Objects
Pre-built objects provided by Salesforce.

Examples:
- Account
- Contact
- Lead
- Opportunity

**Purpose:** Used for CRM processes.

---

## Custom Objects
Objects created by users based on business needs.

Examples:
- Student
- Faculty
- Course
- Attendance

**Purpose:** Used for organization-specific data.

---

# 3. My College Data Model

## Objects
- Student
- Faculty
- Course
- Department
- Attendance

---

## Relationships

### Department → Course
One department can have many courses.

### Course → Student
One course can have many students.

### Faculty → Course
One faculty can teach many courses.

### Student → Attendance
One student can have many attendance records.

---

## Data Model Diagram

```plaintext
Department
   |
   |----< Course >---- Faculty
             |
             |
        Student
             |
             |
       Attendance
      
       