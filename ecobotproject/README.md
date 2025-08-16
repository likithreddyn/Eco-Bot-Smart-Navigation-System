
# 🌍 EcoBot – AI-Powered AQI-Based Navigation Assistant

EcoBot is an **AI-powered chatbot navigation system** designed to revolutionize travel with eco-conscious route planning.  
By combining **Google Maps API** for route suggestions and **AQICN API** for real-time Air Quality Index (AQI) monitoring,  
EcoBot recommends the cleanest possible travel routes, encourages sustainable transportation choices,  
and rewards users with **Carbon Coins** for eco-friendly behavior.

---

## 🚩 Problem Statement

Transportation contributes significantly to **air pollution** and **carbon emissions**, as highlighted by EPA data.  
Conventional navigation systems prioritize speed or distance without considering **environmental impact**.  
This leads to route choices that may increase exposure to poor air quality and worsen pollution levels.

---

## 💡 Our Solution

EcoBot addresses this challenge by integrating **real-time AQI data** into route planning:  

- **Step 1:** User inputs **origin** and **destination** via chatbot interface.  
- **Step 2:** Google Maps API fetches multiple route options.  
- **Step 3:** AQICN API analyzes AQI levels along each route.  
- **Step 4:** it recommends the **cleanest route** with AQI score and transport advice.  
- **Step 5:** Users earn **Carbon Coins** for choosing sustainable transport, redeemable for rewards.

---

## ✨ Key Features

- **🌱 Real-Time AQI-Based Route Optimization**  
  Selects travel routes with the lowest pollution exposure.

- **🚲 Eco-Friendly Transport Recommendations**  
  - 🚗 Car/Bike for low AQI  
  - 🚴 Bike or walking for moderate AQI  
  - 🚌 Public transport for high AQI  
  - 😷 Mask alerts for hazardous conditions  

- **💰 Carbon Coin Rewards System**  
  Earn coins for eco-conscious travel, redeemable via partner businesses.

- **🤖 AI Chatbot Assistance**  
  Built with **Flask + OpenAI API** for natural user interaction.

---

## 🏗 Technical Architecture

| Layer         | Technology Used                           | Purpose |
|---------------|-------------------------------------------|---------|
| Frontend      | HTML, CSS, JavaScript                      | User interface for chatbot and AQI results |
| Backend       | Flask (Python)                             | API requests, AQI processing, and route logic |
| APIs          | Google Maps API, AQICN API, OpenAI API     | Route data, AQI data, chatbot responses |
| Rewards Logic | Python Random Module                       | Carbon Coin generation based on AQI levels |

---

## 📊 User Experience Flow

1. **User**: Inputs "From" and "To" locations in chatbot.  
2. **System**: Fetches coordinates via Google Maps API.  
3. **System**: Retrieves AQI values for routes using AQICN API.  
4. **System**: Calculates cleanest route & suggests transport mode.  
5. **System**: Displays Google Maps link, AQI score, transport suggestion, and Carbon Coins earned.  

---

## 📈 Impact

- Promotes **eco-friendly transportation choices** to reduce emissions.  
- Encourages **public transport usage** to improve public health.  
- Raises awareness about **air quality** and personal exposure risks.  

---

## 🔮 Future Development

- Integrate **real-time traffic** and **weather data**.  
- Partner with local businesses for **reward redemption**.  
- Expand to **global cities** with localized AQI and transport data.  

---
I see what happened — your code block formatting broke in the **"Clone the repository"** section.
It’s because you started a triple backtick code block but didn’t close it properly before writing the next steps.

Here’s the **fixed README section** with correct Markdown formatting:

---

````markdown
## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/likithreddyn/Eco-Bot-Smart-Navigation-System
cd ecobot
```

### 2. Create a virtual environment & install dependencies

```bash
python -m venv venv
source venv/bin/activate  # On Mac/Linux
venv\Scripts\activate     # On Windows
pip install -r requirements.txt
```

### 3. Create a `.env` file in the project root

```ini
GOOGLE_MAPS_API_KEY=your_google_maps_key
AQICN_API_KEY=your_aqicn_key
OPENAI_API_KEY=your_openai_key
```

### 4. Run the Flask app

```bash
python app.py
```
