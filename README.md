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

# 🤖 Machine Learning Assignment — Unit 2 Answer Key (7-Mark Detailed Answers)

This file contains **detailed 7-mark answers** for Unit 2 of the Machine Learning assignment. Each answer includes clear explanations, structured points, and real-world examples.

---

## 🔹 Q13. Design a classification model using decision trees for predicting customer churn in a telecommunications dataset. Explain your approach.

**Answer:**

* **Definition:** A Decision Tree is a supervised learning algorithm used for classification and regression. It splits data into branches based on conditions.
* **Goal:** Predict if a customer will leave (churn) or stay.

### **Steps:**

1. **Data Collection:** Use customer data like age, usage, plan type, complaints, etc.
2. **Data Preprocessing:** Handle missing values and convert categorical data (e.g., gender → numeric).
3. **Feature Selection:** Choose features like call duration, bill amount, and contract type.
4. **Model Building:** Use the Decision Tree algorithm (e.g., ID3, C4.5, or CART).
5. **Training:** The tree splits based on **information gain** or **Gini index**.
6. **Prediction:** For a new customer, the model predicts churn based on conditions.

📘 **Example:**
If a user has a short contract, low call usage, and high complaints → model predicts **“Churn = Yes.”**

✅ **Conclusion:** Decision Trees are interpretable and effective for customer churn prediction but may overfit if the tree is too deep.

---

## 🔹 Q14. Define feature extraction in machine learning. List common methods of linear dimension reduction.

**Answer:**

* **Feature Extraction:** It’s the process of transforming raw data into meaningful features that improve model performance.
* It helps reduce **dimensionality**, remove redundancy, and increase **efficiency**.

### **Linear Dimension Reduction Methods:**

1. **Principal Component Analysis (PCA):** Converts correlated variables into uncorrelated principal components.
2. **Linear Discriminant Analysis (LDA):** Maximizes separation between multiple classes.
3. **Singular Value Decomposition (SVD):** Decomposes data matrix into smaller components.

📘 **Example:**
In an image dataset with 1000 features (pixels), PCA can reduce it to 100 main components without losing major information.

✅ **Conclusion:** Linear methods help simplify data while maintaining its structure, improving model speed and accuracy.

---

## 🔹 Q15. Explain the concept of neural networks in nonlinear dimension reduction. Describe the significance of eigenvalues in PCA.

**Answer:**

* **Neural Networks for Nonlinear Reduction:**

  * Neural networks (like **Autoencoders**) can learn complex, nonlinear mappings of data.
  * They compress input data into a smaller hidden layer and reconstruct it — learning efficient feature representations.

📘 **Example:** In face recognition, an autoencoder learns unique facial patterns (eyes, nose) in reduced dimensions.

* **Eigenvalues in PCA:**

  * Represent the **amount of variance** captured by each principal component.
  * Larger eigenvalues → more important components.

✅ **Conclusion:** Neural networks handle complex data patterns, while eigenvalues in PCA help select top features for accurate analysis.

---

## 🔹 Q16. Compare linear and nonlinear dimension reduction techniques in feature extraction.

**Answer:**

| Aspect               | Linear Techniques                  | Nonlinear Techniques                  |
| -------------------- | ---------------------------------- | ------------------------------------- |
| **Nature**           | Assume straight-line relationships | Capture complex, curved relationships |
| **Examples**         | PCA, LDA                           | t-SNE, Autoencoders                   |
| **Speed**            | Faster, simpler                    | Slower, computationally heavy         |
| **Interpretability** | Easy to explain                    | Harder to interpret                   |
| **Use Case**         | Tabular data                       | Image, speech, nonlinear data         |

📘 **Example:**

* PCA (linear) works for simple data like student marks.
* t-SNE (nonlinear) works for visualizing image clusters.

✅ **Conclusion:** Choice depends on data structure — linear for simple relations, nonlinear for complex patterns.

---

## 🔹 Q17. Explain how decision-based methods are applied in classification. Describe the key differences between instance-based learning and decision-based methods.

**Answer:**

* **Decision-Based Methods:**

  * Use a set of rules or tree structures to make predictions.
  * Learn decision boundaries from training data.
  * Example algorithms: Decision Trees, Random Forests.

📘 **Example:** In medical diagnosis, a Decision Tree can predict “Disease or No Disease” based on patient symptoms.

### **Instance-Based Learning:**

* Uses existing data points directly for predictions.
* No explicit model; relies on similarity (e.g., K-Nearest Neighbours).

### **Key Differences:**

| Feature      | Decision-Based        | Instance-Based                  |
| ------------ | --------------------- | ------------------------------- |
| **Approach** | Learns explicit rules | Stores and compares data points |
| **Speed**    | Faster at prediction  | Slower at prediction            |
| **Examples** | Decision Tree, SVM    | KNN                             |

✅ **Conclusion:** Decision-based models generalize patterns; instance-based models memorize and compare examples.

---

## 🔹 Q18. Apply PCA on a dataset to reduce its dimensionality. Show the steps involved.

**Answer:**
**Principal Component Analysis (PCA)** is used to reduce the number of features while keeping most of the information.

### **Steps in PCA:**

1. **Standardize the Data:** Mean = 0, Variance = 1.
2. **Compute Covariance Matrix:** Shows relationships between variables.
3. **Find Eigenvalues & Eigenvectors:** Identify principal components.
4. **Select Top Components:** Choose components with highest eigenvalues.
5. **Transform Data:** Multiply original data with selected eigenvectors.

📘 **Example:**
Dataset with 4 features (height, weight, age, income) → PCA reduces it to 2 components capturing 90% of variance.

✅ **Conclusion:** PCA reduces complexity, helps visualization, and improves computational efficiency without losing major data insights.

---

✅ **End of Unit 2 Answer Key** — All answers are structured for **7 marks**, include examples, and are written in **simple, easy-to-understand language**.


# 🧠 Machine Learning Assignment — Unit 3 Answer Key (7-Mark Detailed Answers)

This section provides **Unit 3 answers** written in simple, easy-to-understand language with detailed explanations and real-world examples. Each answer is designed for **7 marks**.

---

## 🔹 Q25. Explain how neural networks can be used as discriminative models. Describe the key differences between discriminative models and generative models.

**Answer:**

* **Neural Networks as Discriminative Models:**

  * Neural networks learn to **classify** input data by modeling the boundary between classes.
  * They estimate **P(y | x)** — the probability of class *y* given input *x*.
  * Used in classification problems like image or speech recognition.

📘 **Example:**
A neural network can classify images of cats vs dogs by learning from labeled training data.

### **Discriminative vs Generative Models:**

| Feature        | Discriminative                          | Generative                  |                |    |
| -------------- | --------------------------------------- | --------------------------- | -------------- | -- |
| **Definition** | Learn decision boundary between classes | Model how data is generated |                |    |
| **Output**     | P(y                                     | x)                          | P(x, y) or P(x | y) |
| **Examples**   | Logistic Regression, Neural Networks    | Naïve Bayes, GANs           |                |    |
| **Goal**       | Classify data                           | Generate new data samples   |                |    |

✅ **Conclusion:** Neural networks are strong discriminative models — excellent for recognizing patterns, but they don’t generate data like generative models do.

---

## 🔹 Q26. Apply MLE to estimate the parameters of a Gaussian distribution.

**Answer:**

* **MLE (Maximum Likelihood Estimation):** It finds parameter values that make the observed data most likely.
* For Gaussian distribution, parameters = Mean (μ) and Variance (σ²).

### **Steps:**

1. **Write Likelihood Function:**
   L(μ, σ²) = Π [1 / (√(2πσ²))] * exp[-(xi - μ)² / (2σ²)]
2. **Take Log:** Simplifies multiplication into addition.
3. **Differentiate:** Set derivative = 0 to find μ and σ².
4. **Result:**

   * Mean (μ̂) = Σxi / n
   * Variance (σ̂²) = Σ(xi - μ̂)² / n

📘 **Example:**
If exam scores are {70, 75, 80}, MLE estimates:
μ̂ = 75, σ̂² = 16.67.

✅ **Conclusion:** MLE helps estimate parameters that best describe data, ensuring the model fits real-world observations.

---

## 🔹 Q27. Explain how multinomial models are used in text classification. Describe the relationship between generalized linear models and linear regression.

**Answer:**

* **Multinomial Model in Text Classification:**

  * It predicts the probability of a document belonging to multiple classes.
  * Often used in **Naïve Bayes classifiers** for tasks like spam detection.
  * Considers frequency of words (features) in documents.

📘 **Example:**
If words like “free” and “offer” appear often, the model predicts “Spam = Yes.”

* **Relationship between GLM and Linear Regression:**

  * **Linear Regression:** Models continuous outputs using straight-line relationships.
  * **Generalized Linear Models (GLMs):** Extend linear regression to handle non-normal distributions and link functions (e.g., logistic, Poisson).

✅ **Conclusion:** Multinomial models handle categorical outcomes efficiently, while GLMs generalize regression for various data types.

---

## 🔹 Q28. Evaluate the impact of prior selection in Bayesian learning.

**Answer:**

* **Bayesian Learning:** Updates prior beliefs with new data using Bayes’ Theorem.

  * Formula: Posterior = (Likelihood × Prior) / Evidence

### **Impact of Prior Selection:**

1. **Informative Prior:** Reflects strong prior knowledge → influences posterior strongly.
2. **Non-Informative Prior:** Minimal prior knowledge → data dominates the result.
3. **Wrong Prior:** Can mislead results if it contradicts actual data.
4. **More Data = Less Prior Effect:** As data increases, posterior depends more on new evidence.

📘 **Example:**
If you believe a student is 90% likely to pass before seeing marks (strong prior), that belief affects the final probability even after viewing data.

✅ **Conclusion:** Choosing the right prior is crucial; it balances expert belief with observed data for accurate Bayesian predictions.

---

## 🔹 Q29. Compare logistic regression and support vector machines (SVM) as discriminative classifiers.

**Answer:**

| Feature              | Logistic Regression              | Support Vector Machine (SVM)                   |
| -------------------- | -------------------------------- | ---------------------------------------------- |
| **Type**             | Probabilistic model              | Geometric model                                |
| **Output**           | Probability (0–1)                | Decision boundary (margin)                     |
| **Objective**        | Maximize likelihood              | Maximize margin between classes                |
| **Kernel Support**   | Limited                          | Supports linear & nonlinear (kernel) functions |
| **Interpretability** | Easy                             | Complex                                        |
| **Use Case**         | Medical or financial predictions | Image or text classification                   |

📘 **Example:**

* Logistic Regression → Predict whether a student passes (Yes/No).
* SVM → Separate handwritten digits using boundary lines.

✅ **Conclusion:** Logistic Regression is simpler and interpretable; SVM is powerful for high-dimensional and nonlinear data.

---

## 🔹 Q30. Evaluate the effectiveness of generative models in unsupervised learning tasks.

**Answer:**

* **Generative Models:** Learn how data is generated by estimating **P(x)** — the probability of input features.
* Used in unsupervised learning where labels are not available.

### **Effectiveness:**

1. **Data Generation:** Can create new realistic samples (e.g., GANs generating faces).
2. **Feature Learning:** Capture hidden patterns or structures in data.
3. **Missing Data Handling:** Estimate missing values from learned distributions.
4. **Denoising:** Improve data quality (e.g., in images or audio).

📘 **Example:**

* **GANs:** Generate realistic human faces.
* **VAEs:** Learn compressed representations for image reconstruction.

✅ **Conclusion:** Generative models are powerful for unsupervised tasks like image synthesis, clustering, and data augmentation, but require large data and computational resources.

---

✅ **End of Unit 3 Answer Key** — All answers are in 7-mark detailed format with examples, definitions, and comparisons for clarity.

✅ **End of Unit 1 (7-Mark Detailed Answer Key)**
