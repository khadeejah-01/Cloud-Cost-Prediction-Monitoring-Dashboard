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

I learned how to integrate Java with a machine learning model using Flask API, handle and process real datasets, and structure a project in a modular way. I also understood how backend data flows to the frontend for visualization and why proper documentation and clean architecture are important in real-world software development.
---

##  License

This project is for educational purposes.

---

##  Author

**Khadeejah Yasin**
Computer Science Student
