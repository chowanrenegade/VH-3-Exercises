# Awareness Exercise Generator

A minimalist productivity and self-awareness tool designed to provide users with three random "conscious reminders" per day as recommended by Vernon Howard. This tool is based on psychological and spiritual practices aimed at breaking mechanical behavior and increasing present-moment awareness.

---

## 🧘 Overview

The philosophy of this tool is rooted in the "Do for full day" method. By generating three specific prompts, the user is encouraged to practice these specific states of mind for 24 hours before rotating to a new set of exercises the following day.

---

## ✨ Features

* **Curated Exercises:** Includes over 20 unique prompts such as "SLOW DOWN," "DETACHMENT FROM EVENT," and "CATCH ARTIFICIAL BEHAVIOUR."
* **No Duplicates:** The generator logic ensures that the three prompts selected in a single click are always unique.
* **Minimalist Interface:** A distraction-free "Click me" interface to keep the focus on the practice itself.
* **Lightweight & Offline:** A single HTML file that requires no internet or external libraries.

---

## 🧠 How It Works

The script manages a list of exercises and performs a "destructive" random selection process:

1. **Array Storage:** All prompts are stored in a JavaScript array.
2. **Loop Selection:** The function runs a `for` loop exactly three times.
3. **Randomization:** It uses `Math.floor(Math.random() * exercises.length)` to pick a valid index.
4. **Splicing:** Crucially, it uses `.splice()` to remove the chosen exercise from the temporary list, ensuring the
