# Football Ticket Booking System Database



**Assignment:** B7A3 - PostgreSQL Database Design and Querying  
**Project Title:** Football Ticket Booking System


---

# Project Overview

The Football Ticket Booking System is a relational database designed to manage football match ticket reservations. The system stores information about users, football matches, and booking records while maintaining data integrity through primary key and foreign key constraints.

The database allows users to:

* View available football matches
* Book tickets for matches
* Track payment status
* Manage booking information
* Retrieve booking and match-related reports using SQL queries

---

#  Final Submission:
✅ ERD Link (Public):  https://drawsql.app/teams/john-nz/diagrams/assignment 
✅ GitHub Repository Link (Public): https://github.com/Fahmid-run/Football-Ticket-Booking-System-Database

# Database Design

The database consists of three tables:

## 1. Users

Stores information about registered users.

Attributes:

* user_id (Primary Key)
* full_name
* email
* role
* phone_number

---

## 2. Matches

Stores football match information.

Attributes:

* match_id (Primary Key)
* fixture
* tournament_category
* base_ticket_price
* match_status

---

## 3. Bookings

Stores ticket booking information.

Attributes:

* booking_id (Primary Key)
* user_id (Foreign Key)
* match_id (Foreign Key)
* seat_number
* payment_status
* total_cost

---

# Entity Relationship Diagram (ERD)

Relationship Structure:

* One User can have multiple Bookings.
* One Match can have multiple Bookings.
* Each Booking belongs to one User.
* Each Booking belongs to one Match.

Cardinality:

Users (1) → (Many) Bookings

Matches (1) → (Many) Bookings

---

# Technologies Used

* PostgreSQL
* SQL
* Draw.io (ERD Design)
* beekeeper

---



# Project Structure

```text
Football-Ticket-Booking-System/
│
├── README.md
├── QUERY.sql
```

---

# How to Run

### Step 1

Open PostgreSQL or pgAdmin.

### Step 2

Create a new database.

### Step 3

Open the QUERY.sql file.

### Step 4

Execute the script.

The script will:

* Create all required tables
* Insert sample data
* Execute all required queries

