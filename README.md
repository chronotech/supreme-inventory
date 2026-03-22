# 📦 Supreme Inventory & BOM System

The resource management engine for **Supreme Outdoor Advertising Ltd.** This app handles stock levels, material requisitions, and maintenance tracking for estate assets.

## 🏗️ System Architecture
This app serves as the **Data Provider** for the [Supreme HQ Hub](LINK_TO_YOUR_HQ_REPO).
- **Backend**: Google Sheets (Database) + Apps Script (API).
- **Frontend**: GitHub Pages (Mobile-First Interface).

---

## 🚀 Key Functionalities
- **Live Stock Alerts**: Color-coded indicators (Green/Red) based on minimum threshold values in the Google Sheet.
- **Dynamic Requisitions**: Allows staff to log material usage (Ink/Vinyl) against specific Job IDs.
- **Auto-Sync API**: Provides a real-time list of available items to the Master Hub to prevent manual data entry errors.
- **Asset Management**: Separate tracking for Fairview Farm Estate maintenance (Roof, Plumbing, Infrastructure).

---

## 🔧 Google Apps Script Integration
The `Code.gs` file in the linked Google Sheet handles the following API actions:
- `GET_STATS`: Returns the count of items below critical levels.
- `GET_ITEM_LIST`: Returns a flat array of all active inventory items for the Hub dropdown.
- `CREATE_REQUISITION`: Appends a new row to the 'Log' sheet from the Hub's Quick-Action button.

---

## 📊 Inventory Logic (2026)
- **Primary Warehouse**: Main shop in Red Hills.
- **Thresholds**: Alerts are triggered when `Current Stock` < `Minimum Buffer`.
- **BOM (Bill of Materials)**: Logic to calculate total material cost per square foot for Carnival projects.

---

## 📝 Change Log
- **March 21**: Enabled `GET_ITEM_LIST` endpoint to support the Hub's "Auto-Sync" feature.
- **February 14**: Completed full recalibration of the **YOTTA H3200KJ** Hybrid UV Printer; added maintenance log category.
- **January 20**: Initialized "Offsite" asset tracking category.

---

## 👤 Administrator
**Damian A. Moncrieffe**# supreme-inventory

