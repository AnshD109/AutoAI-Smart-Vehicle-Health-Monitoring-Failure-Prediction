# 🚗 AutoAI - Smart Vehicle Health Monitoring & Failure Prediction

> Built with a strong foundation in AI and data science, this project applies real-time sensor analytics and machine learning to improve vehicle safety and reliability. Developed during advanced studies at UE Potsdam.

---

## 📊 Project Overview 

AutoAI is an AI-driven vehicle health monitoring system that uses real-time sensor data to predict potential component failures. With a combination of machine learning, MQTT protocol, and a web-based dashboard, the system helps ensure smarter, safer, and more proactive vehicle maintenance.

---

## 🔹 Key Features 

* ⏱️ Real-time sensor data streaming via MQTT
* 🤖 Predictive maintenance using XGBoost
* 📊 Exploratory Data Analysis (EDA) with insights
* 🔄 Live model inference in a Flask web app

---

## 🧠 Technologies Used

* Python 3.x
* Flask (web interface)
* XGBoost (ML model)
* Pandas, NumPy, Matplotlib, Seaborn (data analysis)
* MQTT (sensor data streaming)

---

## 🌐 Architecture

1. Sensor data is published using `sensor_publisher.py`.
2. Data is subscribed and processed by `sensor_subscriber.py`.
3. The trained XGBoost model (`xgb_model.pkl`) predicts health status.
4. Results are displayed on a Flask-based web dashboard.

---

## 📁 Files Overview

* `app.py` - Flask server for the web interface
* `model.ipynb` - Model training workflow
* `EDA.ipynb` - Data exploration and visualization
* `real_time_sensor_data.csv` - Sample dataset
* `sensor_publisher.py` - Simulates vehicle sensor readings
* `sensor_subscriber.py` - Consumes sensor data via MQTT
* `xgb_model.pkl` - Pretrained ML model

---

## 🔢 Setup Instructions

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/AnshD109/AutoAI-Smart-Vehicle-Health-Monitoring-Failure-Prediction.git
   cd AutoAI-Smart-Vehicle-Health-Monitoring-Failure-Prediction

2. **Set Up Python Virtual Environment**:

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows

3. **Install Python Dependencies**:

   ```bash
   pip install -r requirements.txt

4. **Simulate Sensor Data with MQTT Publisher & Subscriber**:

   ```bash
   python sensor_publisher.py
   python sensor_subscriber.py

5. **Launch the Flask Web Application**:

   ```bash
   python app.py

6. **Train or Retrain the Machine Learning Model(if required)**
   - model.ipynb

---

## 🌟 Future Enhancements

* Integrate with actual IoT sensor hardware
* Add mobile dashboard
* Deploy on cloud platforms for scalability
* Model tuning with real-world telemetry data

---

> "Combining AI, IoT, and real-time analytics to redefine automotive intelligence."
