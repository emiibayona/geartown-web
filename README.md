# GearTown Web | [🔗 Visit](https://geartown.store)

Frontend application for **GearTown**, a Trading Card Game (TCG) platform built to manage products, collections and store operations.

The project started as a website for a local card store and gradually evolved into a larger application with public storefronts, authenticated areas and administrative tools. It currently supports multiple TCGs while keeping a shared and reusable architecture.

---

## Features

* Public storefront for multiple Trading Card Games
* Product browsing and filtering
* Shopping cart
* Personal collection management
* Administrative dashboard
* Inventory management
* Sales management
* User authentication

Currently supported games include:

* Magic: The Gathering
* Yu-Gi-Oh!
* Pokémon
* Riftbound

---

## Tech Stack

### Frontend

* Vue.js 3
* Pinia
* Tailwind CSS
* Sass
* Vite

### Utilities

* Vercel Analytics

---

## Project Structure

```text
src/
│
├── assets/          Global styles and static resources
├── components/      Reusable UI components
├── composables/     Reusable business logic
├── pages/           Route-based application pages
├── router/          Vue Router configuration
├── services/        API communication layer
├── stores/          Pinia state management
├── utils/           Shared utilities
└── sections/        Large reusable page sections
```

The application follows a modular architecture where each layer has a single responsibility:

* **Pages** are responsible for rendering complete views.
* **Components** encapsulate reusable UI elements.
* **Composables** contain reusable business logic using Vue Composition API.
* **Services** centralize communication with the backend API.
* **Stores** manage shared application state using Pinia.
* **Utils** contain helper functions shared across the application.

This separation helps keep the codebase maintainable as new features and card games are added.

---

## Main Functional Areas

### Storefront

Users can browse products, filter listings and manage their shopping cart.

### Authentication

Authenticated users can access private features such as collection management and administration tools.

### Administration

Administrative pages provide tools for managing products, inventory and sales across different Trading Card Games.

### Collections

Registered users can manage and organize their personal card collections.

---

## Architecture

The application is organized around reusable modules instead of game-specific implementations whenever possible.

Shared functionality such as authentication, shopping cart, navigation and common UI components is reused across all supported Trading Card Games, while game-specific pages extend this shared foundation.

Communication with the backend is isolated inside the **services** layer, allowing components and pages to remain focused on presentation and user interaction.

---

## Future Improvements

Some planned improvements include:

* Progressive Web App support
* Performance optimizations
* Internationalization (i18n)

---

## Related Projects

Backend API:

https://github.com/emiibayona/geartown-api

---

## About

This project was built as a personal initiative to solve real-world needs for a local TCG store while experimenting with scalable frontend architecture, reusable components and modern Vue.js development practices.

<img width="1906" height="1240" alt="Screenshot 2026-07-24 at 6 48 59 PM" src="https://github.com/user-attachments/assets/4a325fe4-a09c-444b-9b17-ce636a8282bb" />
