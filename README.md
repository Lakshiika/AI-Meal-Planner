# AI-Meal-Planner (Plateful Planner)
AI Meal Planner App is a smart web application that generates personalized meal plans based on your daily calorie needs and food preferences. It combines the power of AI (Llama-3 via Groq API) and optimization algorithms to create balanced, nutritious, and creative meal suggestions for breakfast, lunch, and dinner.

## 🚀 Features

- 🔢 Calculates daily calorie needs using age, height, weight, and gender
- 📏 Supports both metric (kg, cm) and imperial (lb, ft+in) units
- 🥦 Lets you choose food preferences, allergies, or dietary restrictions
- 📊 Generates optimized meal plans for breakfast, lunch, and dinner
- 🤖 Uses Llama-3 70B (Groq API) to generate creative meal names/descriptions
- 🍽️ Shows detailed nutritional breakdown for each meal

---

## 🛠️ Tech Stack

- **Python** – Core logic and backend
- **Streamlit** – Interactive web interface
- **Pandas** – Data manipulation and food database handling
- **Groq API** – To access the Llama-3 70B model for AI-powered text generation
- **Knapsack Algorithm** – Optimizes food selections to meet calorie targets

---

At the heart of the app is the Knapsack algorithm, which helps plan each meal efficiently:

Based on your Basal Metabolic Rate (BMR), it divides your total daily calories as:

50% for breakfast

33% for lunch

17% for dinner

For each meal:

It scans through all available food options

Selects the best combo of items that stay within the calorie limit

Uses dynamic programming to find the most optimal combination

Outputs the chosen items along with their nutritional breakdown

Once the ingredients are finalized, they’re passed to the Llama-3 AI, which adds a creative touch by generating names and descriptions for each meal.
