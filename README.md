# 🏢 KAEFER Employee Utility & Support Portal

A lightweight, multi-lingual web portal built to help KAEFER Saudi Arabia employees estimate monthly payroll/overtime amounts and easily register salary or site queries.

🔗 **Live Portal Link:** [https://tinyurl.com/kaefer-portal](https://tinyurl.com/kaefer-portal)  
📌 **GitHub Pages URL:** [https://supportkaefer.github.io/KAEFER-s-Portal/](https://supportkaefer.github.io/KAEFER-s-Portal/)

---

## 🌟 Key Features

* **🧮 Overtime & Payslip Calculator**
  * Automated base rate and overtime calculation according to 240-hour monthly basis.
  * Supports **Normal OT (1.5x)**, **Holiday OT (1.5x)**, **Retro Normal OT**, **Retro Holiday OT**, and **Bonus OT (1.0x)**.
  * Built-in support for **25th Monthly Pay Cutoff Rules** (separating current month OT from previous month retro OT).
  * Includes configurable allowances and instant gross/net breakdown previews.

* **🎫 Support & Issue Tracking System**
  * Simple, worker-friendly issue registration form.
  * Generates a unique **Support Ticket ID** (e.g., `T-582910`) upon submission.
  * Real-time ticket status tracking and direct follow-up / reopening option if not resolved.
  * Powered by a real-time Google Sheets backend for HR and support teams.

* **🌐 Multi-Language Accessibility**
  * Instant 1-click language toggling for **English**, **Arabic (العربية)**, **Hindi (हिंदी)**, and **Urdu (اردو)**.
  * Automatic Text Direction (RTL/LTR) support for simplified navigation across all nationalities.

---

## 🏗️ System Architecture

┌────────────────────────────────┐
                           │   GitHub Pages Frontend        │
                           │   (HTML5, Tailwind CSS, JS)    │
                           └───────────────┬────────────────┘
                                           │
                            ┌──────────────┴──────────────┐
                            ▼                             ▼
                 ┌──────────────────┐          ┌──────────────────┐
                 │ OT & Payslip     │          │ Ticket Submission│
                 │ Calculation      │          │ & Tracking Engine│
                 │ Engine (Local)   │          └──────────┬───────┘
                 └──────────────────┘                     │
                                                          │ Async JSON Fetch
                                                          ▼
                                               ┌────────────────────┐
                                               │ Google Apps Script │
                                               │ Webhook Engine     │
                                               └──────────┬─────────┘
                                                          │
                                                          ▼
                                               ┌────────────────────┐
                                               │ Google Sheets DB   │
                                               │ (Support Dashboard)│
                                               └────────────────────┘

---

## ⚠️ Important Notice & Disclaimer

> **PLEASE NOTE:** This portal is an **unofficial, community-built utility** operating under **Test Mode** for limited sites. It is intended to assist employees with quick estimations and streamline support follow-ups. All calculations are approximate reference figures; official earnings remain subject to SAP payroll processing.

---

## 🛠️ Technology Stack

* **Frontend:** Single-page app hosted via **GitHub Pages** (HTML5, Tailwind CSS, FontAwesome, Vanilla JS).
* **Backend:** **Google Apps Script** deployed as a Web App API endpoint.
* **Database / Admin Dashboard:** **Google Sheets** for real-time ticket review, HR notes, and task resolution.
