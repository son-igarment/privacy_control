# Privacy Control System

A Java Swing based application developed by **Phạm Lê Ngọc Sơn** for managing customer and product information with database connectivity.

## Project Overview

The Privacy Control System is a desktop application that provides an interface for managing:
- Customer information storage and retrieval
- Product details management
- Database connectivity using JDBC

## Project Structure

```
privacy_control/
├── src/                  # Source code files
│   ├── gg.java           # Product information form (Java code)
│   ├── gg.form           # Product information form (Swing form)
│   ├── frmProduct.java   # Alternative product form implementation
│   ├── frmProduct.form   # Alternative product form design
│   ├── frmCustomer.java  # Customer information form (Java code)
│   ├── frmCustomer.form  # Customer information form (Swing form)
│   ├── cro4ky_Yin_Yang1.jpg # Background image for Customer form
│   └── 3.JPG             # Background image for Product form
├── build/                # Compiled files
├── dist/                 # Distribution files
├── nbproject/            # NetBeans project files
├── manifest.mf           # Manifest file
└── build.xml             # Ant build script
```

## Features

### Customer Management
- Add new customer details
- Store customer ID, name, address, mobile number, email
- Link customers to products

### Product Management
- Add new product details
- Store product ID, name, version, price, validity
- Track product information

## Technologies Used

- **Java Swing**: For the graphical user interface
- **JDBC**: For database connectivity
- **SQL Server**: Main database connection for product information
- **ODBC**: Alternative database connection for customer information
- **NetBeans IDE**: Development environment

## Setup Requirements

1. **Java Development Kit (JDK) 8 or higher**
2. **NetBeans IDE** (recommended for form editing)
3. **Microsoft SQL Server** with a database named "SPC"
4. **JDBC Driver** for SQL Server
5. **ODBC Connection** named "SPC"

## Database Configuration

### SQL Server Configuration
- Create a database named "SPC"
- Create a login with username "sa" and password "sa" (for production, use more secure credentials)
- Enable SQL Server authentication

### Tables Required
1. **tblCustomer**:
   - CustId (Primary Key)
   - CustName
   - Address
   - mobno
   - EmailId
   - ProductId (Foreign Key)

2. **tblProduct**:
   - ProductId (Primary Key)
   - ProdName
   - ProdVersion
   - ProdPrice
   - ProdValidity

## How to Use

1. **Compile and Run the Application**:
   - Open the project in NetBeans
   - Build the project (F11)
   - Run the project (F6)

2. **Adding a New Product**:
   - Launch the application
   - Enter product details (ID, name, version, price, validity)
   - Click "Submit" to save to database

3. **Adding a New Customer**:
   - Open the customer form
   - Enter customer details (ID, name, address, mobile, email)
   - Enter an existing product ID to associate with the customer
   - Click "SUBMIT" to save to database

## Future Improvements

- Implement data validation
- Add search and update functionality
- Implement user authentication
- Create reports and data export features
- Improve UI design and user experience

## Contact

For any inquiries regarding this project, please contact Phạm Lê Ngọc Sơn.

---

© 2023 Phạm Lê Ngọc Sơn. All rights reserved.