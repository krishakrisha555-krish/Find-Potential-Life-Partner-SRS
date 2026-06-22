# Find Potential Life Partner Online Platform - System Requirement Specification (SRS)

**Author:** P. Krishanthini  
**Organization:** Remu (Pvt)  
**Date:** 29-04-2025  
**Target Client:** Matchmaking Company  

---

## 1. Introduction
This repository contains the comprehensive System Requirement Specification (SRS) for the **Find Potential Life Partner Online Platform**. This document delivers a detailed breakdown of both the functional and non-functional requirements proposed by the client. 

The primary purpose of this project is to create an accessible online platform that helps the local community discover potential life partners. Users can securely register, build personal profiles, browse other members, and initiate contact via simple messaging.

---

## 2. Project Scope

### 📦 In Scope
*   **Profile Creation:** Local community members can create an individual account populated with basic background details (Age, Gender, Religion, Occupation, a brief bio, and a profile photo).
*   **Profile Lifecycle Management:** Users maintain full control to edit or delete their profile details at any time.
*   **Criteria-Based Search:** Members can search and filter through other public profiles using targeted fields (Age, Gender, Religion, Occupation).
*   **Profile Visibility:** Users can open and view the profile details of other members.
*   **Basic Communication:** If a user finds someone they are interested in, they can initiate a connection by sending a simple text message.

### 🚫 Out of Scope (Current Version)
*   **Advanced Media:** Users cannot make voice calls or video calls through the platform.
*   **Automated Matchmaking:** There are no automated matching algorithms integrated into this initial release phase.
*   **Localization:** Multi-language options are currently unavailable.

---

## 3. Functional Requirements

### 👥 User Stories

#### 1. Authentication
*   **As a user,** I want to log in to my account securely using a strong password so that my private data is protected.
*   **As an admin,** I want to log in to my admin panel securely using a strong password so that I can maintain system integrity.

#### 2. Create Profile
*   **As a user,** I should be able to create my own account using my basic information (Age, Gender, Religion, Occupation, short bio, and a photo).

#### 3. Search Option
*   **As a user,** I can search for other profiles based on selective criteria (Age, Gender, Religion, Occupation).

#### 4. Send Message
*   **As a user,** if I find someone I am interested in, I can send a simple text message to them.

#### 5. Manage Profile
*   **As an admin,** I can view members' profiles and manage/moderate their profiles properly to ensure community standards.

### 📊 Use Case Diagram
Below is the system boundary mapping out the relationship between the primary Actors (**User** and **Admin**) and the core system Use Cases:

![Use Case Diagram](https://github.com/krishakrisha555-krish/Find-Potential-Life-Partner-SRS/blob/main/use_case_diagram.jpg?raw=true)

---

## 4. Non-Functional Requirements

*   **Usability:** The platform must feature a simple, intuitive, and user-friendly interface optimized for individuals who may not be highly tech-savvy.
*   **Reliability:** The system must remain stable and operate consistently without frequent crashes or unhandled execution errors. All user-entered data must save securely without threat of data loss.
*   **Performance:** 
    *   The platform interface must load fully in **under 2 seconds**.
    *   Authentication actions and data submission operations must execute reasonably fast.
*   **Security:** High priority is placed on ensuring that users' personal and sensitive demographic information is protected in a secure manner.
*   **Maintainability:** The platform architecture must be designed in a modular way to facilitate future feature expansions, algorithmic updates, and quick bug fixes.

---

## 5. Technological Specification

*   **Supported Platforms:**
    *   **Mobile:** Native/Hybrid deployment for Android and iOS (minimum OS versions to be determined by target demographic analysis).
    *   **Desktop:** Full cross-browser support for Google Chrome and Mozilla Firefox.
*   **Frontend Stack:** HTML, JavaScript, Java
*   **Backend Framework:** Spring Boot, Node.js (JavaScript)
*   **Database Engine:** MongoDB (NoSQL data storage for flexible user profiles)

---

## 6. System Limitations
1.  The initial platform release completely lacks an automated matching algorithm.
2.  Communication capabilities are strictly restricted to basic text messaging; no voice or video calls are supported.
3.  The system is built to support single-language deployment only.
4.  **Concurrency Constraints:** The platform is configured to handle a maximum threshold of **200 concurrent users** right now.
5.  There is no push or in-app notification functionality integrated into this build version.
