---

title: Data Engineering — Complete Roadmap & Detailed Syllabus  
category: Data Engineering  
subject: Data Engineering  
difficulty: Beginner → Advanced  
status: Learning  
created: 2026-08-10  
tags:

- data-engineering
    
- syllabus
    
- roadmap
    
- cse-foundation
    
- sql
    
- python
    
- linux
    
- git
    
- spark
    
- kafka
    
- databricks
    
- delta-lake
    
- gcp
    
- bigquery
    
- dataflow
    
- airflow
    
- system-design
    

---

# 🧭 Data Engineering — Complete Master Roadmap

> [!abstract] Ultimate Goal  
> Become capable of **understanding → designing → building → debugging → optimizing → explaining → defending** real-world Data Engineering systems.

> [!tip] Core Learning Philosophy  
> **WHY → WHAT → INTUITION → HOW → UNDER THE HOOD → IMPLEMENT → EXPERIMENT → BREAK → DEBUG → OPTIMIZE → PROJECT → INTERVIEW → CERTIFICATION**

---

# MODULE 01 — [[SQL for Data Engineering]]

> [!info] Module Properties  
> **Module:** 01  
> **Category:** SQL  
> **Level:** Beginner → Advanced  
> **Goal:** Master SQL for databases, analytics, ETL/ELT, optimization, and Data Engineering interviews.

---

## 1.1 [[Relational Database Foundations]]

### Properties

- **Type:** Foundation
    
- **Level:** Beginner
    
- **Purpose:** Understand how relational databases store and organize data.
    

### Topics

- [[Database]]
    
- [[DBMS]]
    
- [[RDBMS]]
    
- [[Relational Model]]
    
- [[Tables]]
    
- [[Rows]]
    
- [[Columns]]
    
- [[Schema]]
    
- [[Data Types]]
    
- [[Primary Keys]]
    
- [[Foreign Keys]]
    
- [[Constraints]]
    
- [[Relationships]]
    
- [[NULL Values]]
    

---

## 1.2 [[SQL Fundamentals]]

### Properties

- **Type:** SQL Fundamentals
    
- **Level:** Beginner
    
- **Purpose:** Learn the basic structure of SQL queries.
    

### Topics

- [[SELECT]]
    
- [[FROM]]
    
- [[WHERE]]
    
- [[DISTINCT]]
    
- [[ORDER BY]]
    
- [[LIMIT]]
    
- [[OFFSET]]
    
- [[SQL Aliases]]
    

---

## 1.3 [[SQL Filtering]]

### Properties

- **Type:** SQL Filtering
    
- **Level:** Beginner
    
- **Purpose:** Filter rows based on conditions.
    

### Topics

- [[Comparison Operators]]
    
- [[AND]]
    
- [[OR]]
    
- [[NOT]]
    
- [[IN]]
    
- [[NOT IN]]
    
- [[BETWEEN]]
    
- [[LIKE]]
    
- [[NOT LIKE]]
    
- [[IS NULL]]
    
- [[IS NOT NULL]]
    

---

## 1.4 [[SQL Aggregations]]

### Properties

- **Type:** Aggregation
    
- **Level:** Beginner
    
- **Purpose:** Summarize and analyze data.
    

### Topics

- [[COUNT]]
    
- [[SUM]]
    
- [[AVG]]
    
- [[MIN]]
    
- [[MAX]]
    
- [[GROUP BY]]
    
- [[HAVING]]
    

---

## 1.5 [[SQL Conditional Logic]]

### Properties

- **Type:** Conditional Logic
    
- **Level:** Beginner → Intermediate
    
- **Purpose:** Perform conditional transformations inside SQL queries.
    

### Topics

- [[CASE]]
    
- [[WHEN]]
    
- [[THEN]]
    
- [[ELSE]]
    
- [[END]]
    
- [[COALESCE]]
    
- [[NULLIF]]
    

---

## 1.6 [[SQL Functions]]

### Properties

- **Type:** SQL Functions
    
- **Level:** Intermediate
    
- **Purpose:** Transform and manipulate values.
    

### [[String Functions]]

#### Properties

- **Type:** String Functions
    
- **Level:** Beginner → Intermediate
    

### Topics

- [[CONCAT]]
    
- [[SUBSTRING]]
    
- [[LENGTH]]
    
- [[LOWER]]
    
- [[UPPER]]
    
- [[TRIM]]
    
- [[REPLACE]]
    

### [[Numeric Functions]]

#### Properties

- **Type:** Numeric Functions
    
- **Level:** Beginner → Intermediate
    

### Topics

- [[ROUND]]
    
- [[CEIL]]
    
- [[FLOOR]]
    
- [[ABS]]
    

### [[Date and Time Functions]]

#### Properties

- **Type:** Date/Time Functions
    
- **Level:** Intermediate
    

### Topics

- [[CURRENT_DATE]]
    
- [[CURRENT_TIMESTAMP]]
    
- [[DATE_PART]]
    
- [[DATE_TRUNC]]
    
- [[Date Arithmetic]]
    

---

## 1.7 [[SQL JOINs]]

### Properties

- **Type:** Relational Operations
    
- **Level:** Intermediate
    
- **Importance:** ⭐⭐⭐⭐⭐
    
- **Purpose:** Combine data from multiple tables.
    

### Topics

- [[INNER JOIN]]
    
- [[LEFT JOIN]]
    
- [[RIGHT JOIN]]
    
- [[FULL OUTER JOIN]]
    
- [[CROSS JOIN]]
    
- [[SELF JOIN]]
    
- [[Multiple JOINs]]
    
- [[JOIN Conditions]]
    
- [[JOIN Cardinality]]
    
- [[Duplicate Rows Caused by JOINs]]
    

---

## 1.8 [[SQL Subqueries]]

### Properties

- **Type:** Query Composition
    
- **Level:** Intermediate
    
- **Purpose:** Build queries using nested queries.
    

### Topics

- [[Scalar Subqueries]]
    
- [[Multi-row Subqueries]]
    
- [[Correlated Subqueries]]
    
- [[EXISTS]]
    
- [[NOT EXISTS]]
    
- [[IN vs EXISTS]]
    

---

## 1.9 [[SQL CTEs]]

### Properties

- **Type:** Query Organization
    
- **Level:** Intermediate
    
- **Purpose:** Write modular and readable SQL.
    

### Topics

- [[WITH]]
    
- [[Multiple CTEs]]
    
- [[Recursive CTE Basics]]
    
- [[CTE vs Subquery]]
    
- [[CTE Readability]]
    
- [[CTE Reusability]]
    

---

## 1.10 [[SQL Set Operations]]

### Properties

- **Type:** Set Operations
    
- **Level:** Intermediate
    
- **Purpose:** Combine results from multiple queries.
    

### Topics

- [[UNION]]
    
- [[UNION ALL]]
    
- [[INTERSECT]]
    
- [[EXCEPT]]
    

---

## 1.11 [[SQL Window Functions]]

### Properties

- **Type:** Advanced SQL
    
- **Level:** Intermediate → Advanced
    
- **Importance:** ⭐⭐⭐⭐⭐
    
- **Purpose:** Perform calculations across related rows without collapsing them.
    

### Topics

- [[OVER]]
    
- [[PARTITION BY]]
    
- [[Window ORDER BY]]
    
- [[ROW_NUMBER]]
    
- [[RANK]]
    
- [[DENSE_RANK]]
    
- [[LAG]]
    
- [[LEAD]]
    
- [[FIRST_VALUE]]
    
- [[LAST_VALUE]]
    
- [[Running Totals]]
    
- [[Moving Averages]]
    
- [[Ranking Within Groups]]
    

---

## 1.12 [[SQL Transactions]]

### Properties

- **Type:** Database Transactions
    
- **Level:** Intermediate → Advanced
    
- **Purpose:** Understand reliable database operations and concurrency.
    

### Topics

- [[Transaction]]
    
- [[COMMIT]]
    
- [[ROLLBACK]]
    
- [[ACID]]
    
- [[Atomicity]]
    
- [[Consistency]]
    
- [[Isolation]]
    
- [[Durability]]
    
- [[Isolation Levels]]
    
- [[Database Locks]]
    
- [[Concurrency]]
    

---

## 1.13 [[Database Performance]]

### Properties

- **Type:** Database Optimization
    
- **Level:** Intermediate → Advanced
    
- **Importance:** ⭐⭐⭐⭐⭐
    
- **Purpose:** Understand how databases execute and optimize queries.
    

### Topics

- [[Indexes]]
    
- [[B-tree Index]]
    
- [[Composite Indexes]]
    
- [[Query Planner]]
    
- [[Query Execution]]
    
- [[Full Table Scan]]
    
- [[Index Scan]]
    
- [[EXPLAIN]]
    
- [[EXPLAIN ANALYZE]]
    

---

## 1.14 [[Advanced SQL Performance]]

### Properties

- **Type:** Advanced Optimization
    
- **Level:** Advanced
    
- **Purpose:** Optimize complex queries and analytical workloads.
    

### Topics

- [[Query Optimization]]
    
- [[Predicate Filtering]]
    
- [[Join Optimization]]
    
- [[Database Partitioning]]
    
- [[Index Selection]]
    
- [[Query Cost]]
    
- [[Materialized Views]]
    

---

## 1.15 [[SQL for Data Engineering]]

### Properties

- **Type:** Data Engineering SQL
    
- **Level:** Intermediate → Advanced
    
- **Importance:** ⭐⭐⭐⭐⭐
    
- **Purpose:** Apply SQL directly to production data pipelines.
    

### Topics

- [[ETL with SQL]]
    
- [[ELT with SQL]]
    
- [[SQL Data Cleaning]]
    
- [[SQL Deduplication]]
    
- [[Incremental Loading]]
    
- [[Upserts]]
    
- [[MERGE]]
    
- [[Change Data Capture]]
    
- [[Data Validation]]
    
- [[Analytical SQL]]
    

---

## 1.16 [[SQL Practice]]

### Properties

- **Type:** Practice
    
- **Level:** Beginner → Advanced
    
- **Purpose:** Build problem-solving and interview skills.
    

### Topics

- [[Beginner SQL Problems]]
    
- [[Intermediate SQL Problems]]
    
- [[Advanced SQL Problems]]
    
- [[Real Business SQL Queries]]
    
- [[SQL Interview Problems]]
    
- [[Data Engineering SQL Scenarios]]
    

---

## 1.17 [[SQL Projects]]

### Properties

- **Type:** Projects
    
- **Level:** Beginner → Advanced
    
- **Purpose:** Apply SQL to realistic data problems.
    

### Projects

- [[Employee Analytics]]
    
- [[E-commerce Analytics]]
    
- [[Customer Retention Analysis]]
    
- [[Sales Analytics]]
    
- [[SQL Data Cleaning Project]]
    
- [[SQL ETL Pipeline]]
    

---

# 🎯 [[SQL Mastery]]

> [!success] Mastery Target  
> I can **write, explain, debug, optimize, and defend SQL** used in real-world Data Engineering pipelines.

### Mastery Checklist

-  [[Relational Database Foundations]]
    
-  [[SQL Fundamentals]]
    
-  [[SQL Filtering]]
    
-  [[SQL Aggregations]]
    
-  [[SQL Conditional Logic]]
    
-  [[SQL Functions]]
    
-  [[SQL JOINs]]
    
-  [[SQL Subqueries]]
    
-  [[SQL CTEs]]
    
-  [[SQL Set Operations]]
    
-  [[SQL Window Functions]]
    
-  [[SQL Transactions]]
    
-  [[Database Performance]]
    
-  [[Advanced SQL Performance]]
    
-  [[SQL for Data Engineering]]
    
-  [[SQL Practice]]
    
-  [[SQL Projects]]
    

---

# 🗺️ SQL Learning Flow

```text
[[Relational Database Foundations]]
                ↓
       [[SQL Fundamentals]]
                ↓
         [[SQL Filtering]]
                ↓
        [[SQL Aggregations]]
                ↓
      [[SQL Conditional Logic]]
                ↓
          [[SQL Functions]]
                ↓
            [[SQL JOINs]]
                ↓
         [[SQL Subqueries]]
                ↓
            [[SQL CTEs]]
                ↓
       [[SQL Set Operations]]
                ↓
      [[SQL Window Functions]]
                ↓
        [[SQL Transactions]]
                ↓
      [[Database Performance]]
                ↓
  [[Advanced SQL Performance]]
                ↓
     [[SQL for Data Engineering]]
                ↓
          [[SQL Practice]]
                ↓
          [[SQL Projects]]
                ↓
          [[SQL Mastery]]
```

# 📁 Suggested Obsidian Folder Structure

```text
Data Engineering/
│
├── 00 - Roadmap/
│   └── Data Engineering — Complete Roadmap.md
│
├── 01 - SQL/
│   ├── 01 - Relational Database Foundations/
│   ├── 02 - SQL Fundamentals/
│   ├── 03 - SQL Filtering/
│   ├── 04 - SQL Aggregations/
│   ├── 05 - SQL Conditional Logic/
│   ├── 06 - SQL Functions/
│   ├── 07 - SQL JOINs/
│   ├── 08 - SQL Subqueries/
│   ├── 09 - SQL CTEs/
│   ├── 10 - SQL Set Operations/
│   ├── 11 - SQL Window Functions/
│   ├── 12 - SQL Transactions/
│   ├── 13 - Database Performance/
│   ├── 14 - Advanced SQL Performance/
│   ├── 15 - SQL for Data Engineering/
│   ├── 16 - SQL Practice/
│   └── 17 - SQL Projects/
│
└── Templates/
    ├── Topic Template.md
    ├── Subtopic Template.md
    └── Project Template.md
```

# 🧩 Obsidian Topic Note Template

Use this template for **every topic/subtopic** linked above.

```yaml
---
title: Topic Name
type: topic
category: Data Engineering
module: SQL
level: Beginner
status: Not Started
importance: Medium
tags:
  - data-engineering
  - sql
---
```

# 📚 Topic Note Structure

```markdown
# [[Topic Name]]

## Properties

- **Category:** [[Data Engineering]]
- **Module:** [[SQL for Data Engineering]]
- **Level:** Beginner
- **Status:** Not Started
- **Importance:** Medium

## 🎯 Learning Objectives

- Understand [[Topic Name]]
- Explain why it is needed
- Understand how it works
- Implement it
- Debug common problems
- Optimize when applicable
- Apply it in real-world Data Engineering

## 🧠 Core Concept

> [!note] Definition
> Write the simple definition here.

## 💡 Intuition

Explain the concept in simple terms.

## ⚙️ How It Works

Explain the internal working step by step.

## 🔬 Under the Hood

Explain implementation details and database internals where applicable.

## 💻 Examples

Add practical SQL/code examples.

## 🧪 Practice

- [ ] Beginner problem
- [ ] Intermediate problem
- [ ] Advanced problem

## ⚠️ Common Mistakes

- Mistake 1
- Mistake 2
- Mistake 3

## 🚀 Real-World Data Engineering Usage

Explain where this concept appears in production pipelines.

## 🔗 Related Topics

- [[Related Topic 1]]
- [[Related Topic 2]]
- [[Related Topic 3]]

## 🎯 Interview Questions

- Question 1
- Question 2
- Question 3

## ✅ Mastery Checklist

- [ ] I can define it
- [ ] I understand the intuition
- [ ] I can implement it
- [ ] I can debug it
- [ ] I can explain it in an interview
- [ ] I can use it in a real project
```