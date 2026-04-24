# 🍲 Food Recipe Generator using AI

> An intelligent web-based application that generates complete cooking recipes from food images using Deep Learning and Django.

---

## 📋 Table of Contents

* [Overview](#overview)
* [Features](#features)
* [How It Works](#how-it-works)
* [Tech Stack](#tech-stack)
* [Installation](#installation)
* [Usage](#usage)
* [Project Structure](#project-structure)
* [Model Details](#model-details)
* [Future Enhancements](#future-enhancements)

---

## 🎯 Overview

The **Food Recipe Generator** is an AI-powered system that takes a food image as input and automatically generates:

* 🍴 Dish Name
* 🧂 Ingredients Required
* ⏱ Cooking Time
* 📖 Step-by-step Recipe
* 🍽 Recommended Similar Dishes

This system leverages **Computer Vision and Deep Learning** to analyze food images and provide meaningful culinary insights, enhancing user experience in cooking and meal planning.

---

## ✨ Features

* 📸 Upload any food image
* 🤖 AI-based dish recognition
* 🧾 Automatic recipe generation
* 🧂 Ingredient extraction
* ⏱ Estimated cooking time
* 🍽 Smart recommendation system (similar dishes)
* 🌐 User-friendly web interface (Django-based)

---

## ⚙️ How It Works

1. **Image Input**

   * User uploads a food image

2. **Image Processing**

   * Image is preprocessed using `Pillow` and `NumPy`

3. **Model Prediction**

   * Deep learning model (TensorFlow/Keras) predicts the dish

4. **Recipe Mapping**

   * Predicted dish is matched with dataset (`indian_recipes.json`)

5. **Output Generation**

   * Displays:

     * Ingredients
     * Cooking time
     * Recipe steps

6. **Recommendation System**

   * Suggests similar dishes based on category (e.g., paneer dishes)

---

## 🛠 Tech Stack

| Layer            | Technology                |
| ---------------- | ------------------------- |
| Frontend         | HTML, CSS                 |
| Backend          | Django                    |
| ML Framework     | TensorFlow, Keras         |
| Image Processing | Pillow, NumPy             |
| Dataset          | JSON-based recipe dataset |
| Database         | SQLite                    |

---

## 🚀 Installation

### 🔧 Prerequisites

* Python 3.9+
* pip

---

### ⚙️ Steps

```bash
# Clone the repository
git clone https://github.com/keerthisaa/Food-Recipe-Generator.git

# Navigate to project folder
cd Food-Recipe-Generator

# Create virtual environment
python -m venv venv

# Activate environment
# Windows
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run server
python manage.py runserver
```

---

## 💻 Usage

1. Open browser:

   ```
   http://127.0.0.1:8000
   ```

2. Upload a food image

3. View:

   * Predicted dish name
   * Ingredients
   * Cooking instructions
   * Recommended dishes

---

## 📁 Project Structure

```
FoodRecipeGenerator/
├── src/
│   ├── RecipeLens/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   │
│   ├── main/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── encoder.py
│   │   ├── static/
│   │   └── templates/
│   │
│   ├── db.sqlite3
│   └── manage.py
│
├── requirements.txt
└── README.md
```

---

## 🤖 Model Details

* Framework: TensorFlow + Keras
* Type: Image Classification Model
* Input: Food Image
* Output: Dish Name

### 📊 Pipeline

* Image resizing & normalization
* Feature extraction
* Classification using trained model
* Mapping with recipe dataset

---

## 🍽 Recommendation System

* Based on predicted dish category
* Suggests related dishes (e.g., paneer → paneer butter masala, paneer tikka)
* Uses dataset similarity mapping

---

## 🔮 Future Enhancements

* 🔊 Voice-based recipe assistant
* 📱 Mobile application integration
* 🌍 Multi-cuisine dataset expansion
* 🧠 Improved recommendation using NLP
* ☁️ Cloud deployment

---

## ❤️ Acknowledgement

This project was developed as part of an academic initiative to explore **AI in real-world applications**, specifically in food recognition and personalized recipe generation.

---

## 📌 Conclusion

The Food Recipe Generator demonstrates how **Artificial Intelligence + Web Development** can simplify everyday tasks like cooking by providing instant, intelligent, and personalized recipe suggestions.

---
