# Free SIM and Broadband Database Management System

A terminal-based Python application that provides a complete CRUD interface for managing SIM and broadband records. Built with Python and MySQL, the program simulates a lightweight administrative backend for managing user details based on Aadhar authentication.

## 🚀 Features

- Create and switch to MySQL databases.
- Create tables for:
  - `freesim`: Stores SIM owner name, phone number, Aadhar number (Primary Key), and country code.
  - `freebroadband`: Stores modem owner, broadband ID, telephone number (Primary Key), plan, and Aadhar reference.
- Insert new user data with integrity across both tables.
- Display records (all or conditional queries).
- Delete and update entries using Aadhar number as the key.
- Filter records based on various fields (e.g., SIM owner, plan, telephone number).
- Interactive menu-based CLI with prompts for database setup and operations.

## 🧠 Tech Stack

- **Language**: Python
- **Database**: MySQL
- **Connector**: `mysql-connector-python`

## 🗂️ Table Structure

### `freesim`
| Column | Type        | Description                  |
|--------|-------------|------------------------------|
| som    | VARCHAR(30) | SIM Owner Name               |
| pn     | VARCHAR(30) | Phone Number                 |
| ac     | VARCHAR(30) | Aadhar Number (Primary Key)  |
| cc     | VARCHAR(30) | Country Code                 |

### `freebroadband`
| Column | Type        | Description                    |
|--------|-------------|--------------------------------|
| mon    | VARCHAR(30) | Modem Owner Name               |
| bbi    | VARCHAR(30) | Broadband ID                   |
| tn     | VARCHAR(30) | Telephone Number (Primary Key) |
| plan   | INT         | Broadband Plan                 |
| ac     | VARCHAR(30) | Aadhar Number (Foreign Key)    |

## 🔧 How to Run

1. Make sure MySQL is installed and a user with appropriate permissions is available.
2. Install the Python MySQL connector:
   ```bash
   pip install mysql-connector-python
Run the script:

bash
Copy
Edit
python your_script.py
Follow on-screen prompts to create a database or use an existing one, then perform operations as desired.

📌 Notes
Ensure MySQL is running locally (localhost) and credentials (user='root', passwd='Mysql') are valid.

To avoid manual re-entry, future enhancement could involve GUI integration or session storage.

✍️ Author
Priyanshu Acharya

📄 License
This project is open for educational purposes and experimentation.

vbnet
Copy
Edit





