# HandsMen Threads - Inventory Management Automation

**HandsMen Threads** is an automated inventory management solution built on Salesforce. It uses Apex triggers and workflows to maintain real-time stock levels and calculate total inventory values, streamlining manual operations.

---

## 📁 Project Structure

HandsMen-Threads/  
│  
├── screemshots/                  # Project screenshots  
├── source code/                  # Apex triggers and related code  
│   ├── stock_deduction_trigger.trigger  
│   └── update_total_trigger.trigger  
├── HandsMen Threads project documentation.docx  
└── readme.md                     # Project README  

---

## ⚙️ Features

- **Real-Time Stock Management**: Automatically updates stock on purchase or sale events.
- **Dynamic Total Calculation**: Keeps track of total product value based on current stock and unit prices.
- **Trigger-Based Automation**: Uses custom Apex triggers for seamless inventory operations.

---

## 🔧 Apex Triggers

### 1. `stock_deduction_trigger`
**Purpose**:  
Handles automatic deduction of stock from the inventory whenever a transaction or order is created.

**Functionality**:
- Triggered after insert operations on the transaction object.
- Deducts the ordered quantity from available stock.
- Ensures stock does not go negative.

---

### 2. `update_total_trigger`
**Purpose**:  
Calculates and updates the total inventory value for each product after stock changes.

**Functionality**:
- Triggered after insert or update on the stock object.
- Multiplies stock quantity by unit price to compute `Total_Value__c`.
- Keeps the total value field updated in real time.

---

## 📸 Screenshots

Find all relevant UI and setup screenshots in the `screemshots/` folder.

---

## 📄 Documentation

For complete functional explanation and implementation details, refer to the file:  
**`HandsMen Threads project documentation.docx`**

---

## 📌 Requirements

- Salesforce Developer Edition
- Basic knowledge of Apex Triggers and Salesforce Objects
- Admin permissions to modify object schema

---

## 🧑‍💻 Author

**Rahul Koranga**  
📧 rahulkoranga30@gmail.com  
📍 Clement Town, Dehradun

---
