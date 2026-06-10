# 🥛 Milk Recommendation System
## Overview
Milk Recommendation System is a personalized milk recommendation web application developed through collaboration between students interested in Biology and Computer Science.
The project combines:
- nutrition analysis,
- recommendation systems,
- barcode scanning,
- and data standardization.
Unlike simple nutrition information websites, our project focuses on:
> fair comparison and personalized recommendations.
---
# 🌱 Motivation
The project began with a simple question:
> “Why is it difficult to compare milk products fairly?”
At first, we only planned to:
- organize milk nutrition information,
- compare products,
- and explain health-related differences.
However, we realized that:
> users could already search nutrition information online.
This made us rethink the purpose of the project.
We then shifted our focus from:
```text
Information Display
```
to:
```text
Personalized Recommendation and Fair Comparison
```
---
# 🚩 Problem Statement
Many milk products use different serving-size standards.
Examples:
- 100mL
- 200mL
- 1 bottle
- 1 serving
This creates several problems:
```text
• Difficult to compare products fairly
• Users must calculate nutrition manually
• Personalized recommendations are unavailable
• Actual intake differs from label information
```
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
Preference-Based Scoring
        ↓
Personalized Recommendation
        ↓
Actual Intake Calculation
```
---
# 🧠 Development Process
## Stage 1 — Simple Nutrition Website
Initial Goal:
- Display milk nutrition data
- Create comparison tables
- Explain health information
Problem:
- Similar information already existed online
- Lack of uniqueness
---
## Stage 2 — Recommendation System
We introduced:
- low sugar preferences
- high protein preferences
- lactose-free filtering
- price importance
A weighted scoring system was added.
This transformed the project into:
> a personalized recommendation system.
---
## Stage 3 — Barcode Scanner
We added:
- barcode scanning,
- Open Food Facts API integration,
- automatic product lookup.
This improved accessibility and usability.
---
## Stage 4 — Nutrition Standardization
We discovered another important issue:
Different products used different serving sizes.
For example:
```text
Product A → 200mL standard
Product B → 100mL standard
```
Direct comparison was misleading.
To solve this, we standardized all nutrition values into:
> per 100mL values.
This became one of the most important technical aspects of the project.
---
## Stage 5 — Actual Intake Calculation
Most nutrition labels only show:
- fixed serving sizes,
- not real consumption amounts.
Our application allows users to:
- enter their actual intake amount,
- and automatically calculate:
  - calories,
  - sugar,
  - protein,
  - calcium intake.
---
# 🔄 Project Growth
```text
Simple Website
      ↓
Nutrition Comparison
      ↓
Preference-Based Recommendation
      ↓
Barcode Scanner
      ↓
API Integration
      ↓
100mL Standardization
      ↓
Actual Intake Calculation
```
---
# 🧬 Biology Contributions
The biology-related aspects include:
## Nutritional Analysis
- sugar intake
- protein comparison
- calcium analysis
## Health Considerations
- lactose intolerance
- low-fat / non-fat milk
- high protein products
## Dietary Interpretation
Helping users understand:
- healthier choices,
- nutritional differences,
- and dietary suitability.
---
# 💻 Computer Science Contributions
## Recommendation Algorithm
- weighted scoring system
- Boolean preference filtering
- ranking system
## Database Design
- structured milk database
- nutrition organization
- standardized values
## API Integration
- Open Food Facts API
- real-time nutrition retrieval
## Barcode System
- barcode detection
- camera-based interaction
## Data Normalization
- automatic 100mL conversion
- fair comparison system
---
# ⚙️ Core Features
## ✅ Personalized Recommendation
Users can select:
- low sugar
- high protein
- lactose free
- low fat
- price importance
The application calculates recommendation scores automatically.
---
## ✅ Barcode Scanner
Users can scan products directly using their camera.
The system retrieves nutrition information automatically.
---
## ✅ 100mL Standardization
Nutrition values are automatically converted into:
> standardized 100mL-based values.
This enables fair product comparison.
---
## ✅ Actual Intake Calculator
Users can input:
```text
“How much will I actually drink?”
```
The system calculates real nutritional intake automatically.
---
## ✅ Product Comparison
Users can compare:
- calories
- sugar
- protein
- calcium
- price
between multiple products.
---
# 🗂️ Mind Map
```text
Milk Recommendation System
│├── Nutrition Database
│   ├── Calories
│   ├── Sugar
│   ├── Protein
│   ├── Calcium
│   └── Price
│├── Personalized Recommendation
│   ├── Low Sugar
│   ├── High Protein
│   ├── Lactose Free
│   ├── Low Fat
│   └── Price Importance
│├── Barcode System
│   ├── Camera Input
│   ├── Barcode Detection
│   └── API Integration
│├── Nutrition Standardization
│   ├── 100mL Conversion
│   └── Fair Comparison
│└── Actual Intake Calculation
    ├── Intake Input
    ├── Real Sugar Intake
    ├── Real Protein Intake
    └── Real Calorie Intake
```
---
# 👥 Role Distribution
## Biology Team
- nutrition research
- health analysis
- lactose intolerance research
- dietary interpretation
## Computer Science Team
- recommendation algorithm
- database organization
- barcode scanner implementation
- API integration
- web application development
---
# ⚠️ Limitations
Current limitations include:
```text
• Limited milk database
• Dependency on external APIs
• Rule-based recommendation system
• OCR nutrition recognition not implemented yet
• Limited mobile optimization
```
---
# 🚀 Future Development
Possible future improvements:
- OCR nutrition label recognition
- expansion to other food categories
- AI-based recommendation systems
- mobile application development
- health profile integration
- machine learning recommendation models
---
# 🛠️ Technologies Used
- HTML
- CSS
- JavaScript
- Open Food Facts API
- Netlify
- GitHub
- Google Spreadsheet
---
# 📌 Conclusion
This project began as a simple milk information website but gradually evolved into:
> a personalized nutrition recommendation system.
The project combines:
- Biology,
- Computer Science,
- nutrition analysis,
- recommendation algorithms,
- and data standardization.
More importantly, the project taught us:
- iterative problem solving,
- interdisciplinary collaboration,
- and user-centered design thinking.
