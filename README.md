# 🍻 BAC TRAC

**BAC TRAC** is a lightweight, browser-based widget designed for stream overlays.  
It continuously estimates **Blood Alcohol Content (BAC)** based on:

- body weight  
- gender  
- what you’re drinking  
- sip size  
- time passing (BAC slowly falls as you metabolise alcohol)

It’s ideal for creators who want a fun, transparent way to track estimated BAC during a stream — **purely for entertainment and awareness.**

> ⚠️ **Important:** This tool provides an **estimate only** and should **never** be used to judge whether you are safe to drive, operate equipment, or make safety-critical decisions.

---

## 🧪 How It Works

BAC TRAC uses the **Widmark formula**, combined with an average metabolism rate, to:

✔ instantly add BAC when you record a sip  
✔ slowly reduce BAC in real-time  
✔ convert drink volume & ABV into ethanol mass  
✔ keep a running total over time  

### Core assumptions

- **Instant absorption**
  - Real life absorption = ~30–90 minutes  
  - This app assumes alcohol reaches the bloodstream immediately

- **Average metabolism**
  - ≈ **0.015 % BAC per hour**

- **Widmark r-factor**
  - Male → **0.68**
  - Female → **0.55**

- **Ethanol density**
  - **0.789 g/ml**

These are widely used public health & research averages.

---

## 🚀 Getting Started

### 1️⃣ Download the release
Download the latest `.html` file.

### 2️⃣ Open it
Open it in **any modern browser** — no install needed.

### 3️⃣ (Optional) Add to OBS
Add as a **WINDOW CAPTURE**  
Crop the settings panel so only the live BAC display is shown.
It __**WILL NOT**__ work as a browser source as you will not be able to edit the settings or press the sip button until later versions.

Done 👍

---

## 🍺 Setting Your Drink Correctly

BAC TRAC works for any drink where you know:

- **Total Drink Volume (ml)**  
- **Alcohol Volume (ml)** — the alcohol liquid only (e.g., vodka amount in a mixed drink like a vodka lemonade)  
- **ABV (%)**  
- **Sip Size (ml)** — your average mouthful  

### Example — 500ml Beer @ 6%

| Field | Value |
|------|-------|
| Total Drink Vol | `500` |
| Alcohol Vol | `500` |
| ABV (%) | `6` |
| Sip Size | however much you drink per sip |

### Example — Vodka Lemonade

| Field | Value |
|------|-------|
| Total Drink Vol | `400` |
| Alcohol Vol | `50` |
| ABV (%) | spirit ABV (e.g. `37.5`) |
| Sip Size | your sip size |

> ⚠️ This **will not work for cocktails** unless you know the alcohol volume.

You can **change parameters mid-session** (new drink, new glass, etc.) and tracking continues normally.

---

## 🕒 Real-Time Metabolism

BAC slowly falls over time based on:

- weight  
- gender  
- metabolism rate  

This is calculated continuously.

> ⚠️ Absorption time is **not included** — BAC rises instantly after a sip.

This is a simplification.

---

## 🎯 Intended Use

This widget is meant for:

- streaming overlays  
- fun experiments  
- educational curiosity  
- self-awareness  

It is **not medical software** and **not legally accurate**.

---

## ⚠️ Safety Disclaimer

- BAC values are **estimates only**
- Real BAC varies person-to-person
- Medications, illness, hydration, tolerance, food etc all change results
- **Do not drink and drive**
- **Do not use this tool to assess fitness for work or safety**

If you feel unwell while drinking — **seek help.**

---

## 📦 Requirements

- Any modern browser
- That’s it 🙂

---

## ❤️ Credits

Created for fun and streaming use.  
Built using JavaScript and the Widmark BAC model.

---

## 🙌 Contributions / Suggestions

Suggestions welcome!  
Ideas I may add in future:

- colour-coded impairment zones  
- sober-by countdown  
- configurable metabolism rate  
- Twitch/stream hotkeys  

Feel free to open a PR or share feedback.
