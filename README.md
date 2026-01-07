# Offline Swiss Ephemeris – Tantric Dark Mode

An **offline, Swiss-Ephemeris–based astrology calculation tool** with a dark Tantric UI, built using **Python + Tkinter**.  
Designed for **Vedic / KP astrology**, supporting **Lahiri, KP New, and Raman ayanamsha**.

This project performs **accurate planetary, Rahu–Ketu (mean & true), Lagna, and cuspal calculations** completely offline.

## ⬇️ Download (Windows EXE)

👉 **[Download Tantric Swiss Ephemeris – Windows EXE]
(https://github.com/DonnieDarsshan/tantric-swiss-ephemeris/releases)**

- No Python required
- Fully offline
- Includes Swiss Ephemeris files



---

## ✨ Features

- ✅ Fully **offline Swiss Ephemeris**
- 🌑 Dark Tantric UI (high-contrast, eye-safe)
- 🕉️ Ayanamsha support:
  - Lahiri
  - KP New (Krishnamurti)
  - Raman
- 🌍 Accurate UTC conversion with DST
- 🪐 Calculates:
  - All classical planets
  - Rahu (Mean & True)
  - Ketu (Mean & True)
  - Lagna
  - 12 Placidus cusps
- 💾 Outputs clean **JSON files**
- 📦 Ready for **EXE packaging (PyInstaller)**

---

## 📂 Project Structure

offline-swiss-ephemeris/
│
├── main.py # Main application
├── settings.json # Auto-generated user settings
├── ephe/ # Swiss Ephemeris files
│ ├── sepl_18.se1
│ ├── semo_18.se1
│ └── ...
├── README.md
├── .gitignore

---

## 🔧 Requirements

- Python **3.9+**
- Swiss Ephemeris Python binding

Install dependencies:

```bash
pip install pyswisseph

How to Run (Source)
python main.py



Output Format (JSON)

Each calculation generates a JSON file containing:
Meta data (name, ayanamsha, UTC datetime)
Planetary longitudes
Lagna
All 12 cusps


{
  "meta": {},
  "lagna": 123.45,
  "planets": {},
  "cusps": {}
}



🧪 Accuracy Notes
Uses Swiss Ephemeris official algorithms
Rahu/Ketu calculations follow Swiss standard
Cusps are calculated in sidereal mode


📦 Building EXE (Optional)
You can convert this project into a standalone Windows EXE using PyInstaller.

pyinstaller --onefile --noconsole main.py


⚠️ Legal & Licensing Notes
Swiss Ephemeris data files are subject to Astrodienst license
This project is intended for research, educational, and personal use
Commercial use requires proper Swiss Ephemeris licensing

🙏 Credits
Swiss Ephemeris – Astrodienst
Python, Tkinter
Built with precision for serious astrologers



---

## B) STEP-BY-STEP: HOW TO UPLOAD TO GITHUB (PROPERLY)

### 1️⃣ Create Repository
- Go to GitHub → **New Repository**
- Name suggestion:
- Public ✔️
- Add README ❌ (you already have one)

---

### 2️⃣ Add `.gitignore` (IMPORTANT)

Create a file named `.gitignore` and paste:
pycache/
build/
dist/
*.exe
settings.json



👉 This prevents junk files from being committed.

---

### 3️⃣ Folder Check Before Upload
Your folder should look like:
offline-swiss-ephemeris/
├── main.py
├── ephe/
│ ├── *.se1
├── README.md
├── .gitignore

✔️ This is **perfect**

---

### 4️⃣ Git Commands

```bash
git init
git add .
git commit -m "Initial release: Offline Swiss Ephemeris Tool"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/offline-swiss-ephemeris.git
git push -u origin main




















