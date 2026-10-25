# Arcadia E-Commerce Shopping Cart

A modern React JS shopping cart application built with Vite, React Router, Axios, and LocalStorage-based cart persistence.

## Features

- Home page with hero banner and featured products
- Product listing with search, category filters, and sorting
- Product detail page with quantity selection and add-to-cart flow
- Cart page with quantity updates, removal, and live totals
- Checkout form with validation and demo order confirmation
- Login and registration UI pages with validation and password toggle
- Responsive layout for mobile, tablet, and desktop screens
- LocalStorage persistence for cart data

## Tech Stack

- React JS
- Vite
- React Router DOM
- Axios
- Lucide React
- CSS3

## Installation

```bash
npm create vite@latest ecommerce-shopping-cart -- --template react
cd ecommerce-shopping-cart
npm install
npm install react-router-dom axios lucide-react
```

## Run the App

```bash
npm run dev
```

Then open the local URL shown in the terminal, usually http://localhost:5173.

## Build for Production

```bash
npm run build
```

## Project Structure

```text
src/
  components/
    Navbar.jsx
    Footer.jsx
    ProductCard.jsx
    ProductGrid.jsx
    SearchBar.jsx
    CategoryFilter.jsx
    Loading.jsx
  context/
    CartContext.jsx
  pages/
    Home.jsx
    Products.jsx
    ProductDetails.jsx
    Cart.jsx
    Checkout.jsx
    Login.jsx
    Register.jsx
    OrderConfirmation.jsx
    NotFound.jsx
  services/
    productService.js
  utils/
    storage.js
  App.jsx
  App.css
  main.jsx
  index.css
```

## API Integration

The app uses the public Fake Store API:

- Base URL: https://fakestoreapi.com/products
- Product listing: GET /products
- Product detail: GET /products/:id
- Categories: GET /products/categories

## Notes

- Checkout is a UI demonstration and does not process real payments.
- Authentication pages are demo-only screens and do not connect to a backend.
- Cart items persist after refresh using LocalStorage.
