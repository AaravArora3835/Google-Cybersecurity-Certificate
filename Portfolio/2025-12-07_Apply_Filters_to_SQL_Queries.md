# Apply Filters to SQL Queries

## Project Description

In this project, I used SQL to retrieve and filter security-related and organizational data from a database. I applied the `WHERE` clause along with the `AND`, `OR`, and `NOT` operators to isolate specific records. These queries demonstrate how SQL can be used in cybersecurity to investigate login activity and manage employee information.

---

## Retrieve After-Hours Failed Login Attempts

I queried the login attempts table to identify **failed login attempts that occurred outside normal business hours**. This helps detect potentially suspicious activity that may indicate unauthorized access attempts.

Example logic used:

* Filter for failed login attempts
* Filter for timestamps outside standard working hours
* Combine conditions using `AND`

---

## Retrieve Login Attempts on Specific Dates

I retrieved login attempts that occurred on **specific dates** to support incident investigations or audits tied to known events.

Example logic used:

* Filter records by date
* Use comparison operators within the `WHERE` clause
* Narrow results to only relevant time periods

---

## Retrieve Login Attempts Outside of Mexico

I filtered login attempt records to show activity originating **outside of Mexico**, which is useful for identifying unusual geographic access patterns.

Example logic used:

* Use the `NOT` operator
* Exclude records where the country equals `Mexico`

---

## Retrieve Employees in Marketing

I queried the employees table to return all employees who work in the **Marketing** department.

Example logic used:

* Filter by department name
* Use an equality condition in the `WHERE` clause

---

## Retrieve Employees in Finance or Sales

I retrieved employees who work in either the **Finance** or **Sales** departments.

Example logic used:

* Combine multiple conditions using the `OR` operator
* Return records that match at least one department

---

## Retrieve All Employees Not in IT

I filtered the employees table to return all employees **who are not part of the IT department**.

Example logic used:

* Use the `NOT` operator
* Exclude a specific department from the results

---

## Summary

In this activity, I:

* Used SQL to filter security and employee data
* Applied `AND`, `OR`, and `NOT` operators to refine queries
* Retrieved login attempts based on time, date, and location
* Filtered employee records by department inclusion and exclusion

This project demonstrates my ability to use SQL for **security investigations, auditing, and organizational analysis**, which are essential skills in cybersecurity roles.
