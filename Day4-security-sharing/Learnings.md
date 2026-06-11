# 📚 Learnings from Day 4

During Day 4 of the Salesforce Administrator Track, I learned how Salesforce secures data and controls user access through the Security & Sharing Model.

---

## 🔹 Data Security

Learned the importance of securing business data within Salesforce.
Understood how Salesforce ensures that users only access the data necessary for their roles.

---

## 🔹 Profiles

Learned that Profiles define what a user can do in Salesforce.

Key permissions controlled by Profiles:
- Object Permissions
- App Access
- Tab Visibility
- System Permissions

---

## 🔹 Permission Sets

Learned that Permission Sets provide additional permissions without modifying Profiles.

Key points:
- Extend user access
- Multiple permission sets can be assigned
- Follow the principle of least privilege

---

## 🔹 Field Level Security (FLS)

Learned how to control access to specific fields.

Understood how Salesforce can:
- Hide sensitive fields
- Make fields read-only
- Restrict field visibility

---

## 🔹 Organization-Wide Defaults (OWD)

Learned that OWD is the foundation of record-level security.

Key access levels:
- Private
- Public Read Only
- Public Read/Write
- Controlled by Parent

---

## 🔹 Role Hierarchy

Learned how Salesforce uses role hierarchies to provide record access based on organizational structure.

Benefits:
- Easier record sharing
- Managerial visibility
- Better data organization

---

## 🔹 Sharing Rules

Learned how Sharing Rules grant additional record access beyond OWD.

Types learned:
- Owner-Based Sharing Rules
- Criteria-Based Sharing Rules

---

## 🔹 Record-Level Security

Learned how Salesforce determines which records users can access.

Understood the relationship between:
- OWD
- Role Hierarchy
- Sharing Rules
- Manual Sharing

---

## 🔹 Enterprise Access Control

Learned how organizations design secure access models.
Understood how different users such as Students, Faculty, HODs, Principals, and Administrators require different levels of access.

---

## 🎯 Key Takeaway

Day 4 helped me understand that Salesforce security is not just about restricting access—it is about ensuring that the right users have the right access to the right data at the right time. Proper implementation of Profiles, Permission Sets, Roles, OWD, and Sharing Rules helps maintain security, privacy, and compliance across an organization.
