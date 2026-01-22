# Optimization in Deep Learning: Learning Rates, Stability, and Drift

This notebook explores how optimization choices directly affect training stability,
generalization, and real-world performance in machine learning models.

Rather than focusing on model architecture alone, the goal here is to understand
**how learning rate selection, optimizer choice, and scheduling strategies influence
both convex and non-convex optimization problems**.

---

## What This Notebook Covers

- Logistic Regression on a convex loss surface
- Multi-Layer Perceptron (MLP) training on a non-convex loss
- Effects of learning rate magnitude on convergence and stability
- SGD vs Adam behavior under identical conditions
- Constant vs decaying learning rate schedules
- Overfitting and generalization gaps
- Concept drift and post-deployment performance degradation

All experiments are backed by quantitative results and visualizations.

---

## Key Takeaways

- Even convex problems can fail to converge with poor learning rate selection
- Non-convex optimization is highly sensitive to optimizer choice
- Adam converges more consistently than SGD under the same constraints
- High training accuracy does not imply strong generalization
- Data distribution drift can significantly reduce accuracy without any model changes

This reinforces why **training metrics alone are not sufficient** and why
monitoring and retraining strategies are critical in deployed systems.

---

## Why This Matters

These experiments reflect real challenges faced in production ML systems:
models can appear to perform well during training and validation,
yet degrade over time due to optimization instability or changing data.

Understanding these dynamics is essential for building **robust, maintainable ML pipelines**.

---

## Tools & Frameworks

- Python
- PyTorch
- NumPy
- Matplotlib

---

## File

- `learning_rate_optimization.ipynb`

---

## Author

Cordell Stonecipher  
AI / Machine Learning | Optimization & Training Dynamics
