
# 🧑‍🎓 Student Progress Management System

A full-stack web application to manage student data and track competitive programming progress on **Codeforces**, built using the **MERN stack** with Python automation scripts.



📌 Project Overview

This system is designed for EdTech platforms to monitor and manage students' performance in competitive programming. It includes:

- A dashboard to manage student information
- Codeforces rating and submission tracking
- Automated data syncing with cron jobs
- Inactivity detection and email reminders

Built as part of the hiring assignment for **TLE Eliminators**.

---

## 🛠️ Tech Stack

**Frontend:** React.js, TailwindCSS  
**Backend:** Node.js, Express.js  
**Database:** MongoDB  
**Automation & Emailing:** Python (Cron jobs, SMTP/email logic)  
**Charts & Visuals:** Chart.js / Recharts / React Calendar Heatmap

---

## ⚙️ Features

### 🎓 Student Table View
- View all students with:
  - Name, Email, Phone Number
  - Codeforces Handle, Current Rating, Max Rating
- Add, Edit, Delete students
- CSV export
- “View Details” button for profile access

### 📊 Student Profile View
- **Contest History**
  - Filter by last 30/90/365 days
  - Rating graph and contest data
- **Problem Solving Stats**
  - Most difficult problem solved
  - Average rating, total problems, problems per day
  - Bar chart of rating buckets
  - Submission heatmap

### 🔄 Codeforces Data Sync
- Daily cron job (default: 2 AM)
- Stores data locally to avoid real-time API calls
- Manual sync on handle update
- Shows "Last Updated" per student

### 🚨 Inactivity Detection
- After each sync, students with 0 submissions in the last 7 days are:
  - Sent a reminder email
  - Tracked with a counter of total emails sent
- Option to disable auto-email per student



