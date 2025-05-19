# 🏥 Healthcare Diagnostic and Treatment

## 🎯 Objective
**Healthcare Diagnostic and Treatment** is designed to help users identify potential diseases based on their symptoms, providing basic treatment advice, lifestyle tips, and urgency levels for medical attention. It also logs user feedback for future improvements.

> ⚠️ **Disclaimer:** This tool is *not* a substitute for professional medical advice. Always consult a doctor before taking any medication.

---

## ✨ Features
- 🔍 Diagnoses **7 common diseases** based on user-input symptoms (e.g., fever, chest pain, sore throat).
- 💊 Provides **treatment advice**, including medicines and lifestyle recommendations.
- 🚨 Assigns **urgency levels**: Low, Medium, High.
- 🗂 Logs **user feedback** with timestamps in a `feedback.log` file.
- 📢 Displays a **disclaimer** to remind users to consult a doctor.

---

## 🛠️ Technology Used
- **Language:** Python  
- **Libraries:**
  - `datetime` – for timestamp logging  
- **Tools:**
  - File I/O – for saving feedback to `feedback.log`

---

## ⚙️ How It Works
1. The user enters their **name** and a short description of **symptoms** (e.g., “I have a fever”).
2. The `smart_match()` function maps the symptoms to one of **7 diseases** in the database.
3. If matched, the program outputs:
   - 🦠 Possible **disease**
   - 🚦 **Urgency level** (Low / Medium / High)
   - 💊 **Treatment advice** (medicines + lifestyle tips)
   - 📝 A **note** about the condition
4. User gives **feedback** ("Was this helpful?"), which is logged with a timestamp.
5. The program repeats unless the user types **“exit”**.

---

## 📊 Data Collection
- Uses a **hardcoded dictionary** called `disease_db` in the script.
- Contains data for **7 diseases** (e.g., Viral Infection, Gastritis, Angina).
- All data is **manually curated**—no external sources used.

---

## 🎮 Controls
- **Input:** User interacts via the console.
- **Exit:** Type `"exit"` when prompted for the name to quit the program.
- **Loop:** The app runs continuously until exited.

---

## 🧠 ML Techniques Used
No machine learning used.  
This is a **rule-based system** using `smart_match()` function with **string matching** logic.

---

## 📤 Output Explanation
The program prints:
- **Diagnosis:** Possible disease (e.g., `Possible Disease: Viral Infection`)
- **Urgency:** Medical advice level (e.g., `Seek immediate medical attention`)
- **Treatment Advice:** Medicines and lifestyle tips (e.g., `Paracetamol – consult doctor`, `Rest well, stay hydrated`)
- **Note:** Context about the disease (e.g., `Usually caused by seasonal infection`)
