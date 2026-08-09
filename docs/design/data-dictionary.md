# Data Dictionary

## Student__c

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| Student_ID__c | Auto Number | Yes | Unique student id |
| First_Name__c | Text | Yes | Student first name |
| Last_Name__c | Text | Yes | Student last name |
| Email__c | Email | Yes | Unique email |
| Mobile__c | Phone | Yes | Mobile number |
| Date_of_Birth__c | Date | Yes | Date of birth |
| Gender__c | Picklist | Yes | Gender |
| Address__c | Long Text | No | Address |
| Registration_Status__c | Picklist | Yes | Registration status |

---

## Admission_Application__c

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| Application_Number__c | Auto Number | Yes | Application number |
| Student__c | Master Detail | Yes | Student |
| Course__c | Lookup | Yes | Course |
| Application_Date__c | Date | Yes | Application date |
| Status__c | Picklist | Yes | Application status |
Status = Draft, Submitted, Approved, Rejected
---

## Course__c

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| Course_Code__c | Text | Yes | Course code |
| Course_Name__c | Text | Yes | Course name |
| Department__c | Picklist | Yes | Department |
| Duration__c | Number | Yes | Course duration |
| Fee__c | Currency | Yes | Course fee |
