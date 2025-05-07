# Essential AI/ML Concepts: Quick Study Guide

## 1. Intelligent Agents

An intelligent agent perceives its environment through **sensors** and acts on it through **actuators**.

Four key rules:

1. **Perception** - Collect information from environment
2. **Decision-making** - Use observations to decide
3. **Action** - Act based on decisions
4. **Rationality** - Take actions that maximize goal achievement

**Example**: A smart thermostat senses room temperature, decides if it's too hot/cold, turns on heating/cooling to maintain desired temperature.

## 2. Types of Agents

1. **Simple Reflex Agents**: Act based only on current perception (like a thermostat)
2. **Model-Based Agents**: Maintain internal model of world (like a robot vacuum that maps a room)
3. **Goal-Based Agents**: Work toward specific goals (like a delivery drone planning routes)
4. **Utility-Based Agents**: Maximize "happiness" by evaluating desirability of states (like a personal assistant prioritizing tasks)
5. **Learning Agents**: Improve performance over time (like self-driving cars getting better with experience)

## 3. Search Algorithms

### Uninformed Search

- **Breadth-First Search (BFS)**: Explores all neighbors before moving to next level
  - **Pros**: Finds shortest path, guaranteed to find solution
  - **Cons**: Memory intensive
- **Depth-First Search (DFS)**: Explores as far as possible before backtracking
  - **Pros**: Uses less memory than BFS
  - **Cons**: May get trapped in infinite paths, solution not optimal

### Heuristic Search

- **Best-First Search**: Uses heuristic to guide search toward goal
- **A\* Algorithm**: Combines path cost so far + estimated cost to goal

  - **Formula**: f(n) = g(n) + h(n)
  - Most efficient when h(n) never overestimates cost to goal

- **Hill Climbing**: Always moves in direction of increasing value
  - **Problem**: Gets stuck in local maxima

## 4. Logic and Reasoning

- **Propositional Logic**: Statements that are true/false combined with AND, OR, NOT
- **Forward Chaining**: Start with known facts, apply rules to reach goal
- **Backward Chaining**: Start with goal, work backward to find supporting facts

## 5. Machine Learning Basics

### Supervised Learning Algorithms

1. **K-Nearest Neighbors (KNN)**

   - Classifies based on majority vote of K closest neighbors
   - **Example**: Identifying if an animal is a cat or dog based on similarity to known examples

2. **Naive Bayes**

   - Uses probability and assumes feature independence
   - **Example**: Spam email detection based on word frequencies

3. **Decision Trees**

   - Creates tree-like model of decisions
   - **Example**: Loan approval decision based on income, credit score, etc.

4. **Random Forest**

   - Ensemble of multiple decision trees
   - **Advantage**: Reduces overfitting, improves accuracy

5. **Support Vector Machine (SVM)**
   - Finds optimal hyperplane separating classes
   - Good for high-dimensional data

### Unsupervised Learning

1. **Clustering**

   - **Hierarchical**: Builds tree of clusters (bottom-up or top-down)
   - **K-means**: Groups data into K clusters

2. **Principal Component Analysis (PCA)**
   - Reduces dimensions while preserving variance
   - **Steps**: Standardize data → Compute covariance → Find eigenvectors → Project data

### Neural Networks

- **Structure**: Input layer → Hidden layer(s) → Output layer
- **Activation Functions**:

  - **Sigmoid**: Output between 0-1, useful for binary classification
  - **ReLU**: f(x) = max(0,x), helps with vanishing gradient problem
  - **Tanh**: Output between -1 to 1, centered at zero

- **Gradient Descent**: Optimization algorithm that minimizes error
  - **Formula**: θ = θ - α \* ∇J(θ)
  - α is learning rate

## 6. Association Rule Learning

- **Apriori Algorithm**: Finds frequent itemsets and generates rules
  - **Example**: Customers who buy bread often buy butter too

## 7. Applications of ML

- **Image Recognition**: Object detection, facial recognition
- **Natural Language Processing**: Translation, sentiment analysis
- **Predictive Analytics**: Stock market prediction, demand forecasting
- **Healthcare**: Disease diagnosis, personalized medicine
- **Autonomous Vehicles**: Self-driving cars, drones

## Memory Tricks

- **Types of Agents mnemonic**: "SMALL" - Simple, Model-based, goAl-based, utiLity-based, Learning
- **ML algorithm selection**: "If data is small, try KNN. If features are independent, try Naive Bayes. If interpretability matters, use Decision Tree."
- **Neural Network basics**: "IHO" - Input processes, Hidden learns, Output predicts
