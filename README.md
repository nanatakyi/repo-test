# MarketFlow POS – Frontend Prototype

A responsive supermarket/retail Point of Sale website prototype.

## Included
- Dashboard with sales and payment overview
- POS checkout with product search, category filters, basket quantities and payment selection
- Product catalogue and add-product form
- Inventory overview and stock status
- Customers, suppliers, sales, reports, staff and settings screens
- CSV exports for products and sales
- Online/offline connection indicator
- Browser-local queue demonstration for offline transactions

## Run the website
This is a static frontend prototype. No build tools are required.

1. Extract the project folder.
2. Open `index.html` in a modern browser, or serve the folder with a local web server.
3. For example, if Python is installed, open a terminal in this folder and run:

   ```bash
   python -m http.server 8000
   ```

4. Visit http://127.0.0.1:8000

## Important prototype limitations
This is a frontend demonstration, not a production POS system. Demo records are stored in JavaScript and most changes are held only in the current browser session. Offline transactions are demonstrated with browser local storage, but there is no server synchronization yet.

The next development phase is to create the Django REST Framework backend, PostgreSQL database, authentication/permissions, persistent sales and stock transactions, and a secure synchronization API. Mobile Money and card payments must be connected to an approved payment provider before real payments can be accepted. Never treat an unverified payment as successful.

## Planned production architecture
- Frontend: React (the current prototype uses HTML, CSS and JavaScript for easy preview)
- Backend: Python Django + Django REST Framework
- Database: PostgreSQL
- Offline storage: IndexedDB + service worker
- Containers: Docker
- Version control: Git/GitHub
- Currency: Ghana cedi (GHS)
