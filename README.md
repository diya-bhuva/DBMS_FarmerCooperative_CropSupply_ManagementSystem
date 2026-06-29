# 🌾 Farmer Cooperative Crop Supply System (FCCSS)

A relational database project designed to streamline the agricultural supply chain by managing farmers, cooperative societies, crop procurement, inventory, logistics, and buyer orders.

---

## 📌 Project Overview

The **Farmer Cooperative Crop Supply System (FCCSS)** models the end-to-end workflow of agricultural cooperatives — from farmer registration and crop procurement to inventory tracking and buyer order fulfillment. The system is built on a normalized relational schema, ensuring data integrity, minimal redundancy, and efficient querying.

> **Course Project** - Database Management Systems (DBMS)

---

## 🗂️ Repository Structure

```
FCCSS/
│
├── DDL_SCRIPT.txt                    # SQL DDL script for table creation
├── ER_DIAGRAM.pdf                    # Entity-Relationship diagram
├── FCCSS_Insert_Script.txt           # SQL script for inserting dummy data
├── FCCSS_Queries.pdf                 # Sample SQL queries with output
├── FDs_MinimalFDs_Normalization.pdf  # Functional dependencies & normalization
├── RELATIONAL-SCHEMA.pdf             # Relational schema diagram
└── README.md
```

---

## 🧩 Key Entities & Modules

| Module | Description |
|---|---|
| **Farmers** | Stores farmer profiles, contact details, and cooperative membership |
| **Cooperative Societies** | Manages cooperative organizations that aggregate crop supply |
| **Crops** | Tracks crop types, seasons, and procurement prices |
| **Procurement** | Records crop purchases from farmers by cooperatives |
| **Inventory** | Monitors stock levels held by cooperative warehouses |
| **Buyers** | Maintains buyer/vendor information for order fulfillment |
| **Orders** | Tracks buyer orders, quantities, and delivery status |
| **Logistics** | Manages transport and delivery scheduling |

---

## 🗺️ ER Diagram

The ER diagram captures all entities, attributes, primary keys, foreign keys, and relationships (one-to-many, many-to-many) in the system.

📄 See [`ER_DIAGRAM.pdf`](./ER_DIAGRAM.pdf) for the full diagram.

---

## 🗃️ Database Schema

The database is implemented in **PostgreSQL**. The schema covers:

- Table definitions with appropriate data types and constraints
- Primary key and foreign key relationships
- `NOT NULL`, `UNIQUE`, and `CHECK` constraints for data integrity

📄 See [`RELATIONAL-SCHEMA.pdf`](./RELATIONAL-SCHEMA.pdf) for the relational schema diagram.

To set up the database locally:

```bash
# 1. Create a new PostgreSQL database
createdb fccss_db

# 2. Run the DDL script to create tables
psql -d fccss_db -f DDL_SCRIPT.txt

# 3. Insert dummy data
psql -d fccss_db -f FCCSS_Insert_Script.txt
```

---

## 📐 Normalization

The schema has been normalized to eliminate redundancy and ensure data consistency.

📄 See [`FDs_MinimalFDs_Normalization.pdf`](./FDs_MinimalFDs_Normalization.pdf) for detailed functional dependencies and normalization steps.

**Highlights:**
- **1NF** — All attributes are atomic; no repeating groups
- **2NF** — No partial dependencies on composite keys
- **3NF** — No transitive dependencies between non-key attributes

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **PostgreSQL** | Relational database engine |
| **SQL** | Schema definition and querying |
| **Draw.io / Lucidchart** | ER Diagram design *(or whichever tool was used)* |

---

## 🚀 How to Run

**Prerequisites:**
- PostgreSQL installed on your machine
- `psql` CLI or pgAdmin

**Steps:**

```bash
# Clone the repo
git clone https://github.com/diya-bhuva/DBMS_FarmerCooperative_CropSupply_ManagementSystem.git

# Navigate into the project
cd DBMS_FarmerCooperative_CropSupply_ManagementSystem

# Create the database
createdb fccss_db

# Run DDL script to create tables
psql -d fccss_db -f DDL_SCRIPT.txt

# Insert dummy data
psql -d fccss_db -f FCCSS_Insert_Script.txt
```

---

## 👩‍💻 Author

**Diya Bhuva**
- GitHub: [@diya-bhuva](https://github.com/diya-bhuva)

---

## 📄 License

This project is for academic purposes. Feel free to reference or build upon it with attribution.
