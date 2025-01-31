# ServiceNow Table Management

This guide provides an overview of managing tables in ServiceNow, including auditing, creating custom tables, and designing forms. It also covers key concepts related to rows, columns, and the Incident module.

---

## Auditing in ServiceNow

### Purpose of Auditing
Auditing in ServiceNow tracks record changes in the database, including:
- **Insertions**: New records added.
- **Deletions**: Records removed.
- **Modifications**: Changes made to existing records.

### How to Check Audit History
1. Navigate to the desired table (e.g., User table).
2. Right-click on a record and select **History**.
3. View changes in either **Calendar** or **List** format.

### Enabling Auditing
1. Go to **System Definition > Tables**.
2. Open the desired table (e.g., User table).
3. In the **Dictionary** section, set the **Audit** field to **true**.

---

## Tables, Rows, and Columns

### Key Concepts
- **Table**: A combination of rows and columns.
- **Row**: A single record (horizontal entry).
- **Column**: A field or attribute (vertical entry).

### Types of Tables
- **Out-of-the-Box Tables**: Provided by ServiceNow (e.g., User, Incident).
- **Custom Tables**: Created by users, prefixed with `u_`.

---

## Creating a Custom Table

1. Navigate to **System Definition > Tables**.
2. Click **New**.
3. Fill in the mandatory fields:
   - **Label**: Display name (e.g., Apple 15).
   - **Name**: Automatically generated (e.g., `u_apple_15`).
   - **Extend Table**: Leave as default.
   - **Application Scope**: Set to **Global**.
4. Auto-created fields include:
   - **Created**, **Created By**, **Updated**, **Updated By**, **Sys ID**.

---

## Form Design and Layout

### Form Design
1. Open the table and go to **Configure > Form Design**.
2. Drag and drop fields to rearrange them.
3. Use **Two-Column Layout** for better organization.

### Form Layout
1. Add or remove fields as needed.
2. Use **Begin Split** and **End Split** for grouping related fields.

---

## Incident Module Example

### Incident Table
The Incident table tracks issues and their details.

### Key Fields
- **Incident Number**
- **Caller**
- **Category**
- **Short Description**
- **Priority**

### Audit History
Track changes made to incidents using the audit history feature.

---

## Key Takeaways

### JavaScript
- Practice daily using resources like **W3Schools**.
- Focus on mastering the fundamentals.

### ServiceNow Tables
- Understand the difference between **rows** and **columns**.
- Learn to create and audit custom tables.
- Use **form design** and **layout tools** effectively.

### Incident Management
- Explore the **Incident module** to understand how records are managed and audited.

---

For more details, refer to the official [ServiceNow documentation](https://docs.servicenow.com/).

---
# JavaScript Basics and ServiceNow Table Management

## JavaScript Learning Resources
- **W3Schools**: A free, open-source platform to learn various programming languages like HTML, CSS, JavaScript, SQL, Python, Java, and PHP.
- **Focus on JavaScript**: Essential for portal configurations, designing, and working with frameworks like Angular.

  - Introduction to JavaScript
  - Outputs, statements, and syntax
  - Comments, variables (`let`, `const`), and operators
  - Functions, objects, and APIs

### Example: JavaScript Basics
```html
<!DOCTYPE html>
<html>
<body>
  <h1>JavaScript Example</h1>
  <p id="demo"></p>
  <script>
    let x = 5;
    let y = 2;
    let z = x + y;
    document.getElementById("demo").innerHTML = z;
  </script>
</body>
</html>