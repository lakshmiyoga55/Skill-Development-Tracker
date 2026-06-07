# Skill Development Tracker

## Problem Statement
Students often struggle to track their skills, certifications, internships, and learning progress in a single place. This project provides a centralized platform to manage and monitor skill development activities effectively.

## Objectives
- To track students' skill development progress.
- To update daily learning activities.
- To set and achieve learning goals.
- To monitor completed and ongoing skills.
- To generate progress reports.

## Features
- Add Skills
- Update Progress
- Set Goals
- View Reports

## Technologies Used
- Java
- MySQL

## Project Status
Objective Definition Completed

## Users

### Student
- Add Skills
- Update Progress
- Set Goals
- View Reports

### Admin
- Manage Students
- Monitor Reports

## Modules

### Login Module
- User Authentication

### Skill Management Module
- Add Skill
- Edit Skill
- Delete Skill

### Progress Tracking Module
- Update Progress
- View Progress

### Goal Setting Module
- Set Goals
- Track Goals

### Report Generation Module
- Generate Reports
- View Reports

## Use Case Diagram

### Actors

- Student
- Admin

## Diagram

```text
                +----------------+
                |    Student     |
                +----------------+
                       |
      -----------------------------------
      |          |          |           |
      v          v          v           v
   Login    Add Skill   Add Cert.   Add Internship
      |
      v
 View Progress


                +--------------+
                |    Admin     |
                +--------------+
                       |
      --------------------------------
      |              |              |
      v              v              v
 Manage Users   View Reports   Monitor Progress
```

## Database Requirements

Student Table

- Student ID
- Name
- Email
- Department
- Year

Skill Table

- Skill ID
- Skill Name
- Skill Level
- Student ID

Certification Table

- Certificate ID
- Certificate Name
- Provider
- Completion Date
- Student ID

Internship Table

- Internship ID
- Company Name
- Role
- Duration
- Student ID

Relationships

- One Student can have multiple Skills.
- One Student can have multiple Certifications.
- One Student can have multiple Internships.

Purpose

The database is used to store and manage student skills, certifications, internships, and progress details.

## ER Diagram
```text
+-----------+
|  Student  |
+-----------+
| StudentID |
| Name      |
| Email     |
| Department|
+-----------+
      |
      | 1
      |
      | M
      v
+-----------+
|   Skill   |
+-----------+
| SkillID   |
| SkillName |
| Level     |
+-----------+

      |
      | 1
      |
      | M
      v
+----------------+
| Certification  |
+----------------+
| CertificateID  |
| Name           |
| Provider       |
+----------------+

      |
      | 1
      |
      | M
      v
+--------------+
| Internship   |
+--------------+
| InternshipID |
| CompanyName  |
| Role         |
+--------------+
```

Relationships

- One Student can have many Skills.
- One Student can have many Certifications.
- One Student can have many Internships.
