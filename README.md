# 🌾 Farmer Cooperative Crop Supply System (FCCSS)

A relational database project designed to streamline the agricultural supply chain by managing farmers, cooperative societies, crop procurement, inventory, logistics, and buyer orders.

---

## 📌 Project Overview

The **Farmer Cooperative Crop Supply System (FCCSS)** models the end-to-end workflow of agricultural cooperatives — from farmer registration and crop procurement to inventory tracking and buyer order fulfillment. The system is built on a normalized relational schema, ensuring data integrity, minimal redundancy, and efficient querying.

> **Course Project** — Database Management Systems (DBMS)

---

## 🗂️ Repository Structure

```
FCCSS/
│
├── er_diagram/             # ER Diagram (entity-relationship model)
│   └── er_diagram.pdf
│
├── schema/                 # SQL scripts for database creation
│   └── create_tables.sql
│
├── normalization/          # Normalization documentation (1NF → 3NF/BCNF)
│   └── normalization.pdf
│
└── README.md
```

> ⚠️ *File names above are indicative — refer to actual files in the repo.*

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

📄 See [`er_diagram/`](./er_diagram/) for the full diagram.

---

## 🗃️ Database Schema

The database is implemented in **PostgreSQL**. The schema covers:

- Table definitions with appropriate data types and constraints
- Primary key and foreign key relationships
- `NOT NULL`, `UNIQUE`, and `CHECK` constraints for data integrity

To set up the database locally:

```bash
# 1. Create a new PostgreSQL database
createdb fccss_db

# 2. Run the schema script
psql -d fccss_db -f schema/create_tables.sql
```

---

## 📐 Normalization

The schema has been normalized up to **Third Normal Form (3NF)** to eliminate redundancy and ensure data consistency.

📄 See [`normalization/`](./normalization/) for detailed step-by-step normalization documentation.

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

# Run schema script
psql -d fccss_db -f schema/create_tables.sql
```

---

## 👩‍💻 Author

**Diya Bhuva**
- GitHub: [@diya-bhuva](https://github.com/diya-bhuva)

---

## 📄 License

This project is for academic purposes. Feel free to reference or build upon it with attribution.
