# Azure SQL Database Project

A mini project demonstrating how to create, configure, and query a fully managed relational database using **Microsoft Azure SQL Database**, along with a bonus reference guide covering 25 essential Linux commands.

## 👥 Team: Azure Visioners

**Guide:** Ajey B K

**Members:**
| Name | USN |
|---|---|
| Nisha Sinha | 1EP23CS112 |
| J Vandana | 1EP23CS066 |
| Uzma Samreen Madeena | 1EP23CS170 |

*East Point College of Engineering & Technology — Department of Computer Science & Engineering*

## 📌 Project Overview

This project walks through the complete lifecycle of provisioning an Azure SQL Database via the Azure Portal — from signing in to running SQL queries against a live cloud database.

### Steps Covered
1. Log in to the Azure Portal
2. Search for Azure SQL Database
3. Click "Create"
4. Fill in basic details (Subscription, Resource Group, Database Name)
5. Add a new SQL Server name
6. Set admin username & password
7. Choose Locally Redundant Storage (LRS) for backups
8. Configure Networking (Public endpoint)
9. Review Security defaults
10. Review Additional Settings
11. Skip Tags (optional)
12. Review + Create the resource
13. Wait for deployment to complete
14. Open the Query Editor and authenticate via SQL Authentication
15. Create a `Student` table
16. Insert sample records
17. Run a `SELECT * FROM Student` query to verify data

### Key Concepts Defined
- **Azure Portal** – web console to manage Azure cloud resources
- **Azure SQL Database** – fully managed SQL Server–based relational database service
- **Resource Group** – logical container grouping related Azure resources
- **SQL Server (Azure)** – logical administrative server managing logins, firewall rules, and databases
- **Locally Redundant Storage (LRS)** – low-cost backup redundancy within a single data center
- **Public Endpoint** – connectivity method allowing internet access to the database (firewall-controlled)
- **Query Editor** – in-browser tool to run SQL queries without external software
- **SQL Authentication** – login via username/password rather than Azure AD credentials

## 🗄️ Sample Schema

```sql
CREATE TABLE Student (
    StudentID INT PRIMARY KEY,
    Name VARCHAR(50),
    Department VARCHAR(30),
    CGPA DECIMAL(3,2)
);

INSERT INTO Student VALUES
(101, 'Uzma', 'CSE', 9.10),
(102, 'Aisha', 'ISE', 8.80),
(103, 'Rahul', 'ECE', 8.50);

SELECT * FROM Student;
```

## 🐧 Bonus: 25 Linux Commands You Should Know

A quick reference of essential Linux/WSL commands demonstrated with real terminal output, including:

`ls`, `mkdir`, `cd`, `rmdir`, `pwd`, `touch`, `vim`, `cp`, `mv`, `cat`, `rm`, `man`, `chmod`, `tar`, `gzip`, `gunzip`, `ping`, `ifconfig`, `top`, `sudo`, `df`, `du`, `uptime`, `date`, `whoami`

## 🛠️ Tools Used
- Microsoft Azure Portal
- Azure SQL Database (Serverless, General Purpose tier)
- WSL (Ubuntu) for Linux command demonstrations

## 📄 License
This project is for academic/educational purposes as part of a mini project submission.
