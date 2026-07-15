# Day 1 — Introduction to DBMS, FMS, API, Frontend, Backend, Full Stack

## Overview
This page summarizes the key concepts covered on Day 1: the role of frontend and backend in full‑stack development, how APIs connect them, and where data is stored (file systems vs databases).

---

## Full Stack
Full Stack = Frontend + Backend

- Frontend: the client-side, visual and interactive layer users see (browser / mobile app).
- Backend: the server-side logic, data processing and persistence layer.

## Frontend
Responsibilities:
- Display web pages and UI
- Accept user input (forms, buttons, search)
- Validate input before sending to the server
- Call backend APIs to fetch/send data
- Display responses from the backend
- Provide animations and interactive effects

Common technologies: HTML, CSS, JavaScript, Bootstrap (and modern frameworks like React/Vue/Angular).

## Backend
Responsibilities:
- Process client requests
- Implement business logic
- Connect with databases and perform CRUD operations
- Authenticate and authorize users
- Encrypt sensitive data (passwords)
- Generate reports and return responses to the frontend

Common languages and platforms: Python, Java, .NET, PHP, C/C++ (and Node.js, Go, Ruby, etc.).

## API (Application Programming Interface)
An API is a set of rules/protocols that lets different applications communicate and exchange data without exposing internal implementation details. APIs act as the bridge between frontend and backend.

Advantages of APIs:
- Enable communication between systems
- Promote code reuse
- Platform independent
- Speed up development and integrations
- Improve scalability and maintainability

## Storage Areas
Two main types of storage in applications:

1) Temporary (in-memory) storage — cleared when the process stops. Examples: JVM heap/stack, registers.
2) Permanent (persistent) storage — data saved long-term. Examples: file systems, databases, data warehouses.

## File Management Systems (FMS)
A file management system stores data in files managed by the operating system. Each application is responsible for its own file formats and access routines.

When to use: small/simple datasets, quick prototypes, or when structured storage is not required.

Limitations of FMS:
- Data redundancy (duplicate information across files)
- Data inconsistency (updates not propagated)
- Poor security and access control
- Difficult retrieval and searching (custom code needed)
- Lack of integrity constraints (e.g., uniqueness)
- Scalability problems as data grows

## Database Management System (DBMS)
A DBMS is a collection of programs that enable users to create, manage, and manipulate structured databases. It provides an interface between users/applications and the data store.

Advantages of DBMS:
- Store large amounts of structured data
- Query language support (e.g., SQL) for powerful data operations
- Access control and security (usernames/passwords)
- Structured tables with constraints (primary keys, foreign keys, unique constraints) to prevent duplication and maintain integrity

Limitations:
- Not ideal for extremely large volumes (data warehouses/big data solutions are better for TB-scale or unstructured/semi-structured data)
- Traditional relational DBMSs are optimized for structured/tabular data (other systems are used for unstructured data).

## FMS vs DBMS — Key differences
- Structure: FMS stores raw files; DBMS stores structured tables and schemas.
- Redundancy & Consistency: DBMS enforces constraints to avoid redundancy and inconsistency; FMS does not.
- Querying: DBMSs provide query languages (SQL); FMS requires custom parsing/searching code.
- Security & Access Control: DBMS provides built-in access control; FMS relies on OS permissions.
- Scalability: DBMS scales better for growing datasets and concurrent access.

---

## Next steps / Suggested exercises
- Try building a simple frontend form that calls a backend API.
- Create a small database schema (users, products) and implement basic CRUD operations.
- Compare storing the same data in text files vs a database and observe differences.

---

Created from: Day 1 notes (Day_01_MySQL)
