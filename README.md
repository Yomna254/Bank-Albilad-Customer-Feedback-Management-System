# Bank Albilad – Customer Feedback Management System

A real-world customer feedback management system developed for Bank Albilad to collect customer feedback across branches, monitor customer satisfaction, and help branch management make data-driven decisions.

The system consists of two integrated applications: a Flutter-based customer application and a Flutter Web admin dashboard.

## Project Overview

The system provides a streamlined way for customers to share their experience while giving administrators centralized tools to monitor feedback, analyze satisfaction levels, and manage branch operations.

### 1. Customer Feedback Application

A tablet-based application deployed inside bank branches, allowing customers to submit feedback directly without creating an account or logging in.

**Key Features**
- Instant feedback submission without user registration.
- Customer satisfaction ratings: Satisfied, Neutral, and Unsatisfied.
- Text-based comments.
- Voice feedback recording.
- Local storage of pending feedback using SharedPreferences when the internet connection is unavailable.
- Automatic synchronization and upload when the connection is restored.
- Branch-specific device configuration.

### 2. Admin Dashboard

A web-based dashboard that enables administrators to monitor customer satisfaction and manage feedback across bank branches.

**Analytics & Reporting**
- Total number of submitted feedback entries.
- Distribution of satisfied, neutral, and unsatisfied ratings.
- Average customer satisfaction.
- Filtering by branch and time period.
- Exporting dashboard statistics to Excel for management reporting.

**Feedback Management**
- Dedicated feedback listing page.
- Categorization of feedback into satisfied, neutral, and unsatisfied.
- Access to individual feedback details.

**Admin Management**
- View existing administrators.
- Add new administrators.
- Remove existing administrators.

**Branch Management**
- View all registered branches.
- Display branch names and addresses.
- Monitor branch status (Active / Inactive).

**Role-Based Access Control**
- **Super Admin:** Has access to data across all branches and administrative management features.
- **Branch Admin:** Can access feedback and information belonging to their assigned branch only.

### 3. Automated Notifications

- Automatic email notifications are triggered when an unsatisfied customer rating is submitted.
- Firebase Cloud Functions handle the automated notification workflow.

## System Architecture

The solution consists of two main applications connected through Firebase services:

| Component | Technology |
|---|---|
| Customer Application | Flutter |
| Admin Dashboard | Flutter Web |
| Backend Services | Firebase |
| Database | Cloud Firestore |
| File & Voice Storage | Firebase Storage |
| Serverless Logic | Firebase Cloud Functions |
| Email Notifications | Automated Email Integration |

## Tech Stack

- Flutter & Dart
- Flutter Web
- Firebase Core
- Cloud Firestore
- Firebase Storage
- Firebase Cloud Functions
- SharedPreferences (Local Data Persistence)
- Git & GitHub

## My Role & Contributions

**Sole Developer – End-to-End Development**

I was responsible for developing the complete solution independently, including:

- Analyzing business requirements and translating them into application workflows.
- Designing and developing the customer-facing tablet application.
- Building the administrative web dashboard.
- Designing and implementing database structures and Firebase integrations.
- Implementing role-based access and branch-level data visibility.
- Implementing offline feedback handling using SharedPreferences and automatic synchronization.
- Implementing voice feedback recording and storage.
- Building analytics, filtering, and Excel export functionality.
- Developing automated email notification workflows.
- Implementing administrative and branch management features.

## Project Highlights

- Built a complete feedback management ecosystem with customer and administrative applications.
- Designed a simple, account-free customer experience suitable for in-branch tablets.
- Implemented offline-first feedback handling to reduce data loss caused by unstable internet connections.
- Enabled branch-level access control for administrative users.
- Automated notifications to help branch administrators respond to negative customer experiences.

---

*This is a portfolio case study of a private, live client project. Source code and confidential operational data are not publicly available.*
