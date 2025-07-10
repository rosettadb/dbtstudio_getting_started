# DBTStudio - Getting Started Sample Project

Welcome to the **Getting Started** project for [**DBTStudio**](https://github.com/rosettadb/dbt-studio) — a visual interface for **dbt-core** powered by the magic of [**RosettaDB**](https://github.com/AdaptiveScale/rosetta)!

This sample project provides you with a lightweight, ready-to-use **DuckDB** database to kick off your data modeling journey. It's designed to help you explore DBTStudio’s capabilities for generating **staging**, **enhanced**, and **business** layer dbt models with a few simple clicks.

---

## What You’ll Get With DBTStudio

-  A pre-built **DuckDB** sample database with real-world academic data structures
-  Auto-generated **staging**, **enhanced**, and **business** models via **RosettaDB**
-  One-click execution of **dbt-core** commands directly from the UI
-  A perfect playground to understand how DBTStudio speeds up your analytics workflow

---

##  Sample Schema Overview

This demo simulates a basic university database system. Here are the four core tables included in the sample project:

### `students`

| Column            | Type    | Description                |
| ----------------- | ------- | -------------------------- |
| `student_id`      | INTEGER | Unique ID for each student |
| `name`            | TEXT    | Student's full name        |
| `major`           | TEXT    | Major field of study       |
| `enrollment_year` | INTEGER | Year the student enrolled  |

---

### `courses`

| Column       | Type    | Description                     |
| ------------ | ------- | ------------------------------- |
| `course_id`  | INTEGER | Unique ID for each course       |
| `title`      | TEXT    | Name of the course              |
| `department` | TEXT    | Academic department offering it |
| `credits`    | INTEGER | Credit value of the course      |

---

### `enrollments`

| Column          | Type    | Description                  |
| --------------- | ------- | ---------------------------- |
| `enrollment_id` | INTEGER | Unique ID for the enrollment |
| `student_id`    | INTEGER | Links to the student         |
| `course_id`     | INTEGER | Links to the course          |
| `semester`      | TEXT    | Semester of enrollment       |

---

### `grades`

| Column          | Type    | Description                    |
| --------------- | ------- | ------------------------------ |
| `grade_id`      | INTEGER | Unique ID for the grade entry  |
| `enrollment_id` | INTEGER | Links to the enrollment record |
| `grade`         | INTEGER    | Value grade (10, 9, etc.)      |
| `date_recorded` | DATE    | When the grade was recorded    |

---

## How to Use This

1. **Download [**DBTStudio**](https://github.com/rosettadb/dbt-studio/releases)**


2. **Open DBTStudio**\
   Launch DBTStudio and create a new project by cloning this repository.
   ```bash
    https://github.com/rosettadb/dbtstudio_getting_started.git
   ```

3. **Generate Models with Rosetta**

   - Select tables and generate **staging**, **enhanced**, or **business** models with one click.
   - Explore the automatically created `.sql` files in your dbt models directory.

4. **Run dbt Commands Visually**\
   Use the **"dbt actions"** panel to:

   - Run models (`dbt run`)
   - Test models (`dbt test`)
   - View lineage and documentation

---

## Ideal For

- New users trying dbt for the first time
- Teams adopting DBTStudio in modern data workflows
- Educators and students simulating real-world academic data
- Anyone exploring **RosettaDB** model generation magic

---

## Folder Structure

```
getting-started/
├── dbt_project.yml
├── models/
│   ├── staging/
│   ├── enhanced/
│   └── business/
├── rosetta/
    ├── main.conf
│   └── university_sample.duckdb
│
└── README.md
```

---

## Acknowledgements

- 🛆Powered by [RosettaDB](https://github.com/AdaptiveScale/rosetta)
-  Built for dbt-core lovers and productivity seekers
-  Inspired by the modern data stack

---

Happy modeling!\
— The **DBTStudio** Team

