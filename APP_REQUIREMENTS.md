# Full App Requirements

## 1. Introduction

* **Application Name:** Ruhroh
* **Elevator Pitch:** A social media application where users can post "ruhrohs" (short, ephemeral posts about their mistakes or funny mishaps) that disappear after 24 hours. Friends can react to these posts, and the user with the most reactions at the end of the week gets a "crown."

## 2. User Personas

* **The Jester:** A user who enjoys sharing funny stories and making their friends laugh. They are motivated by getting reactions and winning the weekly crown.
* **The Empathizer:** A user who enjoys seeing the human side of their friends and finds comfort in knowing that everyone makes mistakes. They are motivated by connecting with their friends on a more personal level.
* **The Spectator:** A user who primarily consumes content and enjoys seeing what their friends are up to. They are motivated by entertainment and staying in the loop.

## 3. User Stories

### 3.1. Core Functionality

* As a user, I want to be able to create an account and log in.
* As a user, I want to be able to create a profile with a username, profile picture, and a short bio.
* As a user, I want to be able to find and add friends.
* As a user, I want to be able to see a feed of my friends' "ruhrohs."
* As a user, I want to be able to post a "ruhroh" with text and an optional image or video.
* As a user, I want my "ruhrohs" to disappear after 24 hours.
* As a user, I want to be able to react to my friends' "ruhrohs" with a set of predefined emojis.
* As a user, I want to be able to see who has reacted to my "ruhrohs."

### 3.2. Gamification

* As a user, I want to be able to see a weekly leaderboard of my friends based on the number of reactions they've received.
* As a user, I want to receive a "crown" if I have the most reactions at the end of the week.
* As a user, I want to be able to see my past crowns on my profile.

### 3.3. Notifications

* As a user, I want to receive a notification when someone adds me as a friend.
* As a user, I want to receive a notification when a friend posts a "ruhroh."
* As a user, I want to receive a notification when someone reacts to my "ruhroh."
* As a user, I want to receive a notification if I win the weekly crown.

## 4. Non-Functional Requirements

* **Scalability:** The application should be able to handle a large number of users and posts without performance degradation.
* **Security:** User data should be stored securely, and all communication between the client and server should be encrypted.
* **Usability:** The application should be intuitive and easy to use.
* **Availability:** The application should be available 24/7 with minimal downtime.

## 5. Technology Stack (Proposed)

* **Frontend:** React Native (for cross-platform mobile app)
* **Backend:** Node.js with Express.js
* **Database:** PostgreSQL
* **Real-time Communication:** Socket.io (for notifications and live updates)
* **Cloud Provider:** AWS or Google Cloud
