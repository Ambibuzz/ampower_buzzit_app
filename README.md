# Ampower Buzzit Community Frappe App

A flexible Frappe app designed to manage visibility of key documents and features in the connected mobile app, empowering users with configurable access to business documents and reports.

---
## 🚀 Overview

**Ampower BuzzIT App** enables dynamic control over what features and doctypes are visible in the mobile application interface. Admin users can easily enable or disable specific doctypes through a simple configuration panel.

This is especially useful when you want to provide a streamlined, role-based mobile experience without altering permissions or the backend logic.

---
## ⚙️ Configuration: `Buzzit Config`

The `Buzzit Config` doctype contains a list of options, each corresponding to a specific document type or feature. Checking or unchecking these options will directly affect the visibility of those features in the mobile app.

### ✅ Available Features in `Buzzit Config`

- Purchase Order
- Purchase Invoice
- Sales Order
- Sales Invoice
- Stock Balance Report
- Customer Ledger Report
- Supplier Ledger Report
- Balance Sheet Report
- View Items
- Workflow

These options are stored as individual boolean fields in the `Buzzit Config` doctype. Changes made in the configuration are reflected immediately in the mobile frontend based on API integration.

---
## 📱 Use Case

Imagine you're an organization where not every employee should have access to every doctype on mobile. With this app:

- Salespeople can view only Sales Orders and Invoices.
- Accountants can access ledgers and balance sheets.
- Warehouse managers can view stock balances and item details.
---

## License

MIT

## 🔧 Installation

```bash
# Navigate to your Frappe bench directory
cd ~/frappe-bench

# Get the app
bench get-app https://github.com/your-org/ampower_buzzit_community_frappe_app --branch master

# Install the app on your site
bench --site your-site-name install-app https://github.com/your-org/ampower_buzzit_community_frappe_app
