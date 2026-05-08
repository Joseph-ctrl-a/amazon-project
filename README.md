# Amazon Project

A fully functional Amazon-like e-commerce web app built with vanilla JavaScript, HTML, and CSS.

## Background

This was my first real JavaScript project — my first time working with JS at any meaningful scale. Before this, I had only written small scripts; this project was where I got hands-on experience with the things that actually matter when building something larger:

- **File structure** — figuring out how to organize a codebase so it doesn't become a mess
- **ES6 modules** — importing and exporting across files to keep concerns separated
- **Object-Oriented Programming** — building classes like `Product`, `Cart`, and `Track` and understanding when OOP actually helps
- **State management** — keeping cart and order data consistent across multiple pages using localStorage
- **Working with APIs** — fetching product data and posting orders to a real backend

## Features

- Browse a product catalog fetched from a live API
- Add items to a persistent shopping cart (survives page refresh)
- Select delivery options with accurate date calculations (weekend-aware)
- Place orders and review them in an order history page
- Track individual packages with a visual progress bar
- Responsive layout that adapts from mobile to wide desktop

## Tech Stack

- **Vanilla JavaScript (ES6 modules)** — no frameworks
- **HTML5 / CSS3** — Flexbox and CSS Grid for layout
- **localStorage** — client-side state persistence
- **dayjs** — date formatting and arithmetic
- **Jasmine** — unit testing
- **supersimplebackend.dev** — external REST API for products and orders

## Running the Project

No build step required. Open the project with a local dev server — the VS Code [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension works well (configured for port 5501).

Navigate to `index.html` to start on the product listing page.

To run the tests, open `tests/SpecRunner.html` in the browser.

## Pages

| Page            | File            | Description                               |
| --------------- | --------------- | ----------------------------------------- |
| Product Listing | `index.html`    | Browse and add items to cart              |
| Checkout        | `checkout.html` | Review cart, choose delivery, place order |
| Orders          | `orders.html`   | View order history                        |
| Tracking        | `tracking.html` | Track a specific package                  |
