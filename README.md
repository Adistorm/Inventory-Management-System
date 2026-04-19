# Smart Inventory Management System

A professional full-stack inventory dashboard with a React frontend and Spring Boot backend.

## Features

- Add, update, and delete products
- Low inventory alerts based on product thresholds
- Supplier tracking with contact details and reliability status
- Sales history with automatic stock reduction
- Dashboard metrics for stock value, revenue, units, suppliers, and alerts
- Offline demo data in the frontend when the backend is not running

## Project Structure

```text
backend/
  src/main/java/com/smartinventory/
    controller/
    dto/
    model/
    service/
frontend/
  src/
    main.jsx
    styles.css
```

## Run The Backend

Java 17 is already suitable for this project. Maven is required to run the Spring Boot app.

```bash
cd backend
mvn spring-boot:run
```

The API runs on:

```text
http://localhost:8080/api
```

## Run The Frontend

PowerShell on this machine blocks the `npm.ps1` shim, so use `npm.cmd`.

```bash
cd frontend
npm.cmd install
npm.cmd run dev
```

The React app runs on:

```text
http://localhost:5173
```

## API Endpoints

- `GET /api/summary`
- `GET /api/products`
- `POST /api/products`
- `PUT /api/products/{id}`
- `DELETE /api/products/{id}`
- `GET /api/alerts/low-stock`
- `GET /api/suppliers`
- `POST /api/suppliers`
- `GET /api/sales`
- `POST /api/sales`
