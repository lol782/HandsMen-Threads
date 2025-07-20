# HandsMen Threads - Inventory Management Automation

**HandsMen Threads** is an automated inventory management solution built on Salesforce. It uses Apex triggers and workflows to maintain real-time stock levels and calculate total inventory values, streamlining manual operations.

---

## 📁 Project Structure

HandsMen-Threads/  
│  
├── screemshots/                   Project screenshots  
├── source code/                   Apex triggers and related code  
│   ├── stock_deduction_trigger.trigger  
│   └── update_total_trigger.trigger  
├── HandsMen Threads project documentation.docx  
└── readme.md                      Project README  
---

## ⚙️ Features

- **Real-Time Stock Management**: Automatically updates stock on purchase or sale events.
- **Dynamic Total Calculation**: Keeps track of total product value based on current stock and unit prices.
- **Trigger-Based Automation**: Uses custom Apex triggers for seamless inventory operations.

---

## 🔧 Apex Triggers

### 1. `stock_deduction_trigger`
**Purpose**:  
This trigger handles the automatic deduction of stock from the inventory whenever a new transaction or order is created. It ensures the inventory is always up to date without any manual intervention.

**Functionality**:
- Runs after an insert operation on the transaction object.
- Deducts the quantity ordered from the current stock.
- Prevents stock from going negative.

---

### 2. `update_total_trigger`
**Purpose**:  
This trigger calculates and updates the total value of inventory for each product after every stock update.

**Functionality**:
- Runs after an update or insert on the stock object.
- Multiplies the current stock quantity by the unit price to compute the total value.
- Updates the `Total_Value__c` field of the product.

---

## 📸 Screenshots

Refer to the `screemshots` folder for UI and workflow visuals.

---

## 📄 Documentation

Detailed explanation of project requirements, implementation details, and logic flow is available in the file:  
**`HandsMen Threads project documentation.docx`**

---

## 📌 Requirements

- Salesforce Developer Org
- Basic understanding of Apex Triggers
- Admin access to create objects and fields

---

## 🧑‍💻 Author

Rahul Koranga  
📧 rahulkoranga30@gmail.com  
📍 Clement Town, Dehradun

---
