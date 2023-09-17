# Flask-Angular-OLAP-Retail-Analytics-Dashboard

A full-stack Business Intelligence dashboard for multi-dimensional retail sales and inventory analytics, built during a software engineering internship (Sept-Dec 2023).

## 🎯 Project Overview

This application provides comprehensive analytics for retail business operations across multiple dimensions (Store, Time, Customer, Item) using OLAP (Online Analytical Processing) techniques.

## 🏗️ Architecture

### Backend (Python Flask API)
- **Flask** REST API running on `localhost:5000`
- **Pandas & NumPy** for data processing and analytics
- **Flask-CORS** for cross-origin resource sharing
- Modular service architecture with separate query services

### Frontend (Angular 14)
- **Angular 14** single-page application
- **Bootstrap 5** for responsive UI design
- **Chart.js & ng2-charts** for data visualizations
- **DataTables** for interactive data tables
- **Bootstrap Icons** for UI components

## 📊 Features

### Core Business Queries (Q1-Q10)

1. **Q1** - Division/District-wise Sales Analysis
2. **Q2** - Payment Method Analysis (Cash/Mobile/Card)
3. **Q3** - Regional Sales (Barisal Division)
4. **Q4** - Yearly Sales Performance (2015)
5. **Q5** - Regional Yearly Analysis (Barisal 2015)
6. **Q6** - Top 3 Products per Store
7. **Q7** - Products Sold Within X Days
8. **Q8** - Worst Performing Season per Product
9. **Q9** - Geographic Sales Distribution (Division-wise)
10. **Q10** - Average Monthly Sales per Store

### Financial Analytics (Time-based Comparisons)

- **Store Financial Performance** - Revenue comparison across time periods
- **Customer Financial Metrics** - Customer spending pattern analysis
- **Item Financial Analysis** - Product profitability tracking

### Inventory Analytics (Time-based Comparisons)

- **Store Inventory Levels** - Stock tracking across stores
- **Item Inventory Movement** - Product stock level monitoring

## 🛠️ Technology Stack

### Backend
- Python 3.x
- Flask
- Pandas
- NumPy
- Flask-CORS

### Frontend
- Angular 14
- TypeScript
- Bootstrap 5.2
- Chart.js
- DataTables.net
- jQuery

## 📁 Project Structure
```
.
├── 1.api/                          # Backend API
│   ├── app.py                      # Flask application entry point
│   ├── router.py                   # API route definitions
│   ├── requirements.txt            # Python dependencies
│   ├── DBconnection/               # Database connection logic
│   ├── QueryController/            # HTTP request handlers
│   └── QueryServices/              # Business logic services
│
└── frontend/                       # Angular frontend
    ├── src/app/components/         # Angular components
    ├── src/app/services/           # Angular services
    └── src/assets/                 # Static assets
```

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Node.js 14+
- npm or yarn

### Backend Setup
```bash
cd 1.api

# Install dependencies
pip install -r requirements.txt

# Run the Flask API
python app.py
```

The API will be available at `http://localhost:5000`

### Frontend Setup
```bash
cd frontend

# Install dependencies
npm install

# Run development server
ng serve
```



## 🔌 API Endpoints

### Core Queries
- `GET /api/q1` - Division-wise sales
- `GET /api/q1dis` - District-wise sales
- `GET /api/q2` - Transaction type sales
- `GET /api/q3` - Barisal total sales
- `GET /api/q4` - 2015 total sales
- `GET /api/q5` - Barisal 2015 sales
- `GET /api/q6` - Top 3 products per store
- `GET /api/q7` - Products sold since X days
- `GET /api/q8` - Worst season per product
- `GET /api/q9` - Geographic sales distribution
- `GET /api/q10` - Average monthly sales

### Financial Analytics
- `GET /api/financialStoreTime1` - Store financial metrics (Period 1)
- `GET /api/financialStoreTime2` - Store financial metrics (Period 2)
- `GET /api/financialCustomerTime1` - Customer financial metrics (Period 1)
- `GET /api/financialCustomerTime2` - Customer financial metrics (Period 2)
- `GET /api/financialItemTime1` - Item financial metrics (Period 1)
- `GET /api/financialItemTime2` - Item financial metrics (Period 2)

### Inventory Analytics
- `GET /api/inventoryStoreTime1` - Store inventory (Period 1)
- `GET /api/inventoryStoreTime2` - Store inventory (Period 2)
- `GET /api/inventoryItemTime1` - Item inventory (Period 1)
- `GET /api/inventoryItemTime2` - Item inventory (Period 2)

## 📊 Data Dimensions

The system analyzes data across multiple dimensions:

- **Time Dimension** - Date, Month, Quarter, Year
- **Geography Dimension** - Division, District
- **Store Dimension** - Store ID, Location
- **Product Dimension** - Item, Category, Supplier
- **Customer Dimension** - Customer segments and behavior

## 🎓 Learning Outcomes

This internship project demonstrates:

- Full-stack development with modern frameworks
- RESTful API design and implementation
- Data warehousing and OLAP concepts
- Multi-dimensional data analysis
- Business Intelligence dashboard development
- Responsive UI/UX design
- Data visualization techniques

## 📝 Development Timeline

- **September 2023** - Project setup, core architecture, basic queries (Q1-Q5)
- **October 2023** - Advanced queries (Q6-Q10), data processing optimization
- **November 2023** - Financial analytics modules, time-based comparisons
- **December 2023** - Inventory analytics, UI enhancements, final testing

## 🤝 Contributing

This project was developed as part of a software engineering internship. Contributions, issues, and feature requests are welcome!

## 👨‍💻 Developer

Developed during Data Analytics Internship (September - December 2023)

---

**Note**: This is an academic internship project demonstrating full-stack development and business intelligence capabilities.
