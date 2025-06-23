# 🛒 Python Grocery Store Management System

This is a **3-tier grocery store management application** developed using:

- 🖥️ **Frontend**: HTML, CSS, JavaScript, Bootstrap  
- ⚙️ **Backend**: Python (Flask framework)  
- 🗄️ **Database**: MySQL

The application allows store managers to manage products, units of measurement (UOM), and customer orders efficiently.

![Homepage](homepage.JPG)

---

## 🚀 Features

### ✅ Products Module
- View existing products
- Add new products
- **Edit** product details (💡 newly added based on feedback)
- Delete products
- Add new Units of Measurement (UOM) like **Cubic Meter** (🆕 Backend + Frontend)

### ✅ Orders Module
- Create new customer orders
- Add multiple items per order
- **Frontend validation** for:
  - Empty customer name
  - Invalid product or quantity
- Fix for **grand total calculation bug** (💡 manually editing item price now updates total)
- View detailed order summary including itemized list and price (🆕)

---

## ⚙️ Installation Instructions

### 🔹 Step 1: Set Up MySQL
- Download MySQL for Windows:  
  👉 [MySQL Installer](https://dev.mysql.com/downloads/installer/)
- Create a database named `grocery` and import the required tables (SQL dump provided if available)

### 🔹 Step 2: Install Python Requirements
Install MySQL connector for Python:

```bash
pip install mysql-connector-python

Grocery_Application/
│
├── backend/
│   └── server.py          # Flask server
│
├── frontend/
│   ├── index.html         # Home Page
│   ├── manage-product.html
│   ├── manage-order.html
│   └── css/
│   └── js/
│
├── database/
│   └── grocery_schema.sql # MySQL table definitions (if provided)
│
└── README.md
