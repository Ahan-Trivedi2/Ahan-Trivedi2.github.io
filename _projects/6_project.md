---
layout: page
title: Statistical Database with Differential Privacy
description: 
img: assets/img/sql_db.png
importance: 6
category: 
---

<strong>Github Source Files</strong>: [https://github.com/Ahan-Trivedi2/SQL-Statistical-Database-w-Differential-Privacy](https://github.com/Ahan-Trivedi2/SQL-Statistical-Database-w-Differential-Privacy)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/sql_db.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

For my Databases course, I worked on a team of three to build a lightweight, in-memory SQL-like statistical database engine with built-in privacy protections using Go. Our system supports core SQL commands (CREATE TABLE, INSERT, SELECT, GROUP BY, and basic aggregates) and extends them with differential privacy, k-anonymity, and l-diversity to protect sensitive data by adding controlled noise to query results and enforcing privacy constraints on output. The engine includes a custom lexer and parser to process SQL, a runtime that executes queries on dynamic in-memory table structures, and privacy modules that manage privacy budgets and noise injection to limit what can be inferred about individual records.




