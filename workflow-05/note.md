# Hotel Reservation Automation

## 📌 Description
This workflow automates the hotel reservation process by capturing guest booking details through a form submission and saving the reservation data into Airtable for easy management and tracking.

## ⚙️ Trigger
- **Form Submission (n8n)**
- The workflow starts when a guest submits the reservation form.

## 🔄 Workflow Steps
1. **Form Submission Trigger** – Collects guest information such as name and selected room type.
2. **Airtable: Add Record** – Saves the reservation details as a new record in an Airtable base.

## 🧰 Services Used
- n8n Forms
- Airtable

## 🎯 Use Case
Ideal for hotels or guesthouses that want to collect room reservations digitally and maintain a centralized booking database without manual data entry.

## 📝 Notes
- Requires Airtable API credentials.
- Airtable base and table must be created in advance with matching fields.
- The reservation form must include required inputs such as guest name and room type.

