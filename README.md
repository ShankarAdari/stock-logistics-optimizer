Predictive Stock & Logistics Optimizer (PSLO)
📋 Overview
PSLO is an AI-driven ERP ecosystem designed for high-frequency logistics environments. It leverages real-time data streaming and advanced time-series forecasting to eliminate stockouts and optimize warehouse operations.

✨ Core Innovations
Dual-Engine Forecasting: An ensemble model utilizing ARIMA for seasonal trends and Prophet for promotional growth changepoints.

Feature: Seasonal Decomposition (Trend vs. Seasonality vs. Residuals).

Feature: Demand Lift calculation based on historical promotional data.

WebSocket Infrastructure: Full-duplex communication for real-time inventory updates.

Real-time Sync: Changes made by one warehouse manager are reflected instantly for all others.

Presence Tracking: View who is currently online and which warehouse sector they are managing.

Logistics Route Optimization: Integrated route calculations and cost-per-mile analysis for optimized shipping.

Interactive LLM Analyst: A built-in chat interface that allows managers to query inventory status using natural language (e.g., "Which products are at risk of an anomaly this week?").

📊 Technical Architecture
Frontend: React 19, Tailwind CSS 4, Framer Motion (Animations), Recharts (Live Data Viz).

Backend: Node.js, Socket.io (WebSockets), Express.

Database: MySQL with Drizzle ORM.

New Tables: promotionalEvents, seasonalPatterns, forecastMetrics.

Forecasting: Python-based microservice utilizing Scikit-learn, ARIMA, and Seasonal Decomposition logic.

Testing: 25+ Vitest suites covering WebSocket event loops and reporting logic.

🌍 Real-World Business Value
Reduction in Overstock: By identifying seasonal patterns, businesses reduce capital tied up in slow-moving inventory.

Instant Response: Real-time anomaly alerts allow for immediate correction of supply chain bottlenecks.

Collaborative Efficiency: The WebSocket layer prevents "double-ordering" and communication gaps between multi-site teams.

🚀 Quick Start
Clone & Install:

Bash

git clone https://github.com/yourusername/stock-logistics-optimizer.git
npm install
Database Sync:

Bash

npx drizzle-kit push:mysql
Run with Live Updates:

Bash

npm run dev
