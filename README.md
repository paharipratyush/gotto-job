# 🚀 Gotto Job - DevOps Sprint Simulation

![Status](https://img.shields.io/badge/Status-Completed-success)
![Deployment](https://img.shields.io/badge/Deployed%20to-AWS%20EC2-orange)
![Methodology](https://img.shields.io/badge/Methodology-Scrum%20%2F%20Agile-blue)

This repository contains the source code for the **"Gotto Job"** application, modified and deployed as part of **Assignment 4** of the [DevOps Micro Internship (Cohort 2)](https://youtu.be/PTSkAR7iMpQ?si=SnWGCORuXp8IVrDm).

The primary goal of this project was not just to write code, but to execute a **full Scrum Lifecycle** - from Backlog Refinement in Jira to Production Deployment on AWS.

---

## 📋 Project Overview

**"Gotto Job"** is a job portal listing website template. In this assignment, I acted as the **Product Owner, Scrum Master, and DevOps Engineer** to deliver specific UI improvements within a 1-week Sprint.

### 🎯 Sprint 1 Goal
> *"Ship 2–3 visible UI improvements to Gotto Job and verify them live in production."*

---

## 🛠️ Tech Stack & Tools

* **Frontend:** HTML5, CSS3, Bootstrap 5
* **Web Server:** Nginx (Reverse Proxy / Static Serving)
* **Infrastructure:** AWS EC2 (Ubuntu 24.04 LTS)
* **Project Management:** Jira Software (Team-managed Scrum)
* **Version Control:** Git & GitHub

---

## 🔄 The DevOps Lifecycle (What I Did)

### 1. Planning (Jira)
* Created a **Team-managed Scrum Project**.
* Refined the Product Backlog with **Epics** and **User Stories**.
* Defined clear **Acceptance Criteria (AC)** for every story.
* Estimated effort using **Fibonacci Story Points** (1, 2, 3).

### 2. Development (Local)
* **Feature:** Updated the Hero Section tagline for better discoverability.
    * *Old:* "Search your dream job"
    * *New:* "Find your next role, fast."
* **Branching Strategy:** Maintained a stable `main` branch and developed features on dedicated branches (e.g., `feature/hero-tagline`).

### 3. Deployment (AWS)
* Provisioned an **AWS EC2 Instance** (t2.micro).
* Installed and configured **Nginx** web server.
* Deployed artifacts using a manual **SCP pipeline**:
  
    ```bash
    scp -i "key.pem" -r . ubuntu@<EC2-IP>:/var/www/html
    ```
* Verified the live deployment against Acceptance Criteria.

---

## 📸 Screenshots

| Before (Original) | After (Sprint 1 Delivery) |
| :---: | :---: |
| *Tagline: "Search your dream job"* | *Tagline: "Find your next role, fast."* |

---

## 🚀 How to Run Locally

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/paharipratyush/gotto-job.git](https://github.com/paharipratyush/gotto-job.git)
    cd gotto-job
    ```

2. **Open in Browser:**
    * Simply open the `index.html` file in Chrome/Edge, or use a live server

---

## 🙏 Acknowledgements

* **Mentor:** [Pravin Mishra](https://www.linkedin.com/in/pravin-mishra-aws-trainer/) for the expert guidance on Real-world DevOps.
* **Original Template:** [Tooplate](https://www.tooplate.com/) (2134 Gotto Job).
* **Community:** [DMI Cohort 2 Group 4](https://discord.pravinmishra.com/).

---

*Part of the DevOps Micro Internship (DMI) by [Pravin Mishra](https://www.linkedin.com/in/pravin-mishra-aws-trainer/).*
