# 🛠️ Customer_Flow

### **Overview**
**Customer_Flow** is a Python-based application designed to manage and analyze customer data efficiently. It simplifies customer relationship management by providing tools for handling customer information, processing data, and managing ticket types.

---

## 🚀 Features

- **Customer Management**:  
  Add, update, and delete customer information using the `customers.py` module.

- **Data Processing**:  
  Handle and manipulate data through the `data.py` module.

- **Hub Integration**:  
  Coordinate operations between different modules using the `hub.py` script.

- **Data Storage**:  
  - **ID Records**: Stored in `id.csv`.
  - **Ticket Types**: Defined in `ticket_types.json`.

---

## 📂 Python Files in the Project

### 1️⃣ `customers.py`

**Purpose**:  
Handles customer-related operations, including creating, updating, and deleting customer records, while ensuring data integrity.

#### **Key Features**:
- **Customer Creation**: Create new customer entries with unique IDs.
- **Customer Updates**: Update existing customer data such as contact details.
- **Customer Deletion**: Safely remove customer records.

---

### 2️⃣ `data.py`

**Purpose**:  
Focuses on data manipulation and transformation. Processes raw data and ensures it is clean and usable.

#### **Key Features**:
- **Data Parsing**: Reads and parses data from files like `id.csv`.
- **Data Transformation**: Cleans and structures data for further processing.
- **Validation**: Ensures data adheres to the required schema.

---

### 3️⃣ `hub.py`

**Purpose**:  
Acts as the central script, integrating functionalities from `customers.py` and `data.py`. It manages the overall workflow of the application.

#### **Key Features**:
- **Module Integration**: Serves as the entry point, invoking functions from other modules.
- **User Interaction**: May contain CLI or GUI-related logic.
- **Control Logic**: Oversees data flow and task orchestration.

---

## 📊 Data Files Supporting the Python Scripts

### 1️⃣ `id.csv`

- **Role**: Stores customer ID data and other related information.
- **Format**: CSV with columns like `ID`, `Name`, `Email`, and `Phone`.

#### **Example**:
```csv
ID,Name,Email,Phone
1,John Doe,johndoe@example.com,555-1234
2,Jane Smith,janesmith@example.com,555-5678
```

### 2️⃣ `ticket_types.json`

- **Role**: Defines ticket types available for customer interactions.
- **Format**: JSON structured as key-value pairs.

## 🔗 How It All Works Together

### **Data Flow**:
1. The `hub.py` file loads data from `id.csv` and `ticket_types.json`.
2. The `data.py` module processes the loaded data to validate and clean it.
3. The `customers.py` module handles CRUD operations on customer records.

### **Integration**:
- **Adding a Customer**:  
  `hub.py` calls the relevant function in `customers.py`.
  
- **Exporting or Validating Data**:  
  `hub.py` leverages functions in `data.py`.

### **Modularity**:
Each Python file has a well-defined role, ensuring the project is clean and easy to maintain.

---

