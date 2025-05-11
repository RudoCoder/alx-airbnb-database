AirBnB Clone – Database Schema (DDL)

Objective
This module defines the database schema for the AirBnB clone project, following best practices in normalization and relational design.

Files

- `schema.sql`: Contains all `CREATE TABLE` statements, constraints, enums, and indexes.
- `README.md`: Describes the structure and objectives of the schema.

 Highlights

- All tables use `UUID` as primary keys for scalability and uniqueness.
- Foreign key constraints are used to maintain relational integrity.
- ENUM types are used for predefined values (e.g., role, booking status, payment method).
- Indexes added for frequently queried fields such as email, property_id, and booking_id.
- Data model adheres to Third Normal Form (3NF) to eliminate redundancy.

Tables

- users
- properties
- booking_status
- bookings
- payments
- reviews
- messages

 Usage

To initialize the schema, run:

```bash
psql -d your_database_name -f schema.sql

