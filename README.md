# 🥛 Milk Recommendation System

## 📌 Overview

Milk Recommendation System is a personalized milk recommendation web application created through collaboration between students interested in Biology and Computer Science.

Our project combines:

* nutrition analysis,
* recommendation systems,
* barcode scanning,
* and data standardization.

Unlike simple information websites, our application focuses on:

> helping users compare milk products fairly and receive personalized recommendations.

---

# 🌱 Motivation

This project started from our simple curiosity.

Most milk products look very similar from the outside. However, their tastes are different, and every company advertises that their product is healthier or better for consumers.

This made us question:

> “Which milk is actually good for our health?”

We wanted to compare products scientifically rather than relying only on advertisements or packaging.

At first, our goal was simple:

* collect nutrition information,
* compare products,
* and explain health-related differences.

However, during development, we encountered an important problem.

---

# 💭 Story Behind the Project

At first, our team was not fully unified about the project direction.

I suggested creating a milk information website, and Zion initially agreed with the idea. However, as we continued discussing, we began questioning whether the project was truly useful.

Zion pointed out an important issue:

> “People can already find nutrition information on the internet. The nutrition facts are also written on the side of the milk package.”

His opinion was reasonable, and it made us rethink the purpose of the project.

We realized that:

> simply displaying information would not give users a strong reason to use our service.

Because of this, we shifted our focus from:

```text
Simple Information Display
```

to:

```text
Personalized Recommendation and Comparison
```

Instead of only showing nutrition facts, we decided to:

* recommend products based on personal preferences,
* compare products automatically,
* and explain why a specific milk is suitable for a user.

Later, our teacher advised us to make the project more interactive and visually engaging.

He suggested that:

> recognizing milk products through scanning could become an important feature.

After receiving this feedback, we expanded the project further by adding:

* barcode scanning,
* API integration,
* and product recognition features.

This became one of the biggest turning points in our project.

---

# 🚩 Problem Statement

Many milk products use different serving-size standards.

For example:

* some products use 100mL,
* others use 200mL,
* and some use bottle-based servings.

Because of this:

* products are difficult to compare fairly,
* users must calculate nutrition manually,
* and recommendation systems become inaccurate.

---

# ✅ Our Solution

Our application solves these problems through:

```text
Barcode Scanning
        ↓
Nutrition Data Collection
        ↓
100mL Standardization
        ↓
Preference-Based Recommendation
        ↓
Product Comparison
```

The system:

* standardizes nutrition values,
* compares products fairly,
* recommends products based on user preferences,
* and explains nutritional differences clearly.

---

# 🔄 Development Process

## Stage 1 — Information Website

Initial Goal:

* organize milk nutrition data,
* create comparison tables,
* explain health information.

Problem:

* similar information already existed online,
* lack of originality and usefulness.

---

## Stage 2 — Personalized Recommendation

We introduced:

* low sugar preferences,
* high protein preferences,
* lactose-free filtering,
* and price importance settings.

This transformed the project into:

> a personalized recommendation system.

---

## Stage 3 — Barcode Recognition

We added:

* barcode scanning,
* Open Food Facts API integration,
* automatic product lookup.

This improved accessibility and usability.

---

## Stage 4 — Nutrition Standardization

We discovered another major issue:

Different products used different nutrition standards.

For example:

```text
Product A → 200mL standard
Product B → 100mL standard
```

Direct comparison was misleading.

To solve this issue, we standardized all nutrition information into:

> per 100mL values.

This became one of the most important technical aspects of our project.

---

# ⚙️ Core Features

## ✅ Personalized Recommendation

Users can select:

* low sugar,
* high protein,
* lactose free,
* low fat,
* price importance.

The application calculates recommendation scores automatically.

---

## ✅ Barcode Scanner

Users can scan products directly using their device camera.

The application retrieves product information automatically.

---

## ✅ 100mL Standardization

All nutritional information is converted into:

> standardized 100mL-based values.

This allows fair product comparison.

---

## ✅ Product Comparison

Users can compare:

* calories,
* sugar,
* protein,
* calcium,
* price.

---

# 🧬 Biology Contributions

The biology-related aspects include:

* nutritional analysis,
* sugar intake comparison,
* protein analysis,
* lactose intolerance research,
* low-fat and non-fat milk comparison.

The project focuses on helping users make healthier dietary choices.

---

# 💻 Computer Science Contributions

The computer science-related aspects include:

* recommendation algorithms,
* weighted scoring systems,
* nutrition database design,
* barcode recognition,
* API integration,
* dynamic UI rendering,
* data normalization.

---

# 🗂️ Mind Map

```text
Milk Recommendation System
│
├── Nutrition Database
│   ├── Calories
│   ├── Sugar
│   ├── Protein
│   ├── Calcium
│   └── Price
│
├── Personalized Recommendation
│   ├── Low Sugar
│   ├── High Protein
│   ├── Lactose Free
│   ├── Low Fat
│   └── Price Importance
│
├── Barcode Recognition
│   ├── Camera Input
│   ├── Product Detection
│   └── API Integration
│
├── Nutrition Standardization
│   ├── 100mL Conversion
│   └── Fair Comparison
│
└── Product Comparison
    ├── Calories
    ├── Sugar
    ├── Protein
    ├── Calcium
    └── Price
```

---

# 🚀 Future Directions

Possible future improvements include:

## More Product Expansion

* add more milk brands,
* expand into American products,
* include international products.

## AI Recommendation System

* AI-based health recommendations,
* machine learning recommendation models,
* personalized dietary analysis.

## User Review System

Users can:

* leave reviews,
* score products,
* and contribute to community-based rankings.

## Actual Intake Calculation

Future versions may:

* calculate real nutritional intake,
* based on how much milk users actually drink.

## OCR Recognition

Future versions may:

* recognize nutrition labels directly from images,
* without requiring barcodes.

---

# ⚠️ Limitations

Current limitations include:

* limited milk database,
* dependence on external APIs,
* rule-based recommendation system,
* OCR recognition not fully implemented yet.

---

# 🛠️ Technologies Used

* HTML
* CSS
* JavaScript
* Open Food Facts API
* Netlify
* GitHub
* Google Spreadsheet

---

# 📌 Conclusion

This project began as a simple milk information website but gradually evolved into:

> a personalized nutrition recommendation platform.

More importantly, this project taught us:

* iterative problem solving,
* interdisciplinary collaboration,
* user-centered design,
* and how to improve ideas through criticism and feedback.

Rather than stopping at simple information delivery, we continuously asked:

> “Why would users actually use this service?”

That question became the foundation of our project’s growth.
