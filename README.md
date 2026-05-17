

https://github.com/user-attachments/assets/2bb7c426-e5ab-4b2c-bdac-4e9052bb6d29



Uploading 20260517172833.mp4…

# 🌍 Geographic Customer Mapping Tool (Geospatial Sales Intelligence CRM)

A premium, interactive geospatial data visualization tool designed for sales, operations, and CRM teams. It dynamically processes customer addresses and direct Google Maps coordinates to plot color-coded, interactive markers on a highly polished map interface, enabling data-driven regional planning, customer density analysis, and routing optimization.

---

## ✨ Key Features

- **📍 Pinpoint Accuracy Mapping:** Supports direct latitude/longitude coordinate parsing from Google Maps for 100% millimeter-precise customer placements.
- **🔍 Intelligent Address Geocoding:** Integrates with an advanced ArcGIS World Geocoding Engine to automatically resolve hierarchical Arabic/English addresses (`Building, Street, District, Governorate, Country`) into geographical coordinates.
- **⚡ Bulletproof Excel/CSV Auto-Import:** Dynamically imports bulk client datasets using SheetJS (`XLSX`).
  - **Fuzzy Synonyms Matching:** Intuitively maps varied column headers (e.g., *الاسم / اسم العميل / الشركة / Name / Client*).
  - **Zero Arabic Encoding Loss:** Uses modern `ArrayBuffer` reading to completely prevent Arabic UTF-8 string corruption.
  - **Smart Throttle Queue:** Auto-throttles requests (800ms-1.5s delay) to safely process lists without IP rate-limiting or blocking.
- **📊 Real-time Geographic Analytics:** 
  - Interactive **Doughnut charts (Chart.js)** displaying client distribution across Governorates.
  - High-impact visual indicators tracking status (✅ *Completed/Success*, ⏳ *Under Negotiation/Pending*, ❌ *Rejected*).
- **🗂️ Interactive Geospatial CRM Drawer:** A fully responsive sidebar listing recently mapped clients with full address details, status badges, and fly-to animation triggers.
- **🛡️ Custom Animated Modal Dialogs:** Features custom confirmation modals with smooth glassmorphic blur and scale transitions, completely replacing generic browser alerts.

---

## 🛠️ Tech Stack & Architecture

- **Core Frontend:** HTML5 (Semantic Structure), Tailwind CSS (Premium Modern Styling)
- **Mapping Engine:** LeafletJS (High-Performance GIS Engine) & CartoCDN Voyager Maps
- **Data Handling:** SheetJS (XLSX parsing), Chart.js (Data Visualization)
- **Geocoding API:** ArcGIS World Geocoding REST Service
- **Components:** Responsive CRM Drawer, Custom Confirmation Modals, Interactive Maps

---

## 📂 Project Structure

```bash
├── index.html          # Core Geospatial Dashboard & Map View
├── registry.html       # Regional CRM Registry, Statistics & Governorate Charts
├── app.js              # State Management, Geocoding Engine, and Excel Parser
├── generate_samples.py # Python script for generating mock sales datasets (Excel/Word)
└── README.md           # Professional documentation
```

---

## 🚀 Getting Started

### 1. Run the Project Locally
Simply clone the repository and open `index.html` in any web browser. No server configuration or API keys required!
```bash
# Clone the repository
git clone https://github.com/ibrahimserry24/geographic-customer-mapping-tool.git

# Open index.html in your browser
# (Double-click or drag into browser window)
```

### 2. Format of Excel Import
The smart importer automatically maps columns based on keywords, but here is the recommended template header layout:
| اسم العميل (Client) | المحافظة (Gov) | المنطقة (District) | الشارع (Street) | رقم العمارة (Building) | الحالة (Status) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| شركة النور | القاهرة | مدينة نصر | عباس العقاد | 15 | مكتمل |
| كافيه بلوم | القاهرة | التجمع الخامس | التسعين الشمالي | 2B | تفاوض |

---

## 📸 Screenshots & Showcase
*Developed by **Ibrahim Serry** as part of a high-impact AI Software Engineering portfolio. Specialized in combining robust Python backend workflows, clean data scraping pipelines, and stunning, user-focused GIS interfaces.*
