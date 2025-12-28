# 🤖 AI Agent – IT Support Ticket Summarization & Email Automation

This project demonstrates an AI-powered automation workflow built with **n8n**, **Airtable**, and **ChatGPT** to streamline IT support operations.

The workflow automatically detects new IT support tickets, summarizes them using an LLM, and sends a concise email notification to IT management.

---

## 🚀 Project Overview

Managing IT support tickets manually can be time-consuming, especially for managers who need quick insights rather than full ticket details.

This automation ensures that:
- Every new ticket is detected automatically
- Ticket details are summarized using AI
- Management receives clear and structured email updates

---

## 🧠 Use Case

**Scenario:**  
An IT Support Team logs tickets in Airtable.  
Whenever a new ticket is created, management should be notified with a short summary.

**Goal:**  
Automate ticket monitoring, summarization, and notification without manual intervention.

---

## 🔄 Workflow Architecture---------------

**Trigger → AI Processing → Notification**

1. **Airtable Trigger**
   - Runs every 1 minute
   - Detects newly created ticket records

2. **AI Model (ChatGPT)**
   - Reads ticket data
   - Generates a professional summary
   - Produces:
     - Email subject
     - Email body (bullet-point format)

3. **Gmail**
   - Sends the AI-generated summary to IT management
   - Email is signed as *IT Support Team*

---

## 🧩 Airtable Schema-------

| Field Name        | Type              |
|------------------|-------------------|
| Ticket ID        | Single line text  |
| User             | Single line text  |
| Issue            | Long text         |
| Priority         | Single select     |
| Date Submitted   | Date              |
| Status           | Single select     |

---

## ✉️ Example Email Output---------

**Subject:** New IT Support Ticket – High Priority  

**Body:**
- Ticket ID: TCK-103  
- User: Celia Nguyen  
- Issue: Printer offline  
- Priority: Low  
- Date Submitted: 2025-02-19  
- Status: Pending  

---

## 🛠️ Tools & Technologies--------

- **n8n** – Workflow orchestration
- **Airtable** – Ticket database and trigger source
- **ChatGPT / LLM** – AI-powered summarization
- **Gmail** – Email delivery

---

## ✅ Benefits

- Fully automated ticket monitoring
- No manual checking of Airtable
- AI-generated summaries save time
- Clear communication with management
- Easily scalable for larger teams