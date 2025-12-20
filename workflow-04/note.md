# Smart Car Dealership Automation

## 📌 Description
This workflow automates a smart car dealership process. Every time a car is sold, the system automatically notifies the dealership owner via email and records the sale details in a Google Sheet.

## ⚙️ Trigger
- **Webhook**
- The workflow starts whenever a sale event is received through an HTTP request.

## 🔄 Workflow Steps
1. **Webhook Trigger** – Receives car sale data such as car model, price, and buyer information.
2. **Gmail: Send Message** – Sends an email to the dealership owner with the sale details.
3. **Google Sheets: Append Row** – Stores the sale data in a Google Sheet for record-keeping.

## 🧰 Services Used
- Gmail
- Google Sheets

## 🎯 Use Case
Ideal for car dealerships or sales teams that want to automate notifications and maintain a structured sales log without manual data entry.

## 📝 Notes
- Requires OAuth credentials for Gmail and Google Sheets.
- Google Sheet must have predefined column headers matching the sale data.
- This workflow does not use AI agents and focuses on simple automation.
