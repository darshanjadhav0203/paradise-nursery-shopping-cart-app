# Paradise Nursery - Shopping Application

Welcome to **Paradise Nursery**, an e-commerce web application where green meets serenity! This application allows users to browse a wide variety of houseplants, learn about their unique benefits, add them to their shopping cart, and manage their orders dynamically with Redux Toolkit.

---

## 🌿 Project Overview

Paradise Nursery is designed to bring nature closer to your home and workspace. The application features:
- **Landing Page**: An inviting entrance introducing Paradise Nursery with background imagery, mission statement, and a "Get Started" call-to-action button.
- **Product Catalog**: A plant directory grouped into distinct categories (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, and Low Maintenance), featuring thumbnail images, prices, descriptions, and dynamic "Add to Cart" functionality.
- **Dynamic Shopping Cart**: Real-time cart tracking with badge count, quantity increment/decrement controls, item removal, cost breakdown per item, total cart calculation, and checkout navigation.

---

## ✨ Features

1. **Landing Page (`App.jsx`, `AboutUs.jsx`, `App.css`)**:
   - High-definition greenhouse background image with elegant overlay.
   - Company branding with title, subtitle, and informative "About Us" section.
   - Smooth transition into the product catalog upon clicking "Get Started".

2. **Product Listing (`ProductList.jsx`)**:
   - Over 30 unique indoor plants organized across 5 specialized categories.
   - Responsive cards displaying plant thumbnail, title, description, and price.
   - "Add to Cart" button that disables and updates text once added to prevent duplicate additions.
   - Fixed navigation bar with brand logo, "Plants" catalog link, and cart icon.
   - Dynamic cart quantity badge displaying the total item count in real-time.

3. **Shopping Cart Management (`CartSlice.jsx`, `CartItem.jsx`)**:
   - Centralized global state management using **Redux Toolkit**.
   - `addItem`: Adds plant to cart or increments quantity.
   - `removeItem`: Removes specific plant from cart.
   - `updateQuantity`: Adjusts plant quantity with increment and decrement buttons.
   - Auto-calculated subtotal per plant and total bill for the cart.
   - "Continue Shopping" button returning directly to the catalog.
   - "Checkout" button with instant user notification.

---

## 🛠️ Technology Stack

- **React 18** - Frontend UI library
- **Redux Toolkit** & **React-Redux** - Global state management
- **Vite** - High-performance frontend build tool and dev server
- **HTML5 & CSS3** - Semantic structure and responsive styling

---

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed on your system (v16 or higher recommended).

### Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate into the project folder:
   ```bash
   cd e-plantShopping
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally

To run the development server:
```bash
npm run dev
```
Open your browser and navigate to `http://localhost:5173` (or the port specified in your terminal).

### Building for Production

To create a production-ready build:
```bash
npm run build
```

---

## 📁 Project Structure

```text
├── public/                 # Static assets
├── src/
│   ├── assets/             # Images and media
│   ├── AboutUs.css         # About Us component styling
│   ├── AboutUs.jsx         # Company mission and background info
│   ├── App.css             # Landing page and global layouts
│   ├── App.jsx             # Main landing page & catalog view toggle
│   ├── CartItem.css        # Shopping cart view styles
│   ├── CartItem.jsx        # Shopping cart items and total calculation
│   ├── CartSlice.jsx       # Redux Toolkit slice for cart state
│   ├── ProductList.css     # Product cards and navigation styles
│   ├── ProductList.jsx     # Plant catalog grouped by category
│   ├── index.css           # Global CSS variables and resets
│   ├── main.jsx            # React root and Redux store provider
│   └── store.js            # Redux store configuration
├── index.html              # HTML entry point
├── package.json            # Project dependencies and scripts
├── vite.config.js          # Vite configuration
└── README.md               # Project documentation
```

---

## 📄 License

This project is licensed under the MIT License.