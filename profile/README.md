# Ius Ecosystem 🎓⚖️

Welcome to the official GitHub organization for **Ius**, a specialized educational platform designed to help law students prepare for their exams and competitive certifications.

This organization hosts the complete source code for the Ius platform, which consists of a mobile application and a robust headless backend infrastructure.

## 🏗️ Architecture Overview

The Ius ecosystem is built using a modern decoupled architecture:
- **Frontend**: A high-performance cross-platform mobile app.
- **Backend (CMS)**: A WordPress-based headless system for content management.
- **Backend (Services)**: Custom PHP microservices and plugins for authentication and specialized logic.

---

## 📦 Repositories

### 📱 [ius-app](https://github.com/Jurixio/ius-app)
The flagship mobile application for Ius.
- **Utility**: Provides law students with a comprehensive learning interface including news feeds, interactive flashcards, study sessions, and progress tracking.
- **Tech Stack**: Built with **React Native (Expo/CLI)** and **Redux Toolkit**.
- **Key Features**: Offline mode, push notifications, and synchronization with the Ius central API.

### 🎨 [ius-theme](https://github.com/Jurixio/ius-theme)
The foundational WordPress theme for the headless CMS.
- **Utility**: A minimalist "API-only" theme. Since the platform uses WordPress as a headless CMS, this theme strips away traditional front-end weight to optimize performance and ensure the server primarily serves data via the REST API.
- **Tech Stack**: PHP, WordPress.

### 🔌 [ius-bridge](https://github.com/Jurixio/ius-bridge)
The bridge to the main Jurixio content ecosystem.
- **Utility**: A dedicated WordPress plugin installed on the **main Jurixio website**. It acts as a content provider for the Ius app, allowing the app to fetch articles and resources directly from the primary site.
- **Key Features**: Secure content exposure from the main site, custom REST API endpoints, and advanced visibility rules for premium legal content.

### ⚙️ [ius-rest-api](https://github.com/Jurixio/ius-rest-api)
The core backend services and authentication layer.
- **Utility**: Handles advanced backend functionalities that go beyond standard WordPress capabilities. It manages secure authentication flows and bridges different services.
- **Tech Stack**: PHP, Composer, Firebase JWT, Facebook SDK.
- **Key Features**: Social login management (OAuth2), JWT token generation/validation for secure app access, and custom restriction logic for user permissions.

---

## 🛠️ Main Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Mobile** | React Native, TypeScript, Redux Toolkit, React Navigation |
| **CMS** | WordPress (Headless) |
| **Backend** | PHP, Composer, Firebase JWT, MySQL |
| **Integration** | REST API, OAuth 2.0 |

---

## 🚀 Getting Started

To get the full environment running locally:

1.  **Backend**: Set up a WordPress environment and install the `ius-theme` and `ius-bridge` plugin.
2.  **API Services**: Configure `ius-rest-api` with the necessary environment variables for Firebase and OAuth providers.
3.  **Frontend**: Navigate to `ius-app`, run `npm install`, and start the development server with `npm start`.

---
*Note: This ecosystem is private property. Unauthorized copying or distribution of these repositories is strictly prohibited.*
