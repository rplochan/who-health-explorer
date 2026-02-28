# 🌍 WHO Health Explorer

An interactive, browser-based dashboard that combines **RestCountries API** and the **WHO Global Health Observatory (GHO) API** to display real-time country health data — no backend, no API keys, no build step required.

![WHO Health Explorer Preview](https://img.shields.io/badge/Live-Demo-00e5a0?style=flat-square) ![No API Key](https://img.shields.io/badge/API%20Key-Not%20Required-3d8bff?style=flat-square) ![Vanilla JS](https://img.shields.io/badge/Built%20With-Vanilla%20JS-ffd166?style=flat-square)

---

## ✨ Features

- 🔍 **Search any country** with live autocomplete
- 🏳️ **Country overview** — flag, population, capital, currency, languages
- 📊 **8 WHO health indicators** per country:
  - ❤️ Life Expectancy at Birth
  - 👶 Under-5 Mortality Rate
  - ♂️ Adult Mortality (Male)
  - ♀️ Adult Mortality (Female)
  - ⚖️ Obesity Rate
  - 💉 Measles Vaccination Coverage
  - 🩺 DTP3 Vaccination Coverage
  - 🤱 Maternal Mortality Ratio
- 📅 Shows **data year** for each WHO indicator
- 📈 Visual **progress bars** for quick comparison
- ⚡ Quick-pick buttons for popular countries

---

## 🚀 Getting Started

### Option 1: Open directly in browser
```bash
git clone https://github.com/YOUR_USERNAME/who-health-explorer.git
cd who-health-explorer
open index.html   # macOS
# or just double-click index.html on Windows/Linux
```

### Option 2: Serve locally
```bash
# Python
python -m http.server 8000

# Node.js (npx)
npx serve .
```
Then open `http://localhost:8000`

### Option 3: Deploy to GitHub Pages
1. Push to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your app will be live at `https://YOUR_USERNAME.github.io/who-health-explorer`

---

## 🔌 APIs Used

| API | Base URL | Auth |
|-----|----------|------|
| [RestCountries](https://restcountries.com/) | `https://restcountries.com/v3.1/` | ✅ None required |
| [WHO GHO API](https://www.who.int/data/gho/info/gho-odata-api) | `https://ghoapi.azureedge.net/api/` | ✅ None required |

Both APIs are completely free and open — no signup, no API key, no rate limit worries for typical usage.

---

## 📁 Project Structure

```
who-health-explorer/
├── index.html       # Main app (single-file, self-contained)
├── README.md        # You're reading this
├── LICENSE          # MIT License
└── .gitignore       # Standard web gitignore
```

---

## 🛠️ Tech Stack

- **Pure HTML / CSS / JavaScript** — zero dependencies, zero build tools
- **Google Fonts** — Playfair Display + DM Mono
- **WHO OData API** — filtered by country ISO3 code
- **RestCountries v3.1** — country metadata

---

## 📊 WHO Indicator Codes Reference

| Indicator | WHO Code |
|-----------|----------|
| Life Expectancy | `WHOSIS_000001` |
| Under-5 Mortality | `MDG_0000000026` |
| Adult Mortality (Male) | `WHOSIS_000015` |
| Adult Mortality (Female) | `WHOSIS_000016` |
| Obesity Rate | `NCD_BMI_30C` |
| Measles Vaccination | `WHS4_100` |
| DTP3 Vaccination | `WHS4_117` |
| Maternal Mortality | `MDG_0000000020` |

Browse all available indicators at: [ghoapi.azureedge.net/api/Indicator](https://ghoapi.azureedge.net/api/Indicator)

---

## 🤝 Contributing

Contributions welcome! Some ideas:
- Add more WHO indicators
- Add country comparison (side-by-side)
- Add historical trend charts (Chart.js)
- Add export to CSV/PDF

```bash
git checkout -b feature/your-feature
git commit -m "Add your feature"
git push origin feature/your-feature
# Open a Pull Request
```

---

## 📄 License

MIT © 2025 — free to use, modify, and distribute.
