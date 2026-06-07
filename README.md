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

### Diagram

                +----------------+
                |    Student     |
                +----------------+
                       |
      -----------------------------------
      |          |          |           |
      v          v          v           v
   Login  
   Add Skill    Add Cert.   Add Internship 
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
 Manage Users   View Reports   Monitor
                               Progress
