# Subscription Tracker API

## Overview
Subscription Tracker API is a backend service designed to help users track their subscriptions efficiently. It provides endpoints to manage subscriptions, send email reminders, and integrate with cloud storage and security services.

## Tech Stack
- **Node.js** - Runtime environment for executing JavaScript on the server.
- **Express.js** - Lightweight framework for handling API routes.
- **MongoDB** - NoSQL database to store subscription details.
- **Mongoose** - ODM (Object Data Modeling) library for MongoDB.
- **Upstash** - Managed Redis database for caching and session management.
- **Arcjet** - Serverless execution and API security layer.
- **Nodemailer** - Email sending library for notifications and reminders.

## Features
- Add, update, delete, and retrieve subscriptions.
- Automated email reminders for upcoming renewals.
- Caching mechanism using Upstash for improved performance.
- Secure API endpoints using Arcjet.
- MongoDB database integration with Mongoose schema models.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/subscription-tracker-api.git
   cd subscription-tracker-api
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Set up environment variables:
   Create a `.env` file and add the following:
   ```env
   MONGO_URI=your_mongodb_connection_string
   UPSTASH_REDIS_URL=your_upstash_redis_url
   ARCJET_API_KEY=your_arcjet_api_key
   EMAIL_SERVICE=your_email_service_provider
   EMAIL_USER=your_email_username
   EMAIL_PASS=your_email_password
   ```
4. Start the server:
   ```sh
   npm start
   ```

## API Endpoints

### **1. Subscription Management**
- `POST /api/subscriptions` - Create a new subscription.
- `GET /api/subscriptions` - Get all subscriptions.
- `GET /api/subscriptions/:id` - Get a single subscription by ID.
- `PUT /api/subscriptions/:id` - Update a subscription.
- `DELETE /api/subscriptions/:id` - Delete a subscription.

### **2. Notifications**
- `POST /api/notifications/send` - Send email reminders for upcoming renewals.

## Contribution
Feel free to fork this repository and contribute by submitting pull requests.

## License
This project is licensed under the MIT License.

