# Zerodha Clone - Full Stack Trading Platform

A comprehensive full-stack stock trading and investment platform clone based on Zerodha. This project is architected into three distinct applications: a robust backend API, an interactive user dashboard for trading, and a complete marketing-focused landing website.

## 🚀 Features

### Core Functionality

* **Portfolio Management:** Track user holdings, active market positions, and available account funds directly through a dedicated trading dashboard (`Holdings.js`, `Positions.js`, `Funds.js`).


* **Order Execution:** Manage trade executions using a dedicated buy action window and track complete trade history (`BuyActionWindow.js`, `Orders.js`).


* **Market Tracking & Visualization:** Monitor stocks using a custom watchlist (`WatchList.js`) and visualize portfolio allocations through doughnut charts and vertical graphs (`DoughnoutChart.js`, `VerticalGraph.js`).


* **Public-Facing Web Portal:** A complete marketing frontend featuring pricing details, product showcases, an about section, and a customer support portal for creating tickets (`PricingPage.js`, `ProductsPage.js`, `CreateTicket.js`).



## 🛠️ Technology Stack

**Backend & Data Processing**

* **Node.js:** Powers the core backend server logic (`index.js`).


* **MongoDB:** Serves as the primary database, securely configured via environment variables (`MONGO_URL`), storing critical financial data.


* **Mongoose (Inferred):** Utilizes structured schemas and models to cleanly manage `Holdings`, `Orders`, and `Positions`.



**Frontend Architecture**

* **React.js:** Component-based UI architecture driving both the public frontend and the secure dashboard (evidenced by the `.js` component structure and `public/index.html` files).


* **State Management:** Utilizes React Context API for managing global application state (`GeneralContext.js`).


* **Styling:** Modular CSS integration for component-specific designs (`BuyActionWindow.css`, `index.css`).



## 📁 Project Architecture

**Modular Monorepo Structure**
The codebase is cleanly separated into three primary environments to ensure separation of concerns:

1. **`backend/`**: Contains all server-side logic, database schemas, and connection configurations.


2. **`dashboard/`**: The secure, authenticated Single Page Application (SPA) where users interact with their charts, watchlists, and place trades.


3. **`frontend/`**: The static/public landing application housing SEO-friendly pages like Home, About, Signup, and Brokerage details.



**Database Schema Design**
The data layer is strictly organized into distinct models to accurately reflect a real trading environment, featuring separated schemas for `HoldingsSchema.js`, `OrdersSchema.js`, and `PositionsSchema.js`.
