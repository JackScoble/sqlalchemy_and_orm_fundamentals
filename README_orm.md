# Introduction to SQLAlchemy ORM

## Learning Outcomes

### 1. Define and map database tables using SQLAlchemy ORM
- Create Python classes that represent database tables.
- Use `DeclarativeBase`, `Mapped`, and SQLAlchemy column types.
- Add relationships between tables using `relationship()` and foreign keys.

### 2. Perform CRUD operations using the ORM session
Learn to:
- Insert new records (`session.add`, `session.commit`)
- Query existing records (`session.query`, `select()`)
- Update records
- Delete records

### 3. Model simple relationships between tables
Implement database relationships using SQLAlchemy’s ORM tools:
- One-to-many (e.g., Owner → Cars)
- Many-to-one
- One-to-one
- Many-to-many

The accompanying example (in the notebook) demonstrates:
- A one-to-many relationship
- Implemented using a foreign key (`owner_id`)
- With `relationship(back_populates=...)` on both sides

---

## SQLAlchemy Supports Multiple Relationship Types

### ✔ One-to-many  
Example: One owner can have many cars

### ✔ Many-to-one  
A car belongs to exactly one owner

### ✔ One-to-one  
Two tables tightly linked

### ✔ Many-to-many  
Implemented using an association table

---

## Summary

This README introduces the foundational concepts of SQLAlchemy, including:

- Setting up and initialising a SQLAlchemy project  
- ORM modelling using Python classes  
- CRUD operations  
- SQL-safe querying (via parameter binding)  
- Mapping and navigating relationships between tables  

## Additional Notes

SQLAlchemy ORM allows you to work with the database using Python objects rather than raw SQL. It improves:

- Maintainability  
- Testability  
- Security  
- Development speed  

It also automatically prevents SQL injection by parameterising queries internally.
