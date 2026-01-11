
# Purchase Order & Invoice System (Node.js)

This is a **console-based Purchase Order and Invoice Management System** built using **Node.js**.
It simulates how purchase orders are created, invoices are generated, and payments are tracked.

---

## Features

* Create **Purchase Orders (PO)** with unique IDs
* Supports **hourly, daily, and monthly** payment types
* Automatically calculates total amount
* Generate **invoices only after training completion**
* Track invoice status: `UNPAID`, `PAID`, `OVERDUE`
* Simulate **overdue invoice checks**
* Interactive **command-line menu**

---

## Technologies Used

* JavaScript (Node.js)
* `readline` module (CLI interaction)
* In-memory object as database (simulation)

---

## How to Run

1. Make sure **Node.js** is installed
2. Save the file as `app.js`
3. Run the program:

   ```bash
   node app.js
   ```

---

## Available Commands

| Command    | Description                  |
| ---------- | ---------------------------- |
| `po`       | Create a new Purchase Order  |
| `invoice`  | Generate invoice using PO ID |
| `pay`      | Mark an invoice as PAID      |
| `test`     | Simulate overdue invoice     |
| `test-due` | Simulate due-soon invoice    |
| `exit`     | Exit the application         |

---

## Purchase Order Details

* PO Number (Auto-generated)
* Course Name
* Client Name
* Trainer Details
* Payment Type & Rate
* Start & End Dates
* Total Amount

---

## Invoice Rules

* Invoice can be generated **only after end date**
* Due date = **30 days from invoice date**
* Overdue invoices are automatically detected
* Email notification is **simulated via console logs**

---

## Notes

* This project uses **in-memory storage** (data resets on restart)
* Designed for **learning & system design demonstration**
* Can be extended to real databases and payment gateways

---

## Sample Use Case

1. Create a PO using `po`
2. Wait until training end date (or simulate)
3. Generate invoice using `invoice`
4. Mark payment using `pay`
5. Check overdue invoices automatically
