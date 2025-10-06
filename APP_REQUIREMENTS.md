# Full App Requirements

## 1. Introduction

* **Application Name:** Ruhroh App
* **Elevator Pitch:** A platform to connect a pet sitting business with a network of sitters, streamlining the process of onboarding sitters, managing pet profiles, and facilitating communication for pet sitting requests.

## 2. User Personas

* **Business Owner:** Manages the pet sitting business, oversees all requests, and manages the network of sitters.
* **Sitter:** A registered user who can accept or decline pet sitting requests from the business owner.
* **Pet Owner (Implied):** The customer who initiates the pet sitting request. While they may not directly interact with the app, their information and their pet's information is managed within the system.

## 3. User Stories

### 3.1. Sitter Features

* As a sitter, I want to be able to create an account and log in.
* As a sitter, I want to have a dashboard to view incoming pet sitting requests from the business owner.
* As a sitter, I want to be able to accept or decline these requests.
* As a sitter, I want to be able to view all of my accepted requests.
* As a sitter, I want to be able to manage my profile, including my rates and any available discounts.

### 3.2. Business Owner Features

* As a business owner, I want to have a dashboard to view all pet sitting requests from customers.
* As a business owner, I want to see the assignment status of each request (e.g., pending, assigned, completed).
* As a business owner, I want to be able to view all sitters in my network, including their rates and discounts.
* As a business owner, I want to be able to assign a pet sitting request to a specific sitter in the network.
* As a business owner, I want to be able to communicate with sitters regarding requests.

### 3.3. Pet Profile Management

* As a user (business owner or sitter), I want to be able to create and manage a profile for each pet.
* As a user, I want the pet profile to include information such as name, breed, age, and any special instructions or needs.

## 4. Non-Functional Requirements

* **Security:** User data (especially personal and financial information) must be stored securely.
* **Usability:** The application should be intuitive and easy to use for both business owners and sitters.
* **Reliability:** The platform should be reliable and available when needed.

## 5. Technology Stack (Proposed)

* **Frontend:** Web Application (e.g., React, Vue, or Angular)
* **Backend:** Node.js with Express.js
* **Database:** PostgreSQL or MongoDB
