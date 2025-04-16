# 🔄 Bidirectional ClickHouse & Flat File Data Ingestion Tool

A web-based application that enables seamless bidirectional data transfer between ClickHouse databases and flat files, implemented using JDBC for database connectivity.

---

## ✨ Overview

This application provides a user-friendly interface to transfer data:

- 📊 **ClickHouse → Flat File**: Export data from your database to structured flat files.
- 📁 **Flat File → ClickHouse**: Import data from flat files into your database.

The tool allows users to select specific columns for ingestion and reports the total number of records processed upon completion.

---

## 🚀 Features

- ↔️ **Bidirectional Data Flow**: Transfer data in both directions between ClickHouse and flat files.
- 🔍 **Source Selection**: Choose between ClickHouse or flat file as your data source.
- ✅ **Column Selection**: Select specific columns to include in the data transfer.
- 🔐 **JWT Authentication**: Connect to ClickHouse securely using JWT token-based authentication.
- 🔎 **Schema Discovery**: Automatically detect and display available tables and columns.
- 📊 **Completion Reporting**: View the total count of processed records upon successful ingestion.
- ⚠️ **Error Handling**: User-friendly error messages for connection, authentication, and data transfer issues.

---

## 💻 Technology Stack

- **Backend**: Java with JDBC for database connectivity, Spring Boot
- **Frontend**: HTML, CSS, JavaScript, React.js
- **Database**: ClickHouse
- **File Handling**: Java I/O libraries for flat file operations

---

## 📋 Prerequisites

- ☕ Java Development Kit (JDK) 11 or higher
- 🛠️ Apache Maven (for build management)
- 🌐 Web browser
- 🗄️ ClickHouse instance (local Docker or cloud-based)

---

## 🔧 Installation and Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Suryanshrajs/ClickFlat.git
   cd clickhouse-flat-file-ingestion
Build the project:

bash
Copy
Edit
mvn clean install
Run the application:

Execute the BackendApplication.java file.

Backend Port: 8080

Access the web interface:

Navigate to http://localhost:5173 in your web browser.

📝 Usage Guide
📊 ClickHouse to Flat File Transfer
Select Operation: Choose to import or export data.

Provide Necessary Credentials:

🖥️ Host (e.g., localhost)

🔌 Port (e.g., 9440 for HTTPS, 9000 for HTTP)

🗃️ Database name

👤 Username

🔑 Password

Select Tables and Columns: Choose the specific tables and columns for the data transfer.

Preview and Download: View a preview of the data and download the flat file.

📁 Flat File to ClickHouse Transfer
Select Source File: Ensure the data in the file starts from the second line.

Choose Delimiter: Select the appropriate delimiter based on your file format.

Provide Necessary Credentials:

🖥️ Host (e.g., localhost)

🔌 Port (e.g., 9440 for HTTPS, 9000 for HTTP)

🗃️ Database name

👤 Username

🔑 Password

Data Ingestion: The data will be added to the ClickHouse database.

⚙️ Data Processing
Efficient batch processing of records during data transfer.

Type mapping between ClickHouse data types and flat file representations.

Transaction management for reliable data ingestion.

🧪 Testing
The application has been tested with:

ClickHouse example datasets (uk_price_paid and ontime).

Various flat file formats with different delimiters.

Edge cases for error handling.

❓ Troubleshooting
🔴 Connection Failure
Verify ClickHouse host and port.

Check if JWT token is valid and not expired.

Ensure ClickHouse server is running.

📁 File Access Error
Verify file path and permissions.

Check if file format matches the configured delimiter.

⚠️ Data Type Mismatch
Ensure compatibility between ClickHouse columns and flat file data types.

🌟 Quick Start
For the fastest setup experience:

bash
Copy
Edit

# Clone repository
git clone https://github.com/Suryanshrajs/ClickFlat.git