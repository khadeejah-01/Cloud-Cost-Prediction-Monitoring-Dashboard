#  Cloud-Based Cost Monitoring & Prediction Dashboard

##  Overview

This project is a **Cloud Cost Monitoring & Prediction Dashboard** that helps analyze cloud resource usage and predict future costs using Machine Learning.

It combines:

* **Java (Core Application Logic)**
* **Flask (ML Model API)**
* **Frontend Dashboard (HTML/CSS/JS)**
* **Machine Learning (Cost Prediction Model)**
* Data Preprocessing for the used dataset

The system simulates a real-world cloud billing environment by monitoring usage data and providing **cost predictions and insights**.

---

##  Features

*  Monitor cloud resource usage (CPU, Memory, Network)
*  Predict future cloud costs using ML model
*  Interactive dashboard visualization
*  Integration between Java and Python (Flask API)
*  Organized dataset handling (raw & processed)
*  (Optional) Alert system for high predicted costs

---

##  System Architecture

```
Frontend (HTML/JS Dashboard)
        ↓
Java Application (Processing + API Calls)
        ↓
Flask API (ML Model)
        ↓
Predicted Cost
        ↓
Back to Dashboard (Visualization)
```

---

##  Tech Stack

| Layer      | Technology Used       |
| ---------- | --------------------- |
| Backend    | Java (Core)           |
| ML Backend | Python Flask          |
| ML Model   | Scikit-learn          |
| Frontend   | HTML, CSS, JavaScript |
| Data       | CSV / JSON            |

---

##  Project Structure

```
Cloud-Cost-Monitoring-Dashboard/
│
├── java-app/          # Java application (main logic + API calls)
├── ml-service/        # Flask ML backend
├── frontend/          # Dashboard UI
├── data/              # Datasets (raw + processed)
├── docs/              # Documentation & screenshots
├── springboot-version/ # Future upgrade (planned)
└── README.md
```

---

##  How to Run the Project

###  Step 1: Run ML Service (Flask)

```bash
cd ml-service
pip install -r requirements.txt
python app.py
```

Flask server will run at:

```
http://127.0.0.1:5000
```

---

###  Step 2: Run Java Application

* Open `java-app` in your IDE (VS Code / IntelliJ)
* Run `MainApp.java`

---

###  Step 3: Open Dashboard

* Open `frontend/index.html` in browser
* View charts and predictions

---

##  API Example

### POST `/predict`

**Request:**

```json
{
  "cpu": 2,
  "memory": 4,
  "network": 100
}
```

**Response:**

```json
{
  "predicted_cost": 1.82
}
```

---


##  Future Scope

*  Convert Java app into **Spring Boot REST API**
*  Integrate real cloud platforms (AWS, Azure, GCP)
*  Add real-time alert system
*  Live data streaming instead of static CSV
*  Improve UI with modern frameworks (React)

---

##  Learning Outcomes

What I Learned from This Project:

Working on this project actually helped me understand how real systems are built, not just small programs we usually make in class.

First, I learned how different technologies can work together. Before this, I only used Java on its own, but here I connected Java with a Python Flask API for machine learning. It made me realize how systems in real life are not built in one language — they communicate through **APIs**.

I also got hands-on experience with **handling data**. Reading CSV files, processing them, grouping data (daily, weekly costs), and converting everything into JSON for the dashboard really improved my understanding of **data flow** inside an application.

Another important thing I learned was how machine learning can be **integrated** into software. Instead of just training a model, I actually used it in a working system where Java sends data and receives predictions. That made the ML part feel practical rather than theoretical.

I also understood the importance of **structuring** a project properly. At the start, everything was in one place, but later I realized why separating logic (like prediction service, data processing, etc.) makes the system cleaner and easier to manage. This is something that is strongly emphasized in software development practices as well .

Working on the dashboard part helped me see how backend data is finally presented to users. Generating JSON and visualizing it with charts made the project feel complete and closer to a real product.

Another thing I learned was the importance of **documentation** and organization. Writing README, creating a proper folder structure, and adding docs made me realize that code alone is not enough — a project should be understandable to others too. Good documentation actually helps in collaboration and makes systems easier to use and maintain .

Overall, this project improved my problem-solving skills a lot. I faced issues with API calls, data flow, and integration, but solving them step by step gave me confidence that I can handle more complex systems in the future.
where should i add this.. or should i even do it, or make it more compact
---

##  License

This project is for educational purposes.

---

##  Author

**Khadeejah Yasin**
Computer Science Student
