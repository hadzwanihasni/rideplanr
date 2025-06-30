# 🛵 RidePlanr – Smart Weather & Traffic Helper for Your Commute

**RidePlanr** is a GPT-powered assistant that helps motorcycle riders decide whether it's safe to travel between any two locations — based on **real-time weather forecasts** and **live traffic navigation via Waze**.

This project uses **free public APIs** with **no authentication required** and leverages **OpenAI GPT Actions** to dynamically:
- Convert any place into GPS coordinates using **Nominatim**
- Fetch hourly weather forecasts from **Open-Meteo**
- Generate Waze route links for **live traffic checks**
- Recommend whether to ride or not, based on rain, wind, and temperature

---

## 🎯 Use Case

> “Should I ride from Kulim to Bayan Lepas tomorrow at 8AM?”

RidePlanr will:
1. Geocode Kulim and Bayan Lepas → latitude + longitude
2. Call Open-Meteo to get weather forecast at that time
3. Analyze conditions: rain, wind, temperature
4. Output a safety recommendation
5. Generate a Waze link to check live traffic status manually

---

## 📦 Tech Stack

| Component                                              | Purpose                                      |
|--------------------------------------------------------|----------------------------------------------|
| OpenAI GPT Actions                                     | Powers the assistant logic and API calls     |
| [Nominatim API](https://nominatim.org/)                | Converts location names to GPS coordinates   |
| [Open-Meteo API](https://open-meteo.com/)              | Provides hourly forecast data                |
| [Waze Deep Links](https://www.waze.com/live-map)       | Enables quick access to live traffic         |
| GitHub Pages                                           | Hosts public API schemas for GPT             |

---

## 🚀 Getting Started

### 1. 🧬 Fork this Repository
Create your own copy on GitHub.

### 2. 🌐 Enable GitHub Pages
Go to `Settings → Pages → Branch: main → /root`.

### 3. 🔗 Copy these URLs
After Pages is enabled, get public links to:
- `openapi-nominatim.yaml`
- `openapi-meteo.yaml`

### 4. 🧠 Build the GPT
Go to [https://chat.openai.com/gpts](https://chat.openai.com/gpts) → "Create":
- Set instructions: “Help users decide if it's safe to ride by checking weather, generating Waze links, etc.”
- Add both Actions using your GitHub Pages URLs

---

## 🧪 Sample Prompts

> “Should I ride from Kulim to Bayan Lepas tomorrow morning?”

> “Give me weather and traffic for my commute at 7AM from Juru to Queensbay.”

> “Will there be rain if I ride from KL Sentral to UM tomorrow night?”

---

## 🔧 Waze Integration

RidePlanr also provides Waze links like:

[https://www.waze.com/ul?ll=5.4164,100.3327&navigate=yes](https://www.waze.com/ul?ll=5.4164,100.3327&navigate=yes)

Use this link to:
- Launch route in Waze
- View live traffic, road closures, and delays

---

## 📁 File Structure

```markdown
📁 rideplanr/
├── README.md
├── LICENSE
├── openapi-nominatim.yaml     # Place → Coordinates
├── openapi-meteo.yaml         # Coordinates → Weather
```

---

## ⚖ License

This project is licensed under the MIT License — free to use, modify, and enhance.

---

## 🤖 Author

Built by [@hadzwanihasni](https://github.com/hadzwanihasni)  
Made for AI-native commuters — optimized for simplicity, action, and clarity.

