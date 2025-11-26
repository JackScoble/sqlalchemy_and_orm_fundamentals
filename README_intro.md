# Introduction to SQLAlchemy

## Learning Outcomes
- Explain what SQLAlchemy is and why it is used  
- Configure and initialise a SQLAlchemy project  
- Understand how SQLAlchemy prevents SQL injection  

## 1. What is SQLAlchemy?

SQLAlchemy is a Python SQL toolkit and Object Relational Mapper (ORM) that enables developers to interact with relational databases using Python classes and objects instead of writing raw SQL.

It provides:

- A high-level ORM for defining database models using Python classes  
- A lower-level Core layer for constructing SQL statements in a structured, safe way  
- Built‑in protection from SQL injection through automatic parameter binding  
- Database‑agnostic code that works with SQLite, PostgreSQL, MySQL, MariaDB and others  

SQLAlchemy abstracts away many error‑prone aspects of raw SQL and improves maintainability, readability, and long‑term scalability.

## 2. Configure and Initialise a SQLAlchemy Project

To begin working with SQLAlchemy:

1. Create an engine to connect to the database  
2. Create a session factory to manage transactions  
3. Define metadata and ORM models  

These components allow your Python application to communicate with the database in a consistent and structured way.

## 3. How SQLAlchemy Prevents SQL Injection

SQLAlchemy prevents SQL injection by:

- Using parameterised queries for all database interactions  
- Compiling SQL statements safely rather than interpolating raw strings  
- Ensuring user‑supplied data is always treated as values, not executable SQL  

This significantly reduces the risk of malicious input compromising your application.

## Notes
- For more information go to the official SQLAlchemy unified tutorial at https://docs.sqlalchemy.org/en/20/tutorial/index.html