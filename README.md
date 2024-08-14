# Bank Management Database

This repository contains the SQL scripts to create and manage a bank management database. It includes tables for personal information, customer references, bank details, and account information. The project is designed to demonstrate how to set up a relational database for a banking system.

## Database Structure
BankManagementDB/
├── sql/
│   ├── create_tables.sql
│   ├── insert_data.sql
│   └── select_queries.sql
└── README.md


### Tables

- **PersonalInfo:** Stores personal details of customers.
- **CustomerReferenceInfo:** Stores reference information related to customers.
- **BankInfo:** Stores details of banks, including IFSC codes, bank names, and branch names.
- **AccountInfo:** Stores account-related information for customers.

### Relationships

- `CustomerID` in `AccountInfo` references `CustomerID` in `PersonalInfo`.
- `IFSCCode` in `AccountInfo` references `IFSCCode` in `BankInfo`.
- `CustomerID` in `CustomerReferenceInfo` references `CustomerID` in `PersonalInfo`.

## SQL Files

- **`create_tables.sql`:** Contains the SQL statements to create the necessary tables.
- **`insert_data.sql`:** Contains the SQL statements to insert dummy data into the tables.
- **`select_queries.sql`:** Contains the SQL queries for retrieving data from the database.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/BankManagementDB.git
2. Navigate to the directory:
   ``` bash
   cd BankManagementDB/sql
3. Run the SQL scripts in the following order:
   create_tables.sql
   insert_data.sql
   select_queries.sql


###  **Push to GitHub**
   - Add the files to the repository and commit:
     ```bash
     git add .
     git commit -m "Initial commit with SQL scripts and README"
     ```
   - Push the changes to GitHub:
     ```bash
     git push origin main
     ```


   
   
