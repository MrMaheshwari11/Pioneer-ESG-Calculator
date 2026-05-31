# Pioneer Hospitality Services- Interactive ESG Catering Calculator

## Overview
This repository contains the working prototype for the Interactive ESG Catering Calculator, developed for Task 10.3HD. This feature allows corporate facility managers to build a weekly employee meal plan and instantly track the nutritional breakdown and carbon footprint (CO2e) of their choices in real-time.

## Technical Implementation
This feature was designed as a lightweight, single-page application to ensure zero server latency during interaction. It is entirely contained within `index.html`.

### Technologies Used:
* **HTML5 & CSS3 (Bootstrap 5.3):** Used for a responsive, card-based layout and modern UI components.
* **Vanilla JavaScript:** Handles the DOM manipulation, array filtering, and real-time mathematical calculations for the macros and emissions.
* **Chart.js:** A lightweight JavaScript charting library used to render the animated Doughnut and Bar charts.

### How it Operates:
1. **Data Structure:** The menu items and their associated metrics (calories, CO2 grams, water liters) are stored in a structured JSON array within the script.
2. **Event Listeners:** When a user clicks the `+` or `-` quantity buttons, a JavaScript function (`updateQty`) updates the state.
3. **Real-time Rendering:** The `calculateTotals()` function loops through the updated quantities, calculates the new totals, and dynamically updates the HTML text and the Chart.js instances instantly.

### How to Run
Simply download or clone this repository and open `index.html` in any modern web browser. No local server or dependency installation is required.
