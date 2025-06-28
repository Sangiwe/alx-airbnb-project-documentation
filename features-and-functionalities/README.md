# Airbnb Clone - Backend Features Documentation

This document outlines the core features and functionalities of the Airbnb Clone backend system, as visualized in the flowchart (`features-and-functionalities.png`).

## Domains Overview
### 1. User Management
- **Features**:
  - SignUp/SignIn (Guests & Hosts)
  - Profile Management
- **Functionalities**:
  - JWT Authentication
  - OAuth (Google/Facebook)
  - Email/Password Auth
  - Rate Limiting
  - Update Profile Picture
  - Update Contact Info
  - Role-based Access Control

### 2. Property Listings Management
- **Features**:
  - Create/Edit/Delete Listings
  - Search & Filtering
- **Functionalities**:
  - Image Upload (AWS S3)
  - Amenity Tagging
  - Geo-Based Search
  - Add By: title, description, location etc
  - Update/remove Property

### 3. Booking Management
- **Features**:
  - Booking Creation
  - Cancellation
  - Status Tracking
- **Functionalities**:
  - Date Conflict Validation
  - Cancellation Policy Engine
  - Real-Time Status Updates

### 4. Payment Integration
- **Features**:
  - Guest Payments
  - Host Payouts
- **Functionalities**:
  - Stripe/PayPal Integration
  - Multi-Currency Support
  - Automated Service Fee Deduction

### 5. Reviews & Notifications
- **Features**:
  - Booking-Linked Reviews
  - Email/In-App Alerts
- **Functionalities**:
  - Review Moderation
  - Notification Queues

## Flowchart Key
- **Shapes**:
  - 🟦 Rounded Rectangle: Core Domains
  - 🟩 Parallelogram : Features
  - 🟧 Oval: Technical Functionalities

## How to Use
1. Refer to `Features and Functionalities Flowchart Task 0.drawio.png` for visual relationships.
