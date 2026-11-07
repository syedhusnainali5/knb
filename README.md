# Karachi Naseeb Biryani (KNB)

<p align="center">
  <strong>Digital Food Ordering & Restaurant Management Platform</strong><br/>
  A complete mobile ordering and restaurant operations solution.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React_Native-Mobile_App-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React Native"/>
  <img src="https://img.shields.io/badge/Node.js-Backend-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/Express.js-API-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express"/>
  <img src="https://img.shields.io/badge/MongoDB-Database-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
</p>

---

## ⚠️ Repository Notice

This repository is a React Native boilerplate/showcase repository and does **not** contain the actual production source code of the Karachi Naseeb Biryani application.

The actual production application, backend implementation, database, administrative dashboard, credentials, and deployment infrastructure are maintained separately.

---

## 1. About Karachi Naseeb Biryani

**Karachi Naseeb Biryani (KNB)** is a digital restaurant ordering platform designed to modernize the food ordering experience and streamline restaurant operations.

The platform connects customers with restaurant branches through a dedicated mobile application while providing restaurant administrators with a centralized system for managing orders, branches, customers, and operational activities.

The solution combines a customer-facing Android application, backend API services, database infrastructure, and a web-based administrative management system.

### Core Objectives

- Simplify online food ordering.
- Provide a convenient mobile ordering experience.
- Support multiple restaurant branches.
- Improve order processing and management.
- Centralize restaurant administration.
- Reduce manual operational work.
- Provide real-time order-related communication.

---

## 2. Mobile Application Features

The customer application is developed using **React Native**, providing a native mobile experience.

### 🍛 Food & Menu Browsing
- Browse available food items.
- View product information.
- Explore restaurant offerings.
- Access menu information.

### 🛒 Cart & Ordering
- Add food items to the cart.
- Manage order quantities.
- Review selected products.
- Submit food orders.
- Track order-related information.

### 📍 Branch & Location Management
- Discover available restaurant branches.
- Identify eligible branches based on customer location.
- Configurable branch-distance restrictions.
- Default branch eligibility radius of 3 km, configurable between 1–5 km.

### 📦 Order Management
- Place orders through the mobile application.
- Generate unique order references.
- Follow order processing.
- Access order information.
- Maintain order history.

### 🔔 Notifications & Communication
- Receive order-related notifications.
- Stay informed about order updates.
- Support real-time communication between application services and customers.

### 👤 Customer Experience
- Customer account management.
- Profile information.
- Order history.
- Convenient mobile-first interface.

---

## 3. Administrative Management System

KNB includes a dedicated web-based administrative system designed to manage restaurant operations.

The administration system communicates with backend services and provides authorized staff with centralized access to operational functionality.

### Administrative Features

**1. Order Management**
- View incoming customer orders.
- Access order details.
- Manage order processing.
- Update order statuses.
- Monitor order activity.

**2. Automatic Order Printing**

One of the important operational integrations is automatic order-slip printing.

The administrative environment supports browser-based automatic printing when a new order arrives, helping restaurant staff process incoming orders without manually checking and printing each order.

**3. Branch Management**
- Manage restaurant branches.
- Maintain branch-related information.
- Configure branch availability and operational settings.
- Control branch-distance eligibility.

**4. Customer Management**
- Access customer records.
- Review customer-related information.
- Maintain customer order records.

**5. Menu & Product Management**
- Manage food items.
- Maintain menu information.
- Update product details and availability.

**6. Operational Management**
- Monitor restaurant activity.
- Manage order workflows.
- Access relevant operational information through the dashboard.

---

## 4. Technical Architecture

The production KNB platform uses a client-server architecture.

| Component | Technology | Purpose |
|---|---|---|
| Customer Mobile App | React Native CLI | Android application |
| Backend | Node.js | Server-side processing |
| API Framework | Express.js | REST API services |
| Database | MongoDB | Persistent data storage |
| Database Configuration | MongoDB Replica Set | Database deployment |
| Admin Dashboard | Web-based | Restaurant administration |
| Real-time Communication | Socket.IO | Order-related communication |
| Process Management | PM2 | Backend process management |
| Server Infrastructure | Ubuntu VPS | Production hosting |

### System Architecture

```text
              CUSTOMERS
                  |
                  v
         REACT NATIVE APP
                  |
                  v
             REST APIs
                  |
                  v
          NODE.JS + EXPRESS
                  |
          +-------+-------+
          |               |
          v               v
       MONGODB         SOCKET.IO
          |               |
          |               v
          |        REAL-TIME EVENTS
          |               |
          +-------+-------+
                  |
                  v
          ADMIN DASHBOARD
                  |
          +-------+-------+
          |               |
          v               v
     ORDER CONTROL    AUTO PRINTING
          |
          v
     RESTAURANT STAFF
```

This is a conceptual representation of the production platform, not a deployment diagram of the boilerplate repository.

---

## 5. Order Processing Workflow

The platform follows a structured order lifecycle.

1. Customer opens the KNB mobile application.
2. Customer browses the menu and selects food items.
3. Customer adds items to the cart.
4. Customer selects the appropriate ordering and delivery information.
5. The application submits the order to the backend.
6. The backend validates and stores the order.
7. A unique order reference is generated using the `NB-10000+` numbering convention.
8. The administrative system receives the incoming order.
9. The browser-based administrative environment can automatically print the order slip.
10. Restaurant staff process the order and update its status.
11. Customers receive relevant order updates.

---

## 6. Backend & Infrastructure

The production backend is deployed on Ubuntu-based VPS infrastructure.

### Backend Responsibilities

- Authentication and authorization.
- Customer management.
- Order creation and processing.
- Menu and product operations.
- Branch management.
- Order status management.
- Database operations.
- Real-time event communication.
- Administrative API services.

### Production Deployment

The production environment uses:

- Ubuntu 24.04 LTS.
- Node.js and Express.js.
- MongoDB Replica Set (`rs0`).
- PM2 process management.
- Separate backend services for application and administration.
- Socket.IO communication.
- HTTPS-enabled domain configuration.

The production infrastructure is not included in this repository.

---

## 7. Repository Scope

This repository is intended for project presentation and technical reference.

| Included | Not Included |
|---|---|
| React Native boilerplate | Actual production mobile app |
| Starter project structure | Production backend source |
| Project documentation | Production database |
| Development configuration | Admin dashboard source |
| Technical overview | Production credentials |
| Architecture documentation | Server infrastructure |

The production system is maintained separately.

---

## 8. Getting Started

### Prerequisites

- Node.js
- React Native development environment
- Android Studio
- Android SDK
- JDK
- Git

### Clone Repository

```bash
git clone <REPOSITORY_URL>
cd <PROJECT_DIRECTORY>
```

### Install Dependencies

```bash
npm install
```

### Android Development

```bash
npx react-native run-android
```

**Note:** These instructions apply to the included React Native boilerplate and do not reproduce the production KNB application.

---

## 9. Production Application

The KNB mobile application is the customer-facing component of the production restaurant management ecosystem.

**Application:** Karachi Naseeb Biryani (KNB)  
**Platform:** Android  
**Framework:** React Native CLI  
**Backend:** Node.js / Express.js  
**Database:** MongoDB

Google Play Store: https://play.google.com/store/apps/details?id=com.karachinaseebbiryani

---

<p align="center">
  <strong>Karachi Naseeb Biryani</strong><br/>
  Bringing restaurant ordering and management into one connected digital platform.
</p>
