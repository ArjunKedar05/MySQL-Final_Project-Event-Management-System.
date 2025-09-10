# MySQL-Final_Project-Event-Management-System.
"Event Management System is a database-driven project designed to streamline event planning, registration, scheduling, and resource management. It allows organizers to manage attendees, venues, payments, and reports efficiently, making event coordination simple and effective."

# 🎉 MySQL Final Project: Event Management System

An **Event Management System** designed as a final project using **MySQL**.  
This system provides a structured database solution to manage events, participants, registrations, payments, and feedback efficiently.

<img width="270" height="180" alt="image" src="https://github.com/user-attachments/assets/9686f9bf-e96a-432f-9631-e47611020fb3" />

---

## 📖 Table of Contents
- [About the Project](#-about-the-project)
- [Features](#-features)
- [Database Design](#-database-design)
- [ER Diagram](#-er-diagram)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Sample Queries](#-sample-queries)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🔎 About the Project
The **Event Management System** provides a well-structured relational database built in MySQL.  
It helps event organizers to:
- Create and manage events  
- Register participants  
- Track payments  
- Record attendance  
- Collect feedback  

This project demonstrates **SQL database design principles, normalization, and query writing skills**.

---

## ✨ Features
- 👥 Manage participants and organizers  
- 📅 Create and update events  
- 🎟️ Handle registrations and ticketing  
- 💳 Manage payments and track dues  
- 📊 Generate reports (attendance, revenue, feedback)  
- 📝 Collect event feedback  

---

## 🗄 Database Design
The project includes **5 core tables** with meaningful attributes:

1. **Users**  
   - `User_ID`, `Name`, `Email`, `Phone`, `Role`  

2. **Events**  
   - `Event_ID`, `Title`, `Date`, `Location`, `Organizer_ID`  

3. **Registrations**  
   - `Reg_ID`, `User_ID`, `Event_ID`, `Status`, `Payment_ID`  

4. **Payments**  
   - `Payment_ID`, `Amount`, `Method`, `Date`, `User_ID`  

5. **Feedback**  
   - `Feedback_ID`, `User_ID`, `Event_ID`, `Comments`, `Rating`  

---

## 🖼 ER Diagram
*(Add your ER diagram here if available, for example as `assets/er-diagram.png`)*  

```text
Users ----< Registrations >---- Events
   |                               |
   |                               |
 Payments                      Feedback
