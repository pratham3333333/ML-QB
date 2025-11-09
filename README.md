# 🧩 Machine Learning Assignment — Unit 1 Detailed Answer Key (7-Mark Answers)

This section includes **detailed 7-mark answers** for all Unit 1 questions, written in **simple, clear, and structured format** with **real-life examples**.

---

## 🔹 Q1. Define machine learning. List the differences between classification and regression. What is the bias-variance trade-off?

### **Definition:**

Machine Learning (ML) is a branch of Artificial Intelligence (AI) that enables systems to **learn from data**, identify patterns, and make decisions with minimal human intervention.

### **Key Concept:**

Instead of being programmed with fixed rules, ML algorithms improve automatically through **experience**.

### **Classification vs Regression:**

| Type               | Output                  | Example                        | Purpose                           |
| ------------------ | ----------------------- | ------------------------------ | --------------------------------- |
| **Classification** | Predicts a **category** | Spam / Not Spam                | Decision-making (discrete output) |
| **Regression**     | Predicts a **number**   | Predicting salary, temperature | Forecasting (continuous output)   |

### **Bias–Variance Trade-off:**

* **Bias:** Error due to overly simple models → ignores important relationships (Underfitting).
* **Variance:** Error due to overly complex models → memorizes noise in training data (Overfitting).
* The goal is to **find a balance** so that the model performs well on both training and unseen data.

### **Example:**

Predicting house prices:

* Linear regression (too simple) → high bias.
* Deep neural network (too complex, small data) → high variance.
* A medium-depth tree → balanced trade-off.

### **Conclusion:**

A good ML model maintains a **balance between bias and variance**, ensuring both accuracy and generalization.

---

## 🔹 Q2. Apply the concepts of reinforcement learning to a simple game environment. Demonstrate the use of causal inference in a healthcare prediction scenario.

### **Reinforcement Learning (RL):**

RL is a learning method where an **agent interacts with an environment**, takes actions, and learns from **rewards or penalties**.

### **Key Elements:**

* **Agent:** Learner or decision-maker (e.g., robot or game player)
* **Environment:** The world the agent interacts with
* **Action:** Choices made by the agent
* **Reward:** Feedback after each action

### **Example — Simple Game:**

In a maze game, the agent gets:

* +10 points for reaching the goal
* -5 points for hitting a wall
  Over time, the agent learns the best path through trial and error.

### **Causal Inference in Healthcare:**

Causal inference identifies **what causes what**, not just correlations.

**Example:**

* Doctors want to know if a new drug **causes** recovery from fever.
* The system compares two groups (treated vs untreated) while keeping other factors constant.
* This helps identify the real **cause** behind improvement.

### **Conclusion:**

Reinforcement learning teaches through feedback, while causal inference ensures decisions are based on **true cause-effect relationships** — crucial in healthcare, games, and business optimization.

---

## 🔹 Q3. Analyse the role of expectation in deriving the mean and variance of a probability distribution.

### **Expectation (Mean):**

It is the **average value** a random variable takes, considering probabilities.
Formula:
[ E(X) = \sum x \cdot P(x) ]

### **Variance:**

It measures how much values **deviate from the mean**.
Formula:
[ Var(X) = E[(X - E(X))^2] ]

### **Role of Expectation:**

* Expectation is used in both mean and variance.
* It represents the **expected outcome** of random processes.

### **Example:**

For a fair dice (1 to 6):

* Mean (E[X]) = (1+2+3+4+5+6)/6 = 3.5
* Variance = E[X²] - (E[X])² = (91/6) - (3.5)² ≈ 2.92

### **Interpretation:**

* Higher variance → values are more spread out.
* Lower variance → values are close to mean.

### **Conclusion:**

Expectation acts as a foundation for measuring both central tendency (mean) and variability (variance), essential for understanding randomness in ML models.

---

## 🔹 Q4. Evaluate the significance of information theory in feature selection for machine learning.

### **Definition:**

Information theory measures **how much useful information** a feature provides about the target variable.

### **Key Concepts:**

* **Entropy:** Measures uncertainty or randomness in data.

  * Formula:  ( H(X) = - \sum P(x) \log P(x) )
* **Information Gain (IG):** Reduction in uncertainty when a feature is used.

  * Formula:  ( IG(Y, X) = H(Y) - H(Y|X) )

### **Significance in ML:**

* Helps **choose the most informative features**.
* Removes **irrelevant or redundant** features.
* Improves model accuracy and reduces overfitting.

### **Example:**

In spam detection:

* Feature “Free” → high information gain (useful)
* Feature “Hello” → low information gain (less useful)

### **Conclusion:**

Information theory ensures the model focuses on the most **useful and meaningful features**, improving both accuracy and efficiency.

---

## 🔹 Q5. Apply the concept of simple models versus complex models to a given dataset. Explain which model is more suitable.

### **Simple Models:**

* Examples: Linear Regression, Decision Tree (small depth)
* **Advantages:** Easy to interpret, less training time.
* **Disadvantages:** May miss nonlinear relationships (Underfitting).

### **Complex Models:**

* Examples: Random Forest, Neural Networks
* **Advantages:** Capture complex patterns, high accuracy on large data.
* **Disadvantages:** Require more data and computing power, less explainable.

### **Example:**

Predicting house prices:

* **Small dataset:** Use Linear Regression.
* **Large dataset with images or many variables:** Use Neural Network.

### **Model Suitability:**

* Depends on dataset size, complexity, and interpretability needs.

### **Conclusion:**

Choose the model that balances **accuracy, simplicity, and interpretability** based on the problem type and data characteristics.

---

## 🔹 Q6. What is reinforcement learning? Define causal inference in machine learning.

### **Reinforcement Learning:**

A method where an **agent learns from interaction** with its environment using rewards and penalties.

**Components:**

* **Agent:** Learner
* **Environment:** The surrounding setup
* **Reward Signal:** Feedback
* **Policy:** Strategy to choose next action

**Example:** A self-driving car learns to drive by getting rewards for staying on the road and penalties for crashing.

### **Causal Inference:**

A process to determine **cause-and-effect** relationships rather than mere associations.

**Example:** Checking whether diet *causes* weight loss, not just correlates with it.

### **Importance in ML:**

* RL helps in **sequential decision-making**.
* Causal inference helps in **fair, reliable, and ethical decisions**.

### **Conclusion:**

Together, RL and causal inference enhance **learning, reasoning, and fairness**, enabling ML systems to make smarter, cause-based decisions.

---

✅ **End of Unit 1 (7-Mark Detailed Answer Key)**
