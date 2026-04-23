# When Clean Design Gets Complex — Database Normalization Challenge

Welcome Developer 👋

### To the Challenge

In this challenge, you will act as a **database engineer** fixing a poorly designed schema.

The current database works, but it violates several **normalization rules**, which leads to:

- duplicated data
- inconsistent updates
- complex maintenance
- scalability problems

Your mission is to **analyze the schema, normalize it to 3NF, and test queries on the improved structure.**

---

# The Problem

The current database stores product information for an e-commerce system.

However, the schema has several issues:

• Some fields contain **multiple values in a single column**  
• Some attributes **depend on other non-key attributes**  
• Some tables **mix unrelated information**

This violates **database normalization principles**.

Your job is to redesign the schema so that it follows **Third Normal Form (3NF)**.

---

# Learning Goals

By completing this challenge, you will learn how to:

- identify normalization problems
- break composite fields into proper tables
- create correct relationships between entities
- test queries after schema changes
- understand trade-offs between normalization and query complexity

---

# Repository Guide
schema/
broken_schema.sql

queries/
product_queries.sql

docs/
problem-context.md


---

# Where You Will Work

### 1️⃣ Schema Fixing

File:


schema/broken_schema.sql


This file contains the **broken database design**.

Your tasks:

- identify repeating fields
- separate dependent attributes
- create new tables where needed
- define primary and foreign keys

You must:

- create a new file named:


normalized_schema.sql


---

### 2️⃣ Query Testing

File:


queries/product_queries.sql


These queries simulate **real product queries**.

After normalization:

- some queries may break
- some queries may require **JOINs**

Update the queries so they work with your normalized schema.

---

# Expected Output

You should produce:

### 1️⃣ A normalized schema

Either:


schema/normalized_schema.sql


or an updated version of the original schema.

### 2️⃣ Working Queries

Update:


queries/product_queries.sql


So they work with your new schema.

### 3️⃣ Screenshots

Take screenshots showing:

- normalized tables
- working queries

---

# Tips

Start simple.

Look for columns that contain things like:


"Electronics, Mobile, Gadgets"


Those should usually be **separate rows in another table**.

Also check for things like:


supplier_name
supplier_phone
supplier_email


These likely belong in a **Supplier table**.

---

# Evaluation

Your work will be evaluated based on:

- correct normalization
- correct query updates
- understanding of design trade-offs

---

Good luck! 🚀

First you must

git init
git commit -m "Updated files"
git branch -M main
git remote add origin https://github.com/Moureesh-M/4.5-When-Clean-Design-Gets-Complex-Challenge-2.git
git push -u origin main

then Work in Your Own Repository

Make the required changes in your fork:

- Fix the schema  
- Create `normalized_schema.sql`  
- Update `product_queries.sql`  
- Add screenshots  

Commit your changes as pull request in the repository.