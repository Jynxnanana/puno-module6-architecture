# System Architectural Design

## 1. System Overview
The Food Ordering System is a web-based application that allows customers to view a restaurant's menu, place orders online, and track order status in real time, while staff manage and update those orders through a backend interface.

## 2. Selected Architectural Pattern
The proposed system will use a three-tier client-server architecture.
The system will be divided into:
1. Presentation layer
2. Application layer
3. Data layer

This architecture separates the user interface, business logic, and data management responsibilities.

## 3. Architectural Components

### Presentation Layer
The presentation layer will use Vue.js. It will display the menu, collect order details from the customer, and send order requests to the backend.

### Application Layer
The application layer will use Node.js and Express. It will receive order requests, validate order data, apply business rules (e.g. order status transitions), and communicate with the database.

### Data Layer
The data layer will use MongoDB Atlas Free. It will store, retrieve, update, and delete menu items and order records.

## 4. Component Responsibilities

| Component | Technology | Responsibility |
|---|---|---|
| User interface | Vue.js | Displays menu items and collects order input |
| Application server | Node.js and Express | Processes order requests and applies business rules |
| Database | MongoDB Atlas Free | Stores and manages menu and order records |
| Repository | GitHub | Stores documentation and tracks changes |
