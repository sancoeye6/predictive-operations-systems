# Sanco Analytics Engine — Predictive BI Simulator

![Version](https://img.shields.io/badge/version-7.0-blue)
![Status](https://img.shields.io/badge/status-stable-green)
![Architecture](https://img.shields.io/badge/architecture-offline--first-orange)

**Offline-first predictive analytics engine for operational and financial decision modeling.**

Sanco Analytics Engine is a self-contained Business Intelligence application designed to transform raw operational data into actionable insights instantly. Built on a single-file architecture, it runs entirely in the browser with no installation, backend, or internet connection required.

---

## Overview

Healthcare and operations teams often struggle with delayed insights due to fragmented datasets or complex enterprise tools. This engine eliminates the time-to-insight gap by providing real-time analytics, forecasting, and scenario modeling from simple CSV uploads.

The system integrates financial performance with operational efficiency metrics to produce a unified decision dashboard.

---

## Core Capabilities

### Predictive Forecasting
Uses linear regression (least squares method) to generate a 30-day revenue outlook. Includes an R² confidence score indicating prediction reliability.

### Strategic Scenario Simulator
Interactive modeling controls allow real-time adjustments to key variables such as utilization rate, cost inflation, and no-show recovery. Results update instantly to show impact on revenue and margin.

### Operational Intelligence Metrics
Generates high-value KPIs automatically, including:

- Average Hourly Revenue (AHR)
- Accounts Receivable Days
- Margin vs Utilization matrix
- Labor productivity ratios
- Location profitability analysis

### Visual Decision Matrix
Bubble-chart visualization maps service lines by utilization versus margin, making performance outliers immediately visible.

---

## Architecture

This application is built using a **Freeze Logic** design philosophy.

Characteristics:

- Runs entirely client-side
- No server calls
- No data transmission
- Instant calculations
- Works offline after initial load

This ensures maximum privacy, portability, and reliability even in restricted environments.

---

## Technology Stack

Core: HTML5, CSS3, Vanilla JavaScript (ES6+)  
Visualization: Chart.js  
Data Parsing: PapaParse (CSV ingestion)  
Export Engine: SheetJS (Excel generation)  
Styling: Tailwind CSS  

---

## Quick Start

1. Download the HTML file.  
2. Open it in any modern browser.  
3. Upload a CSV dataset.  
4. Dashboard renders instantly.  

No setup. No installation. No configuration.

---

## Expected Data Format

The engine supports flexible column mapping and automatically detects common header names.

Recommended schema:

Date, Location_ID, Service_Line, Total_Revenue, Total_Cost, Patient_Count, Utilization_Pct, Hours_Worked, No_Shows

The parser can also recognize variants such as:

Revenue, Rev, Amount  
Cost, Expense, TotalCost  
Patients, Volume, Visits  

---

## Use Cases

Operational leaders  
Clinic managers  
Financial analysts  
Process engineers  
Performance teams  

Ideal for environments where:

- data must remain local
- speed matters more than infrastructure
- insights are needed immediately
- technical resources are limited

---

## Design Philosophy

This tool was built on three principles:

**Speed over infrastructure**  
**Insight over interface complexity**  
**Privacy over connectivity**

---

## Author

Sanco Isaacs  
Systems Developer and Operational Analyst  

Focus areas:

- Offline-first system design  
- Decision intelligence tooling  
- Human-in-the-loop analytics  
- Operational optimization systems  

---

## License

MIT License
