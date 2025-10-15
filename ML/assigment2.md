## KNN
1. **Store** all training data with labels.
2. **Choose** the number of neighbors \(k\).
3. **For a new input**:
   - Compute distance to all training points.
   - Sort distances and pick \(k\) nearest.
   - Count labels among the \(k\) neighbors.
   - Assign the most frequent label to the input.

<img width="901" height="425" alt="image" src="https://github.com/user-attachments/assets/bd19e54e-b87b-45bb-9e45-9350186abb04" />

<img width="877" height="418" alt="image" src="https://github.com/user-attachments/assets/27f2ceda-da78-43c4-8961-cdcb31376bb4" />

<img width="892" height="394" alt="image" src="https://github.com/user-attachments/assets/fe3199fa-dee0-41fa-b57a-bd21a8e33b96" />

<img width="886" height="428" alt="image" src="https://github.com/user-attachments/assets/4c42b45b-c5f2-4fd5-bf1b-98300b446e35" />


## LR
- Collect Data: Gather input features X and target values y.
- Initialize Parameters: Set initial weights w and bias b (often to 0).
1. Initialize weight (w) and bias (b) to 0
2. Repeat until convergence:
   a. Predict: y_hat = w * x + b
   b. Compute Loss: MSE = (1/n) * Σ(y_hat - y)^2
   c. Compute Gradients:
      dw = (2/n) * Σx * (y_hat - y)
      db = (2/n) * Σ(y_hat - y)
   d. Update Parameters:
      w = w - learning_rate * dw
      b = b - learning_rate * db
3. Use final w and b to make predictions
- Repeat: Iterate steps 3–5 until convergence.
- Predict: Use final w and b to predict new values
Linear Regression Algorithm (Gradient Descent)


---

### 1️⃣ Predict House Prices  
**Dataset**:

| Size (sq ft) | Price ($1000s) |
|--------------|----------------|
| 600          | 150            |
| 800          | 200            |
| 1000         | 250            |
| 1200         | 300            |

**Question**:  
Predict the price of a 1100 sq ft house.

---

### 2️⃣ Estimate Student Scores  
**Dataset**:

| Study Hours | Exam Score (%) |
|-------------|----------------|
| 1           | 50             |
| 2           | 55             |
| 3           | 65             |
| 4           | 70             |

**Question**:  
Predict the exam score for a student who studies 2.5 hours.

---

### 3️⃣ Forecast Sales Based on Ads  
**Dataset**:

| Ad Spend ($1000s) | Sales (units) |
|-------------------|---------------|
| 1                 | 100           |
| 2                 | 180           |
| 3                 | 260           |
| 4                 | 340           |

**Question**:  
Estimate sales if $2.5k is spent on advertising.

---

### 4️⃣ Predict Temperature from Altitude  
**Dataset**:

| Altitude (meters) | Temperature (°C) |
|-------------------|------------------|
| 0                 | 30               |
| 500               | 27               |
| 1000              | 24               |
| 1500              | 21               |

**Question**:  
Predict the temperature at 750 meters altitude.

## multi LR


---

### 1️⃣ Predict House Price  
**Dataset**:

| Size (sq ft) | Bedrooms | Price ($1000s) |
|--------------|----------|----------------|
| 1000         | 2        | 200            |
| 1500         | 3        | 300            |
| 2000         | 4        | 400            |
| 2500         | 4        | 450            |

**Question**:  
Predict the price of a house with 1800 sq ft and 3 bedrooms.

---

### 2️⃣ Estimate Student Exam Score  
**Dataset**:

| Study Hours | Sleep Hours | Exam Score (%) |
|-------------|-------------|----------------|
| 2           | 6           | 55             |
| 3           | 7           | 65             |
| 4           | 6           | 70             |
| 5           | 8           | 80             |

**Question**:  
Predict the exam score for a student who studied 3.5 hours and slept 7 hours.

---

### 3️⃣ Predict Car Fuel Efficiency  
**Dataset**:

| Engine Size (L) | Weight (kg) | MPG |
|------------------|-------------|-----|
| 1.2              | 1000        | 40  |
| 1.6              | 1200        | 35  |
| 2.0              | 1400        | 30  |
| 2.4              | 1600        | 25  |

**Question**:  
Estimate MPG for a car with a 1.8L engine and 1300 kg weight.

---

### 4️⃣ Forecast Sales Based on Ads  
**Dataset**:

| TV Ads ($1000s) | Online Ads ($1000s) | Sales (units) |
|------------------|---------------------|----------------|
| 2                | 1                   | 150            |
| 3                | 2                   | 220            |
| 4                | 3                   | 290            |
| 5                | 4                   | 360            |

**Question**:  
Predict sales if $3.5k is spent on TV ads and $2.5k on online ads.

## Logistic regression


---

### 🔁 Logistic Regression Algorithm (Simplified)

1. **Prepare Data**  
   - Collect input features and binary labels (0 or 1).

2. **Initialize Parameters**  
   - Set initial weights and bias (usually to zero).

3. **Define Sigmoid Function**  
   - `sigmoid(z)` returns a value between 0 and 1, used to convert raw predictions into probabilities.

4. **Make Predictions**  
   - For each input, compute `z = dot_product(weights, features) + bias`.  
   - Apply `sigmoid(z)` to get predicted probability.

5. **Calculate Loss**  
   - Use a loss function like binary cross-entropy to measure prediction error.

6. **Compute Gradients**  
   - Find how much each weight and bias contributes to the error.

7. **Update Parameters**  
   - Adjust weights and bias using gradient descent:
     - `weights = weights - learning_rate * gradient_weights`
     - `bias = bias - learning_rate * gradient_bias`

8. **Repeat Steps 4–7**  
   - Loop for a fixed number of iterations or until the loss is small.

9. **Classify Output**  
   - If predicted probability ≥ 0.5, classify as 1; else classify as 0.

---

### 1️⃣ Predict if a Student Passes  
**Dataset**:

| Study Hours | Passed (1=yes, 0=no) |
|-------------|----------------------|
| 1           | 0                    |
| 2           | 0                    |
| 3           | 1                    |
| 4           | 1                    |

**Question**:  
Predict whether a student who studies for 2.5 hours will pass.

---

### 2️⃣ Classify Email as Spam  
**Dataset**:

| Word Count | Link Count | Spam (1=yes, 0=no) |
|------------|------------|--------------------|
| 50         | 0          | 0                  |
| 100        | 2          | 1                  |
| 80         | 1          | 1                  |
| 30         | 0          | 0                  |

**Question**:  
Predict if an email with 70 words and 1 link is spam.

---

### 3️⃣ Predict Loan Approval  
**Dataset**:

| Income ($1000s) | Credit Score | Approved (1=yes, 0=no) |
|-----------------|--------------|-------------------------|
| 30              | 600          | 0                       |
| 50              | 700          | 1                       |
| 40              | 650          | 0                       |
| 60              | 720          | 1                       |

**Question**:  
Will a person with $45k income and 680 credit score be approved?

---

### 4️⃣ Predict Disease Presence  
**Dataset**:

| Age | Blood Pressure | Has Disease (1=yes, 0=no) |
|-----|----------------|---------------------------|
| 25  | 120            | 0                         |
| 45  | 140            | 1                         |
| 35  | 130            | 0                         |
| 50  | 150            | 1                         |

**Question**:  
Predict if a 40-year-old with 135 blood pressure has the disease.

---
## SVM

---

### ⚙️ SVM Algorithm (Step-by-Step, No Equations)

1. **Prepare Data**  
   - Collect input features and class labels (e.g., 0 or 1).

2. **Choose Kernel Function**  
   - Select a kernel like:
     - `linear_kernel(x1, x2)`
     - `polynomial_kernel(x1, x2)`
     - `rbf_kernel(x1, x2)` (Radial Basis Function)

3. **Initialize Model Parameters**  
   - Set initial values for weights, bias, and regularization settings.

4. **Compute Decision Boundary**  
   - Use the chosen kernel to transform data if needed.
   - Find the best boundary that separates classes with maximum margin.

5. **Identify Support Vectors**  
   - Select data points closest to the boundary — these influence the final model.

6. **Train Model**  
   - Use optimization to adjust weights and bias so that:
     - Most points are correctly classified.
     - Margin between classes is maximized.
     - Misclassifications are minimized (if allowed).

7. **Make Predictions**  
   - For a new input, compute the decision score using the kernel.
   - If score ≥ 0, predict class 1; else predict class 0.

8. **Evaluate Accuracy**  
   - Test on validation data and measure performance (e.g., accuracy, precision).

---


---

### 1️⃣ Classify Fruit Type  
**Dataset**:

| Weight (g) | Color Score (0–1) | Fruit (1=Apple, 0=Orange) |
|------------|-------------------|----------------------------|
| 150        | 0.8               | 1                          |
| 130        | 0.7               | 1                          |
| 170        | 0.3               | 0                          |
| 160        | 0.2               | 0                          |

**Question**:  
Use SVM to classify a fruit weighing 140g with a color score of 0.6.

---

### 2️⃣ Predict if a Person Buys a Product  
**Dataset**:

| Age | Salary ($1000s) | Bought (1=yes, 0=no) |
|-----|------------------|----------------------|
| 25  | 40               | 0                    |
| 30  | 60               | 1                    |
| 35  | 80               | 1                    |
| 40  | 50               | 0                    |

**Question**:  
Will a 32-year-old earning $70k buy the product?

---

### 3️⃣ Classify Email Type  
**Dataset**:

| Word Count | Exclamation Marks | Type (1=Spam, 0=Normal) |
|------------|-------------------|--------------------------|
| 100        | 5                 | 1                        |
| 80         | 0                 | 0                        |
| 120        | 3                 | 1                        |
| 90         | 1                 | 0                        |

**Question**:  
Classify an email with 110 words and 2 exclamation marks.

---

### 4️⃣ Predict Loan Default  
**Dataset**:

| Credit Score | Debt ($1000s) | Defaulted (1=yes, 0=no) |
|--------------|----------------|--------------------------|
| 600          | 20             | 1                        |
| 700          | 10             | 0                        |
| 650          | 15             | 1                        |
| 720          | 5              | 0                        |

**Question**:  
Will someone with a credit score of 680 and $12k debt default?

---

## decision tree

---

### 🌳 Decision Tree Algorithm (Simplified)

1. **Prepare Data**  
   - Collect input features and target labels.

2. **Check for Stopping Conditions**  
   - If all labels are the same → return that label.  
   - If no features left → return majority label.

3. **Select Best Feature to Split**  
   - Use a function like `choose_best_split(data)` to find the feature that best separates the classes.

4. **Split Data**  
   - Divide the dataset into subsets based on the selected feature’s values.

5. **Build Subtrees**  
   - Recursively apply steps 2–4 to each subset.

6. **Create Decision Node**  
   - Store the chosen feature and link it to its subtrees.

7. **Predict**  
   - For a new input, follow the tree from root to leaf based on feature values.

---


---

### 1️⃣ Predict Weather Activity  
**Dataset**:

| Outlook | Temperature | Play (1=Yes, 0=No) |
|---------|-------------|--------------------|
| Sunny   | Hot         | 0                  |
| Overcast| Mild        | 1                  |
| Rainy   | Cool        | 1                  |
| Sunny   | Mild        | 1                  |

**Question**:  
Should you play outside if the outlook is Rainy and temperature is Hot?

---

### 2️⃣ Classify Animal Type  
**Dataset**:

| Has Fur | Lays Eggs | Animal (1=Mammal, 0=Reptile) |
|---------|-----------|------------------------------|
| Yes     | No        | 1                            |
| No      | Yes       | 0                            |
| Yes     | Yes       | 0                            |
| No      | No        | 1                            |

**Question**:  
Is an animal with fur that lays eggs a mammal or reptile?

---

### 3️⃣ Predict Loan Approval  
**Dataset**:

| Income Level | Credit History | Approved (1=Yes, 0=No) |
|--------------|----------------|------------------------|
| High         | Good           | 1                      |
| Low          | Bad            | 0                      |
| Medium       | Good           | 1                      |
| Low          | Good           | 0                      |

**Question**:  
Will someone with Medium income and Bad credit history be approved?

---

### 4️⃣ Classify Fruit Type  
**Dataset**:

| Color | Size | Fruit (1=Apple, 0=Banana) |
|-------|------|---------------------------|
| Red   | Small| 1                         |
| Yellow| Large| 0                         |
| Green | Small| 1                         |
| Yellow| Small| 0                         |

**Question**:  
Is a green, large fruit more likely an apple or banana?

---
# Naive Bais

- Look at past examples
Count how many times each category appears (like spam vs not spam).
- Track feature patterns
For each feature (like a word or symptom), count how often it shows up with each category.
- Save what you learned
Store these counts so you can use them to make future guesses.
- Make a guess for new input
For each category, start with its overall count. Then, for each feature in the new input, check how often it matched that category before.
- Pick the best match
Choose the category with the highest combined score.

---

### 1️⃣ Email Spam Detection  
**Dataset:**

| Email Text         | Label     |
|--------------------|-----------|
| Win money now!     | Spam      |
| Meeting at 3pm     | Not Spam  |
| Free vacation      | Spam      |
| Project update     | Not Spam  |

**Question:**  
Predict whether the email **"Free money offer"** is spam or not.

---

### 2️⃣ Weather Prediction  
**Dataset:**

| Outlook   | Temperature | Play Tennis |
|-----------|-------------|-------------|
| Sunny     | Hot         | No          |
| Overcast  | Mild        | Yes         |
| Rainy     | Cool        | Yes         |
| Sunny     | Mild        | Yes         |

**Question:**  
Will someone play tennis if the outlook is **Sunny** and temperature is **Cool**?

---

### 3️⃣ Customer Purchase Behavior  
**Dataset:**

| Age Group | Browsing Time | Bought Product |
|-----------|----------------|----------------|
| Young     | Long           | Yes            |
| Senior    | Short          | No             |
| Middle    | Medium         | Yes            |
| Young     | Short          | No             |

**Question:**  
Predict if a **Middle-aged** customer with **Long** browsing time will buy the product.

---

### 4️⃣ Disease Diagnosis  
**Dataset:**

| Symptom A | Symptom B | Has Disease |
|-----------|-----------|-------------|
| Yes       | No        | Yes         |
| No        | Yes       | No          |
| Yes       | Yes       | Yes         |
| No        | No        | No          |

**Question:**  
Predict if someone with **Symptom A = Yes** and **Symptom B = Yes** has the disease.

---

## random forest
🌲 Random Forest Algorithm (Minimal Steps)
- Pick random samples
Select multiple random subsets from the training data.
- Build decision trees
Train a separate decision tree on each subset.
- Make predictions
Each tree gives its own prediction for new input.
- Vote
Combine all tree predictions and choose the majority result.


---

### 1️⃣ Loan Approval  
**Dataset:**

| Income Level | Credit Score | Approved |
|--------------|--------------|----------|
| High         | Good         | Yes      |
| Low          | Poor         | No       |
| Medium       | Good         | Yes      |
| Low          | Good         | No       |

**Question:**  
Will a person with **Medium income** and **Poor credit score** be approved?

---

### 2️⃣ Disease Diagnosis  
**Dataset:**

| Fever | Cough | Has Disease |
|-------|-------|-------------|
| Yes   | Yes   | Yes         |
| No    | Yes   | No          |
| Yes   | No    | Yes         |
| No    | No    | No          |

**Question:**  
Predict if someone with **Fever = Yes** and **Cough = No** has the disease.

---

### 3️⃣ Student Performance  
**Dataset:**

| Study Hours | Attendance | Passed |
|-------------|------------|--------|
| High        | Good       | Yes    |
| Low         | Poor       | No     |
| Medium      | Good       | Yes    |
| Low         | Good       | No     |

**Question:**  
Will a student with **Medium study hours** and **Poor attendance** pass?

---

### 4️⃣ Product Recommendation  
**Dataset:**

| Age Group | Browsing Time | Bought Product |
|-----------|----------------|----------------|
| Young     | Long           | Yes            |
| Senior    | Short          | No             |
| Middle    | Medium         | Yes            |
| Young     | Short          | No             |

**Question:**  
Will a **Senior** with **Long browsing time** buy the product?

---

