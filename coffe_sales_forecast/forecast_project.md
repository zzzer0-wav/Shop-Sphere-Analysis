# **☕ Sales Forecasting with Python**

**A Simple Machine Learning Task (scikit-learn)**

Data link: [coffee_sales](https://docs.google.com/spreadsheets/d/1MQfxhhAQPYu4pFdQ70XJbdkf047AAXwk__U9hSL68NQ/edit?usp=sharing)

Colab link: [coffee_forecast.ipynb](https://colab.research.google.com/drive/1juwcB-bVkM_t-utRyOfkyWNVGBzxeQIl?usp=sharing)

# **What this assignment is about**

In this project, you will train your first machine learning model — one that predicts the future sales of a coffee shop based on historical data. You will use the **scikit-learn** library, the most popular ML tool in Python.

**You do not need to be a programmer.** Almost all of the code has already been written. You only need to run the cells one by one and fill in 2–3 small blanks. The main goal of this assignment is **not the code, but the ability to explain the result in simple words**, just like a real analyst would do when presenting to management.

*💡 The model you will build is called **linear regression**. It is the simplest type of forecasting: the model draws a straight line through your data and extends it into the future. Simple, but very useful for understanding the basics.*

# **Scenario**

You are an analyst for the **"CoffeeTime"** coffee shop chain. You have data on monthly revenue for 3 years (2022–2024) — 36 months. The director is preparing the budget for next year and asks you: *"How much revenue will we generate in the first half of 2025?"* Your task is to build a forecast and, most importantly, honestly explain to the director how much this forecast can be trusted.

# **Files**

* **coffee_forecast.ipynb** — the notebook with the assignment (open it in Google Colab)

* **coffee_sales.csv** — the revenue data (place it in the same folder as the notebook)

# **How to complete the assignment**

1. Open **coffee_forecast.ipynb** and read the explanation for each step.

2. Run the cells one by one, from top to bottom (Shift + Enter).

3. Wherever you see **# ⬅️ YOUR CODE**, fill in the blank (it's literally one line).

4. Answer the **interpretation questions** (4 + bonus) — this is the most important part. Write your answers directly in the notebook.

# **What you will do (8 steps)**

* Step 1–2: Import the libraries and load the data.

* Step 3: Build a chart and examine the data visually.

* Step 4–5: Prepare the data and train the model (the main blank here is the `.fit()` call).

* Step 6: Check how well the model describes the historical data.

* Step 7: 🔮 Build a forecast for the next 6 months.

* Step 8: ⭐ Bonus — make a forecast for a specific month.

# **The most important part: interpretation questions**

The notebook contains 4 required questions (plus a bonus). They are the heart of the assignment. Here's what they are about, so you know what to pay attention to:

*🧠 Question 1 — Reading the chart: What is the direction of the trend? Are there any seasonal fluctuations?*

*🧠 Question 2 — The meaning of the "slope": What does the slope value mean for the director in simple words (by how many UAH the revenue increases each month)?*

*🧠 Question 3 — Why don't the points lie perfectly on the line, and is a simple straight line sufficient?*

*🧠 Question 4 (the most important) — Can the forecast be trusted? What are its limitations, and why is extending a straight line "to infinity" dangerous for a business?*

*💡 There is no single "correct" answer to the interpretation questions. We evaluate whether you understand what the model does and whether you recognize its limitations. An honest "The forecast cannot be fully trusted because..." is more valuable than a naive "The model predicted 31,539 UAH, so that's exactly what will happen."*

# **What to submit**

* The completed **coffee_forecast.ipynb** notebook with all cells executed (so the charts are visible) (Google Colab link)

* Answers to all 4 questions + the bonus, written directly in the notebook.

*💡 Before submitting, make sure the notebook runs from top to bottom without errors. The charts should be displayed.*

# **Grading Criteria**

| Criterion | Points |
| :---- | :---- |
| The code works (all blanks are completed, the notebook runs successfully) | **30** |
| Questions 1–2: Reading the chart and understanding the "slope" | **20** |
| Question 3: Understanding why the points deviate from the line | **15** |
| Question 4: Understanding the limitations of the forecast (the most important) | **30** |
| Bonus: Forecast for a specific month + reasoning | **5** |

*Good luck! Remember: an analyst who understands the limitations of a model is more valuable than one who simply knows how to press a button. ☕📈*
