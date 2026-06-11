# 🔐 Salesforce Administrator Track – Day 4

Salesforce Security & Sharing Model controls what users can do and which records they can access. It helps organizations protect sensitive data while ensuring users have the right level of access.

---

# 📚 Trailhead Modules Completed

- Data Security
- Control Access to Objects
- Control Access to Fields
- Control Access to Records
- Role Hierarchy
- Sharing Rules
  
---

# 🔒 What is OWD?

OWD (Organization-Wide Defaults) is the baseline level of record access in Salesforce.

Common OWD settings:
- Private and Public Read Only
- Public Read/Write
- Controlled by Parent

OWD is the first layer of record-level security.

---

# 👥 What is Role Hierarchy?

Role Hierarchy allows users higher in the hierarchy to access records owned by users below them.

Benefits:
- Simplifies data sharing
- Reflects organizational structure
- Provides managerial visibility

Example:
Principal
↓
HOD
↓
Faculty
↓
Student

The Principal can access records owned by all lower roles.

---

# 🔄 What are Sharing Rules?

Sharing Rules extend record access beyond OWD settings.

They automatically grant access to users, roles, or groups.

Types:
- Owner-Based Sharing Rules
- Criteria-Based Sharing Rules

---

# ⚖️ Difference Between Profile, Permission Set, and Role

| Feature | Profile | Permission Set | Role |
|----------|----------|---------------|------|
| Purpose | Controls what users can do | Grants additional permissions | Controls record visibility |
| Mandatory | Yes | No | No |
| Controls Object Access | Yes | Yes | No |
| Controls Record Access | No | No | Yes |
| Used For | Base access | Extra access | Record sharing |

---

# 🏫 College Security Design

### Student
- View own records only
- Edit limited personal details
- Cannot delete records

### Faculty
- View student records of assigned department
- Update attendance
- Cannot delete student records

### Placement Officer
- View placement records
- Update placement information
- Cannot delete student records

### HOD
- View all records within department
- Manage faculty and student information

### Principal
- View all institutional records
- Read-only access to sensitive data if required

### Salesforce Administrator
- Full system access
- Manage users, security, and configurations

---

# 🎓 Faculty Access Scenario

### Requirement

- Faculty A should only see CSE students
- Faculty B should only see ECE students
- HOD should see all students in the department
- Principal should see everything

### Solution

#### OWD
Set Student Records to **Private**

#### Role Hierarchy

Principal
↓
HOD
↓
Faculty

#### Sharing Rules

- Share CSE student records with CSE Faculty
- Share ECE student records with ECE Faculty

#### Permission Sets

Grant additional permissions where required without modifying profiles.

---

# 💭 Reflection

## Why is Record-Level Security Important?

- Protects sensitive information
- Maintains student privacy
- Prevents unauthorized access
- Reduces accidental modifications
- Enhances overall system security

---

# 🎯 Day 4 Outcome

By completing this module, I gained knowledge of:

- Profiles and Permission Sets
- Role Hierarchy
- Organization-Wide Defaults (OWD)
- Sharing Rules
- Field Level Security (FLS)
- Record-Level Security
