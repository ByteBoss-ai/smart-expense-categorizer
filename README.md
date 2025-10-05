# Smart Expense Categorizer (ML-based)

## Overview
The **Smart Expense Categorizer** is a machine learning project that automatically classifies financial transactions into predefined categories such as **Food**, **Travel**, **Groceries**, **Shopping**, **Utilities**, and **Entertainment**. This helps users track spending, generate insights, and organize expenses efficiently.

The project uses **TF-IDF vectorization** for text features and **Logistic Regression** for classification.

---

## Features
- Automatically categorizes transaction texts into multiple expense categories.
- Cleans and preprocesses transaction text by removing unnecessary words and numbers.
- Uses TF-IDF to extract meaningful textual features.
- Provides **accuracy metrics** and **classification reports**.
- Easy to test with new transaction examples.

---

## Dataset
- Synthetic dataset generated for common merchants under each category.
- Each transaction text follows the format:
"TXN SUCCESSFUL FOR <amount> AT <merchant> VIA DEBIT CARD XXXX"


- Example transactions:
  - `TXN SUCCESSFUL FOR 450 AT PIZZA HUT VIA DEBIT CARD XXXX` → Food
  - `TXN SUCCESSFUL FOR 2500 AT FLIPKART VIA DEBIT CARD XXXX` → Shopping

- Categories:
  - **Food**: SWIGGY, ZOMATO, DOMINOS, STARBUCKS, etc.
  - **Travel**: UBER, OLA, METRO CARD RECHARGE, FLIGHT TICKET, etc.
  - **Groceries**: BIGBASKET, GROFER, SUPERMARKET, etc.
  - **Shopping**: AMAZON, FLIPKART, MYNTRA, etc.
  - **Utilities**: ELECTRICITY BILL, MOBILE RECHARGE, WATER SUPPLY, etc.
  - **Entertainment**: NETFLIX, PVR CINEMAS, SPOTIFY, etc.

---

## Technology Stack
- **Language**: Python 3
- **Libraries**:
  - `pandas`, `numpy` → Data handling
  - `scikit-learn` → Machine learning
  - `re` → Text cleaning
  - `random` → Synthetic data generation

---

## Installation
Clone the repository:
   ```bash
   git clone <repository_url>
   cd smart-expense-categorizer




