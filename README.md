# 🎓 **Gestion_Ecole - Student Management System** 🎓

Welcome to **Gestion_Ecole**, a mini-project designed to manage student records in a school. This project is a simple yet powerful Windows Forms application built using **C#** and **MySQL**. It demonstrates the implementation of **CRUD operations** (Create, Read, Update, Delete) and follows best practices in software design, such as **modularity**, **separation of concerns**, and **data binding**.

---

## ✨ **Features**

### **1. CRUD Operations**
- **📝 Create**: Add new student records to the database.
- **📖 Read**: Fetch and display student records in a `DataGridView`.
- **🔄 Update**: Modify existing student records.
- **❌ Delete**: Remove student records from the database.

### **2. 🔍 Dynamic Search**
- Search for students based on criteria such as **name**, **prenom**, **ville**, and **specialite**.
- Dynamically generate SQL queries for flexible searching.

### **3. 📊 Data Binding**
- Use **data binding** to display student records in a `DataGridView`.
- Automatically refresh the `DataGridView` after CRUD operations.

### **4. 🧩 Modular Design**
- **Data Access Layer (DAL)**: Handles database operations (`DAOEleve` and `Connexion` classes).
- **Business Logic Layer (BLL)**: Represents the student entity (`Eleve` class).
- **Presentation Layer**: Provides the user interface (`Form1`).

### **5. 🔒 Secure Database Connectivity**
- Use **parameterized queries** to prevent SQL injection.
- Encapsulate database connectivity logic in the `Connexion` class.

---

## 🛠️ **Technologies Used**

- **Programming Language**: C#
- **Framework**: .NET 8.0
- **Database**: MySQL
- **UI Framework**: Windows Forms
- **Database Connector**: MySql.Data (NuGet Package)

---

## 🎯 **Key Learnings**

### **1. Database Connectivity**
- Learned how to connect a C# application to a MySQL database using the `MySqlConnection` class.
- Implemented reusable methods for executing SQL queries (`select` and `iud`).

### **2. CRUD Operations**
- Gained hands-on experience in implementing **Create**, **Read**, **Update**, and **Delete** operations.
- Understood the importance of **parameterized queries** for security and efficiency.

### **3. Data Binding**
- Learned how to bind a `DataGridView` to a data source (e.g., `DataTable` or `List`).
- Discovered the benefits of using a `BindingSource` for better data management.

### **4. Dynamic Query Generation**
- Implemented dynamic SQL query generation based on user input.
- Improved flexibility and reduced the need for hardcoded queries.

### **5. Error Handling**
- Added basic error handling to manage database exceptions and invalid user input.
- Learned the importance of providing feedback to users (e.g., success/error messages).

### **6. Modular Design**
- Practiced separating concerns into different layers (DAL, BLL, Presentation Layer).
- Improved code maintainability and reusability.

### **7. User Interface Design**
- Designed a simple and intuitive user interface using Windows Forms.
- Learned how to handle user interactions (e.g., button clicks, form loading).

---

## 🚀 **How to Run the Project**

### **Prerequisites**
1. **.NET SDK**: Install the .NET 8.0 SDK from [here](https://dotnet.microsoft.com/download).
2. **MySQL Database**: Set up a MySQL database and create the `eleve` table using the following schema:
   ```sql
   CREATE TABLE eleve (
       id INT PRIMARY KEY AUTO_INCREMENT,
       nom VARCHAR(50),
       prenom VARCHAR(50),
       ville VARCHAR(50),
       specialite VARCHAR(50)
   );
