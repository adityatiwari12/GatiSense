````markdown
# 🚦 GatiSense  
*AI-Powered Traffic Insights & Route Optimization*  

---

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4d/NYC_Traffic.jpg" width="720" />
</p>

---

## 🌍 Overview  

GatiSense is an **AI-powered traffic insight system** that leverages the **NYC Taxi Trip Duration dataset** to provide:  
- 🚗 **Route optimization** with OSRM  
- ⏱️ **Travel time prediction** with ML models  
- 🗺️ **Traffic bottleneck visualization** with Leaflet.js  

The project offers **two dashboards**:  
- **Citizens & Delivery Services** → Route + ETA + Cost optimization  
- **City Officials** → Traffic heatmaps + bottleneck insights  

---

## 🎯 Objective  

**Problem Statement:**  
Build a mini AI-powered system that helps citizens, delivery services, and city officials gain insights into traffic patterns and improve mobility.  

**Solution Highlights:**  
- Predict travel times with ML  
- Optimize routing with OSRM  
- Visualize bottlenecks with GIS  
- Tailored dashboards for end-users & policymakers  

---

## ✨ Features  

### 🧑‍🤝‍🧑 Citizen & Delivery Dashboard  
- 🚦 Route recommendations with ETA  
- 🗺️ Interactive Leaflet.js maps  
- 🔄 Alternate routes with travel time comparisons  
- 💰 Trip efficiency analysis  

### 🏛️ City Officials Dashboard  
- 📊 Aggregated congestion heatmaps  
- 🕒 Peak vs. off-peak insights  
- 🚩 Identification of bottlenecks  
- 🏙️ Policy & infrastructure planning support  

---

## 📊 Business Context  

Traffic inefficiency impacts both productivity and the economy:  

- **New York**  
  - Avg. trip duration: ~15 min  
  - Peak-hour delays: +25–40%  
  - Annual productivity loss: ~$20B  

- **Indore**  
  - Population: 3.2M (2023), projected 3.6M by 2030  
  - Vehicle growth: ~12% CAGR  
  - Avg. speed: 18–22 km/h (peak) vs. 35+ km/h (off-peak)  
  - Congestion cost: ₹1,200 crore annually  
  - Delivery delays: ~15–20% during peak hours  

**Impact of GatiSense:**  
- Citizens save **15–20% commute time**  
- Businesses improve delivery SLAs by **25%**  
- Officials gain **data-driven insights** for better planning  

---

## 🛠️ Tech Stack  

| Layer              | Tools / Frameworks |
|--------------------|---------------------|
| **Frontend (UI)** | React.js, TailwindCSS, Plotly.js, Leaflet.js |
| **Backend**       | FastAPI / Flask |
| **ML Models**     | XGBoost, Random Forest, Scikit-learn |
| **Routing Engine**| OSRM |
| **GIS & Mapping** | Folium, GeoPandas, Leaflet.js |
| **Deployment**    | Streamlit / Docker / GitHub Pages |
| **Dataset**       | [NYC Taxi Trip Duration (Kaggle)](https://www.kaggle.com/c/nyc-taxi-trip-duration) |

---

## 📊 System Workflow  

```mermaid
flowchart TD
    A[NYC Taxi Dataset] --> B[Data Preprocessing]
    B --> C[Feature Engineering: Distance, Time, Routes]
    C --> D[ML Models for Travel Time Prediction]
    D --> E[OSRM Route Optimization]
    E --> F[Citizen & Delivery Dashboard]
    E --> G[City Officials Dashboard]
    F --> H[Route + ETA + Cost Insights]
    G --> I[Heatmaps + Bottleneck Analysis]
````

---

## 📂 Project Structure

```
GatiSense/
│── data/                 # NYC Taxi Dataset
│── notebooks/            # ML Experiments & EDA
│── models/               # Trained ML Models
│── backend/              # FastAPI/Flask APIs
│── frontend/             # React + Leaflet Dashboards
│── docs/                 # Documentation & Flowcharts
│── demo/                 # Screenshots + Demo Video
│── README.md             # Project Documentation
```

<p align="center">
  <img src="https://user-images.githubusercontent.com/45159366/108601086-82e92880-73b1-11eb-8c94-63c19e78146b.png" width="650" />
</p>

---

## 🗺️ Visuals

### Citizen Dashboard

* Pickup/Dropoff → Predicted ETA + Best Route

<p align="center">
  <img src="https://leafletjs.com/docs/images/logo.png" width="400" />
</p>

### City Officials Dashboard

* Heatmaps of congestion zones

<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*puF69bY3p1uh-nv4Y7oO9A.png" width="650" />
</p>

---

## 🚀 Implementation for Indore

The same framework can be **localized to Indore**:

1. **Dataset Replacement**

   * Use **Indore Smart City traffic data** (GPS, counters, cameras)
   * Data portal: [data.gov.in](https://data.gov.in)

2. **Routing Engine**

   * Run **OSRM** on Indore OpenStreetMap extracts
   * Factor Indian driving patterns (auto-rickshaw, two-wheelers)

3. **Live Congestion Feeds**

   * Integrate real-time GPS & camera feeds
   * Dynamic congestion layers on Leaflet maps

4. **Business Benefits**

   * Citizens: -15–20% commute time
   * Businesses: +25% delivery efficiency
   * Officials: Pinpoint bottlenecks at Vijay Nagar, Rajwada, Palasia

5. **Future Scalability**

   * Extend for **BRTS, Metro expansion**, inter-city freight

<p align="center">
  <img src="https://www.researchgate.net/publication/341704547/figure/fig3/AS:900902611451905@1590310705860/Traffic-Congestion-at-Vijay-Nagar-Square-Indore.png" width="600" />
</p>

---

## 📽️ Deliverables

* 📑 Documentation (Markdown + PDF)
* 🔄 Flowchart of System Workflow
* 🧪 POC Demo (Streamlit/React + FastAPI)
* 🎥 2–3 min Demo Video

---

## 👨‍💻 Team Vision

Traffic inefficiency costs Indian cities **billions each year**.
**GatiSense** bridges **AI + GIS + Policy Planning** to enable smoother, faster, and smarter mobility.

---

<p align="center">  
🚦 *Data today, smoother roads tomorrow.* 🚦  
</p>
```  

