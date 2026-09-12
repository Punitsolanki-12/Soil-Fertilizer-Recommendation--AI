# Soil-Sense: Smart Farming & Fertilizer Recommender

Hi there! Welcome to my project, **Soil-Sense**. 

I built this as my final capstone project for the **1M1B AI for Sustainability Virtual Internship (2026)**.

## Why did I build this?
I noticed that a lot of farmers rely on guesswork or basic advice when it comes to using fertilizers. Putting too much chemical fertilizer (like Urea) damages the soil in the long run and pollutes the environment. So, I thought, why not use Machine Learning to tell exactly what the soil actually needs? 

This project is my small step towards **UN SDG 12 (Responsible Consumption and Production)**.

## ⚙️ How does it work?
To make this system truly smart and data-driven system. Here is the flow of my project:
1. **The Input:** It takes raw soil parameters (N, P, K, pH) and weather data (Temp, Humidity, Rainfall).
2. **Data Cleaning:** I used `StandardScaler` to normalize the data and `PCA` (Principal Component Analysis) to reduce 7 features down to 5. This removes noise and helps the model learn better.
3. **Crop Prediction:** I trained a `Random Forest Classifier` (which gave me a solid ~92% accuracy) to predict the best crop for those specific conditions.
4. **The "Smart" Fertilizer Logic:** This is the best part! Instead of generic advice, the code mathematically compares the user's soil data with the "ideal" soil data for the predicted crop. It calculates the exact deficit and recommends the exact amount of Urea, DAP, or MOP needed per acre.

##  Tech Stack Used
* **Language:** Python (Google Colab)
* **Data Handling:** Pandas
* **Machine Learning:** Scikit-Learn (PCA, StandardScaler, RandomForest)

##  About Me
I'm **Punit solanki**, currently pursuing my B.Tech in Data Science at IPS Academy, Indore. I'm passionate about exploring how complex data and algorithms can solve real, grassroots problems. Feel free to check out my code!
