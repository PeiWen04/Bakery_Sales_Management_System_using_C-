# 🍪 Cookies and Cakes Sales Management System

A ** object-oriented system** designed for **The Taste A Bites Bakery** to manage the sales, inventory, and membership of cookies and cakes efficiently.
This program streamlines stock tracking, order handling, and payment processes while offering automated discount systems for members and birthday promotions.

---

## 🧠 Overview

The **Cookies and Cakes Sales Management System** is built to automate and simplify daily bakery operations.
It allows:

* Managing stock for cookies and cakes.
* Recording and verifying members.
* Processing orders and applying discounts.
* Generating detailed payment summaries with tax and discount breakdowns.

This program showcases **Object-Oriented Programming (OOP)** principles such as **encapsulation**, **inheritance**, **polymorphism**, and **composition** in managing real-world sales operations.

---

## 🌟 Features

### 🧁 Inventory Management

* Add, load, and update stock data for cookies and cakes.
* Prevents over-purchasing beyond stock quantity.
* Automatically updates inventory after each sale.

### 🛒 Order Handling

* Allows customers to add cookies and cakes to a shopping cart.
* Supports multiple items per order with customizable quantities.
* Displays cart summary for review before payment.

### 👥 Membership Management

* Register new members with personal details and birthdays.
* Verify existing members from stored records.
* Apply automatic **10% member discount** and **30% birthday discount**.

### 💳 Payment and Receipt

* Calculates total, discount, tax (6%), and final payable amount.
* Updates stock files after successful payment.
* Generates a detailed payment record for future reference.

---

## 🎯 System Objectives

This program solves three key operational challenges for bakeries:

1. **Inventory Control** – Track cookies and cakes availability.
2. **Sales Processing** – Automate order calculation and reduce human error.
3. **Customer Loyalty Management** – Enhance customer engagement through discounts and member tracking.

---

## 🧩 OOP Design

| **Class**     | **Description**                            | **Key Responsibilities**                                     |
| ------------- | ------------------------------------------ | ------------------------------------------------------------ |
| **Member**    | Represents a bakery member.                | Verifies identity, checks birthdays, manages registration.   |
| **StockItem** | Represents a single item in stock.         | Stores product ID, name, price, and quantity.                |
| **Stock**     | Manages inventory of cookies and cakes.    | Loads data, finds items, updates quantities, displays lists. |
| **Cart**      | Represents a customer’s shopping cart.     | Adds, removes, and lists cookies and cakes.                  |
| **Payment**   | Handles billing and tax calculations.      | Applies discounts, calculates totals, and updates stock.     |
| **Customer**  | Combines member, stock, cart, and payment. | Represents the complete customer process flow.               |

**Composition & Inheritance Used:**

* `Customer` **contains** `Member`, `Stock`, `Cart`, and `Payment`.
* `Payment` **inherits** from `Member`.
* `Cart` **has** a relationship with `Stock` (composition).

---

## 🔄 Program Flow

1. **Admin Login (Optional)** – Access restricted files and initialize stock files.
2. **Customer Entry** – Identify member or guest.
3. **Membership Verification or Registration** – Verify ID or add new member.
4. **Order Placement** – Add cookies and cakes to the cart.
5. **Payment Processing** – Apply discounts, calculate tax, and show the final bill.
6. **Inventory Update** – Deduct purchased quantities from stock.
7. **Receipt Generation** – Save order details to the payment record file.

---

## 📁 File Structure

```
Cookies-and-Cakes-Sales-Management-System/
│
├── Cookies and Cakes Sales Management System.py   # Main program logic
├── cookiesDetails.txt                             # Cookie inventory file
├── cakeDetails.txt                                # Cake inventory file
├── memberDetails.txt                              # Registered members
├── paymentDetails.txt                             # Payment records
└── README.md                                      # Documentation
```

---

## 💡 Example Scenario

1. The user launches the system.
2. The program asks if they are a member.
3. If they are, the system verifies the ID from `memberDetails.txt`.
4. The available **cookies** and **cakes** are displayed from respective files.
5. The customer adds selected items to the cart.
6. If it’s the customer’s birthday, a **30% discount** is applied; otherwise, a **10% member discount**.
7. The system calculates tax (6%) and total amount.
8. The stock is updated, and a payment receipt is generated in `paymentDetails.txt`.

---

## 💻 Technologies Used

* **Language:** Python (OOP concepts translated from C++ structure)
* **Paradigm:** Object-Oriented Programming
* **Concepts Demonstrated:** Inheritance, Encapsulation, Composition, File I/O
* **Data Storage:** Text-based files for persistence (`.txt`)

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/cookies-and-cakes-sales-system.git
cd cookies-and-cakes-sales-system
```

### 2. Run the program

```bash
python "Cookies and Cakes Sales Management System.py"
```

### 3. Follow on-screen instructions

The system will prompt:

* Whether you’re an admin or a customer
* Member verification or registration
* Adding cookies/cakes to the cart
* Confirming and processing payment



Would you like me to make this README include **GitHub-friendly badges** (for Python version, license, etc.) and a **diagram of the class relationships (UML-style)**?
