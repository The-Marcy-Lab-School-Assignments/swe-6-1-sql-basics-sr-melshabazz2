# Short Response: SQL Basics

Answer each question below. Write in complete sentences (3–5 per answer).

---

## Question 1

What is a database? Why do we use one instead of storing data in a JavaScript array on your server?

**Your answer:**

---
- A ***Database*** is a structured collection of data that is organized in a manner for easy retrieval. We use databases instead of a JS array in our server because arrays are risky while a database is persistent, ensuring that data is written to a permanent storage. Databases are engineered to handle petabytes of data, while an arrays storage is much smaller and can crash the server due to running out of memory. In arrays any part of your code may corrupt the server while databases enforce strict rules to ensure data follows a specific format and offers access control, allowing those who has access to see or change information.

## Question 2

What is a primary key? Why does every table need one?

**Your answer:**

---
- A **primary key** is a column that uniquely names each record in a table. It's the digital footprint for each record and ensures that no other row is identical, making it easy to locate every single data entry.

## Question 3

In one sentence, describe what this query does in plain English:

```sql
SELECT * FROM books WHERE genre = 'fiction' ORDER BY year DESC LIMIT 5;
```

Aim for something like: *"It returns the 5 most recently published fiction books."*

**Your answer:**

---
- It retrieves the 5 newest fiction books in the order of newest to oldest.

## Question 4

Why is it dangerous to run `DELETE FROM books` without a `WHERE` clause? What does it actually do?

**Your answer:**

---
- It is dangerous to run that query because it will delete all books, their is no undo button either so all data will be permanantely removed but the table will still exist. Using `WHERE` allows you to be more specific in what you want to delete to avoid deleting anything you didnt mean to.

## Question 5

What is the difference between `ORDER BY` and `LIMIT`? Could you use one without the other? Give an example to support your answer.

**Your answer:**
- `ORDER BY` is used to order data by ascending or descending order while `LIMIT` is used to limit the amount of data that is returned. Yes they can be used without the other because they are independant tools, for example we use `ORDER BY` if we want to return oldest to newest video games of a table and `LIMIT` if we only want the 5 oldest games in that table.
