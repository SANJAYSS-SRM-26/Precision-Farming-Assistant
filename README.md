# Precision Farming Assistant (PFA)

## Project Description
**PFA: Precision Farming Insights using AI** is a geospatial crop recommendation system that leverages **satellite imagery, soil data, and weather data** to suggest the most suitable crop for any given geographical location.

The system is designed to assist farmers and agricultural planners in:
- Optimizing land usage  
- Improving crop yield  
- Reducing overuse of water and fertilizers  

It integrates multi-dimensional environmental data from globally available sources and uses a **LightGBM machine learning model** to deliver accurate, location-specific crop recommendations.

Additionally, the system identifies **barren or underutilized land** and suggests rehabilitation strategies, making it scalable across diverse agro-ecological zones.

---

## How It Works

### User Input
- Geographic coordinates (latitude, longitude) are entered manually  
- Or selected via an interactive map  

### Data Collection
- **NDVI (Vegetation Health)** → MODIS via Google Earth Engine  
- **Soil Data (pH, Nitrogen)** → ISRIC SoilGrids  
- **Weather Data (Temperature, Humidity, Rainfall)** → NASA POWER  

### Processing Pipeline
- Data is validated and normalized  
- Integrated into a unified feature vector  
- Passed into a trained **LightGBM model**  

### Output Generation
- Primary crop recommendation  
- Top alternative crops  
- Precision farming insights:
  - Irrigation strategies  
  - Fertilizer recommendations  
  - Soil improvement suggestions  
- Rehabilitation advice for barren/low-NDVI land  

---

## Tech Stack

### Frontend
- HTML  
- CSS  
- JavaScript  

### Backend
- Python (Flask)  
- REST APIs for geospatial data processing  
- Deployment: **Render**  

### Machine Learning
- LightGBM  
- Trained on crop-environment suitability dataset  

### Data Sources / APIs
- Google Earth Engine (MODIS NDVI)  
- ISRIC SoilGrids  
- NASA POWER  
- OpenCage Geocoder (fallback)  
- ICFA Crop Dataset  

---

## System Design

![System Architecture](https://github.com/SANJAYSS-SRM-26/Precision-Farming-Assistant/blob/main/system%20flow.png)

---

## Key Features

- Location-based crop recommendation  
- Multi-source geospatial data integration  
- Machine learning-driven predictions  
- Precision farming insights  
- Barren land identification & rehabilitation  
- Real-time API-based system  

---

## Model Performance

- LightGBM Accuracy: **~95.9%**
- Supports: **22 crop types**
- Low latency suitable for real-time usage  

---

## Future Improvements

- Mobile application for farmers  
- Voice-based interaction  
- Multi-crop & intercropping recommendations  

---

## Authors

- **Sanjay S S**  
- **Akul Abrol**  
  
---

### API Info

Gather API Key from platforms and run the system

---

## Project Insight

This project bridges the gap between **traditional agriculture and modern AI-driven decision systems**, making precision farming **accessible, scalable, and sustainable**.

