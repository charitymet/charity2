# Essential AI/ML Concepts: Quick Study Guide

## 1. Intelligent Agents and Architecture

An **Intelligent Agent (IA)** is like a smart program or system that can perceive its surroundings, think about them, and then act. It operates in a cycle of **perceiving** (sensing the environment), **thinking** (making decisions), and **acting** (performing actions).

- **Core Idea**: An AI system studies a **rational agent** and its interaction with the **environment**.
- **Sensors**: How the agent gathers information (e.g., camera, microphone, keyboard input).
- **Actuators**: How the agent performs actions (e.g., motors, screen display, robotic arm).
- **Mental Properties**: Agents can have properties like knowledge, beliefs, and intentions.

**Four Key Rules for an AI Agent**:

1.  **Perception of the Environment**:
    - The agent must be able to sense or gather information about the current state of its environment using its sensors.
2.  **Use of Observation for Decision-making**:
    - The agent uses the gathered information (observations) to make informed decisions aimed at achieving its goals.
3.  **Action based on Decision**:
    - The decisions made should lead to the agent taking appropriate actions or behaviors to affect its environment and achieve its intended outcomes.
4.  **Rational Action**:
    - The actions taken should be **rational** – meaning they are the best possible actions to maximize the agent's chances of success or achieving its goals, given its knowledge and perceptions.

**Types of Agents by Environment Interface**:

- **Human Agent**:
  - Sensors: Eyes, ears, other organs.
  - Actuators: Hands, legs, vocal tract.
- **Robotic Agent**:
  - Sensors: Cameras, infrared range finders, NLP (for understanding language).
  - Actuators: Various motors, grippers.
- **Software Agent**:
  - Sensors (Inputs): Keystrokes, file contents, network packets.
  - Actuators (Outputs): Displaying on screen, writing to files, sending network packets.

**Real Example**: A **robot vacuum cleaner**.

- It **senses** dirt on the floor using its sensors.
- It **decides** where to move to clean the dirt based on its programming and what it "knows" about the room.
- It **acts** by moving to the location and vacuuming the dirt.
- Good intelligent agents can also **learn from experience** to become more efficient. A thermostat is another simple example of an intelligent agent.

## 2. Types of Agents by Complexity

1.  **Simple Reflex Agents**:

    - Act based only on the **current percept** (what it senses right now).
    - Uses simple "condition-action" rules (e.g., if X, then do Y).
    - No memory of past states or history.
    - Example: A basic thermostat that turns on heat if the temperature is below a set point, without considering how long it's been cold.

2.  **Model-Based Reflex Agents**:

    - Maintains an **internal model** or representation of the world.
    - Tracks how the world changes and how its own actions affect the world.
    - Uses this model along with the current percept to make decisions.
    - Example: An autonomous vacuum cleaner that builds a map of the room (its model) and uses it to navigate efficiently and remember cleaned areas.

3.  **Goal-Based Agents**:

    - Driven by **goals** or objectives they strive to achieve.
    - Considers various possible action sequences and their potential outcomes to select the one that leads to a goal state.
    - Example: A delivery drone that needs to deliver a package. It plans its route considering factors to reach the destination (goal).

4.  **Utility-Based Agents**:

    - Make decisions by evaluating the **utility** (or desirability/happiness) of different states or outcomes.
    - Chooses actions that maximize its expected utility, not just achieving a goal but achieving it in the "best" way.
    - Example: An automated personal assistant scheduling tasks. It considers not just _if_ a task gets done, but also factors like user preferences, deadlines, and task importance to create an optimal schedule.

5.  **Learning Agents**:
    - Have the ability to **improve their performance over time** through learning from experience.
    - Can adapt to new situations and get better at their tasks.
    - May use various learning mechanisms (e.g., supervised learning, reinforcement learning).
    - Example: An autonomous vehicle that learns to navigate through traffic by observing and adapting to different driving scenarios and feedback.

**Mnemonic**: "**S**illy **M**onkeys **G**ive **U**nique **L**essons" or "**SMALL**" - **S**imple, **M**odel-based, go**A**l-based (adjusted for 'A'), **U**tility-based, **L**earning.

## 3. Agent Environments

The **environment** is the world or context in which the agent operates. Environments can vary widely:

- **Observability**:
  - _Fully Observable_: Agent's sensors give it access to the complete state of the environment at each point in time.
  - _Partially Observable_: Agent only has access to a part of the environment's state.
- **Determinism**:
  - _Deterministic_: The next state of the environment is completely determined by the current state and the agent's action.
  - _Stochastic_: There's uncertainty; the next state is not fully predictable even if the action is known (e.g., a robot's wheel slipping).
- **Dynamics**:
  - _Static_: The environment does not change while the agent is deliberating or deciding on an action.
  - _Dynamic_: The environment can change on its own while the agent is thinking.
- **Episodic vs. Sequential**:
  - _Episodic_: Agent's experience is divided into atomic episodes. The choice of action in one episode does not affect future episodes (e.g., classifying images one by one).
  - _Sequential_: Current decisions can affect all future decisions (e.g., playing chess).
- **Discrete vs. Continuous**:
  - Refers to the nature of the environment's state, the way time is handled, and the agent's perceptions and actions.
  - _Discrete_: Finite number of distinct states, percepts, actions (e.g., a crossword puzzle).
  - _Continuous_: States/actions can take on a range of values (e.g., driving a car involves continuous speed and steering angles).
- **Single vs. Multi-agent**:
  - _Single-agent_: Agent operates by itself.
  - _Multi-agent_: Multiple agents interact in the environment, which can be cooperative or competitive.

**Agent-Environment Interaction Example**:
Consider a **self-driving car** in city traffic:

- The car (agent) continuously **perceives** its surroundings (other cars, pedestrians, traffic lights) using sensors like cameras and LiDAR.
- Based on this sensory input and its internal knowledge (its model of driving rules, maps), the car **processes** this information and makes **decisions** about steering, acceleration, and braking.
- These **actions** affect the car's trajectory and interactions, shaping its future observations and decisions.
  This framework helps in analyzing and designing intelligent systems across various domains.

## 4. PEAS Framework

**PEAS** is a structured way to define an intelligent agent and its task. It stands for:

- **P**erformance Measure: How is the agent's success evaluated? What makes it good or bad at its job?
  - _Example (Self-driving car)_: Safety, speed, legality, comfort, minimizing travel time.
- **E**nvironment: Where does the agent operate? What are the characteristics of this world?
  - _Example (Self-driving car)_: Roads, other vehicles, pedestrians, traffic signals, weather conditions.
- **A**ctuators: How does the agent act upon or influence its environment?
  - _Example (Self-driving car)_: Steering wheel, accelerator, brakes, display signals.
- **S**ensors: How does the agent perceive or sense its environment?
  - _Example (Self-driving car)_: Cameras, LiDAR, radar, GPS, speedometer, odometer.

**Purpose**: The PEAS representation helps developers clearly understand and model an agent's task, its capabilities, and the context it operates in, which is crucial for designing effective intelligent agents.

**Memory Aid**: "PEAS in a pod" - all components must work together for a well-defined agent.

## 5. Search Algorithms

### Uninformed Search (Blind Search)

Doesn't use any information about the distance to the goal.

- **Breadth-First Search (BFS)**:

  - Explores all neighbors at the present depth before moving to nodes at the next depth level.
  - **Pros**: Finds the shallowest goal (optimal if path costs are equal), guaranteed to find a solution if one exists (complete).
  - **Cons**: High memory usage (stores all frontier nodes).
  - **When to use**: When the solution is not too deep, and optimality (shortest path) is needed.

- **Depth-First Search (DFS)**:
  - Explores as far as possible along each branch before backtracking.
  - **Pros**: Lower memory usage than BFS (only stores nodes on current path).
  - **Cons**: Can get trapped in infinite loops if not careful (on graphs with cycles), not guaranteed to find the optimal solution.
  - **When to use**: When solutions are expected to be deep, memory is a concern, or any solution is acceptable.

### Informed Search (Heuristic Search)

Uses problem-specific knowledge (heuristics) to find solutions more efficiently.

- **Best-First Search**:

  - Expands the node that appears to be closest to the goal, according to a heuristic evaluation function. (Greedy Best-First Search is a common type).

- **A\* (A-star) Algorithm**:

  - Combines the cost to reach the node (g(n)) and the estimated cost from the node to the goal (h(n)).
  - **Formula**: f(n) = g(n) + h(n)
    - g(n): Actual cost from the start node to node n.
    - h(n): Heuristic estimate of the cost from node n to the goal.
  - **Key Property**: A\* is optimal and complete if the heuristic h(n) is admissible (never overestimates the true cost to the goal) and consistent (for any node n and successor n' generated by action a, h(n) ≤ cost(n,a,n') + h(n')).
  - **Memory trick**: "A\* is A+ at finding optimal paths efficiently."

- **Hill Climbing**:
  - A local search algorithm that continuously moves in the direction of increasing value (uphill) to find the peak (best state).
  - **Problem**: Can get stuck in local maxima (a peak that isn't the highest overall) or on plateaus.
  - **Solutions**: Random restarts, simulated annealing.

## 6. Logic and Reasoning

### Propositional Logic

- Deals with propositions (statements that are either TRUE or FALSE).
- Uses logical connectives (operators) like AND (∧), OR (∨), NOT (¬), IMPLIES (→), IF AND ONLY IF (↔).
- Example: If "It is raining" (P) AND "I have an umbrella" (Q), then "I will not get wet" (R). (P ∧ Q) → ¬S (where S is "I will get wet").

### Inference Methods

How new facts or conclusions are derived from existing knowledge.

1.  **Forward Chaining** (Data-Driven):

    - Starts with known facts (data).
    - Applies inference rules to these facts to derive new facts.
    - Continues until the goal is reached or no new facts can be derived.
    - Example: Medical diagnosis – starting with patient's symptoms (facts) and applying medical rules to reach a diagnosis (goal).

2.  **Backward Chaining** (Goal-Driven):
    - Starts with a potential conclusion or goal.
    - Works backward by finding rules that could lead to this conclusion.
    - Tries to prove the premises of these rules, which may become new sub-goals.
    - Example: A detective trying to solve a crime (goal) by looking for evidence (facts) that supports or refutes hypotheses.

**Tip**: Remember Forward as "**F**acts **F**irst" and Backward as "**B**egin with the **B**elief (Goal)".

## 7. Machine Learning Basics

### Supervised Learning

- Learns from **labeled training data** (input-output pairs).
- The goal is to learn a mapping function that can predict the output for new, unseen inputs.
- Types:
  - **Classification**: Predicts a categorical label (e.g., "spam" or "not spam", "cat" or "dog").
  - **Regression**: Predicts a continuous value (e.g., house price, temperature).

### Unsupervised Learning

- Learns from **unlabeled data** (only inputs, no corresponding outputs).
- The goal is to find hidden patterns, structures, or relationships in the data.
- Types:
  - **Clustering**: Groups similar data points together (e.g., customer segmentation).
  - **Association Rule Learning**: Discovers relationships between variables (e.g., "customers who buy X also tend to buy Y").
  - **Dimensionality Reduction**: Reduces the number of variables while preserving important information.

### Reinforcement Learning

- An agent learns by interacting with an environment.
- The agent takes actions, and the environment provides feedback in the form of **rewards or penalties**.
- The goal is to learn a policy (a strategy for choosing actions) that maximizes the cumulative reward over time.
- Example: Training an AI to play a game (like chess or Go) by rewarding wins and penalizing losses.

## 8. Key ML Algorithms

### K-Nearest Neighbors (KNN)

- A simple supervised learning algorithm for classification (and regression).
- Classifies a new data point based on the majority class of its 'K' closest neighbors in the feature space.
- "Birds of a feather flock together."
- **When to use**: Small datasets, when the decision boundary is irregular, simple to implement.
- **Considerations**: Choosing K, distance metric, can be slow for large datasets.

### Naive Bayes

- A probabilistic classifier based on **Bayes' Theorem**.
- "Naive" because it assumes that features are conditionally independent given the class.
  - Bayes' Theorem: P(A|B) = [P(B|A) * P(A)] / P(B)
- **Example**: Spam email detection (calculates probability of email being spam given certain words).
- **When to use**: Text classification, medical diagnosis, when features are mostly independent. Fast and efficient.

### Decision Trees

- A tree-like model where each internal node represents a test on an attribute, each branch represents an outcome of the test, and each leaf node represents a class label or a continuous value.
- Easy to understand and interpret.
- **Example**: Deciding whether to approve a loan based on income, credit score, age, etc.
- **When to use**: When interpretability is important, for both classification and regression.
- **Risk**: Can overfit if not pruned.

### Random Forest

- An **ensemble learning** method that constructs multiple decision trees during training.
- For classification, the output is the class selected by most trees; for regression, it's the average prediction of the individual trees.
- **Advantage**: Reduces overfitting (compared to a single decision tree) and generally improves accuracy and robustness.
- **When to use**: When higher accuracy is needed, and overfitting is a concern.

### Support Vector Machine (SVM)

- A supervised learning model that finds an optimal **hyperplane** (a decision boundary) that best separates data points of different classes in a high-dimensional space.
- Aims to maximize the margin between the classes.
- Effective in high-dimensional spaces and can model non-linear decision boundaries using the "kernel trick."
- **When to use**: Classification problems, especially with a clear margin of separation or non-linear data.

### Clustering Algorithms

- **K-Means Clustering**:

  - An iterative algorithm that partitions data into 'K' predefined, non-overlapping clusters.
  - **Steps**:
    1.  Randomly initialize 'K' cluster centroids.
    2.  Assign each data point to the nearest centroid.
    3.  Recalculate the centroids as the mean of the points in each cluster.
    4.  Repeat steps 2-3 until centroids no longer change significantly.
  - **Challenge**: Choosing the optimal number of clusters (K).

- **Hierarchical Clustering**:
  - Builds a hierarchy of clusters, often represented as a tree-like diagram called a **dendrogram**.
  - _Agglomerative (bottom-up)_: Starts with each point as a cluster and merges them.
  - _Divisive (top-down)_: Starts with all points in one cluster and splits them.
  - No need to specify the number of clusters beforehand.

### Dimensionality Reduction

- **Principal Component Analysis (PCA)**:
  - Reduces the number of features (dimensions) in a dataset while trying to preserve as much of the original variance (information) as possible.
  - Transforms data into a new set of uncorrelated variables called principal components.
  - **Uses**: Data visualization, speeding up algorithms, noise reduction.

### Neural Networks (Artificial Neural Networks - ANNs)

- Inspired by the structure and function of the human brain.
- Consist of interconnected layers of nodes (neurons):
  - **Input Layer**: Receives initial data.
  - **Hidden Layer(s)**: Perform computations and feature extraction. Networks with many hidden layers are "deep" (Deep Learning).
  - **Output Layer**: Produces the final result (e.g., classification or regression value).
- **Activation Functions**: Introduce non-linearity (e.g., Sigmoid, ReLU, Tanh).
  - _Sigmoid_: f(x) = 1 / (1 + e^-x) --- Squashes output to (0, 1).
  - _ReLU_ (Rectified Linear Unit): f(x) = max(0, x) --- Common, helps with vanishing gradient.
  - _Tanh_ (Hyperbolic Tangent): f(x) = (e^x - e^-x) / (e^x + e^-x) --- Squashes output to (-1, 1).
- **Training**: Typically involves **gradient descent** (and backpropagation) to adjust weights and biases to minimize a loss function.
  - _Gradient Descent Formula_: New Weight = Old Weight - LearningRate \* GradientOfLoss
  - _Types_: Batch, Mini-batch, Stochastic Gradient Descent (SGD).

### Association Rule Learning

- **Apriori Algorithm**:
  - Finds frequent itemsets in a dataset (items that often appear together).
  - Generates association rules from these frequent itemsets (e.g., "If a customer buys bread, they are likely to buy butter").
  - Used in **Market Basket Analysis**.
  - **Key Metrics**:
    - _Support_: How frequently the itemset appears in the dataset.
    - _Confidence_: How often the rule has been found to be true.
    - _Lift_: The ratio of observed support to that expected if X and Y were independent. Lift > 1 suggests items are more likely to be bought together.

## 9. Applications of AI/ML

- **Expert Systems**: Emulate human expert decision-making (e.g., medical diagnosis, financial planning).
- **Natural Language Processing (NLP)**: Enabling computers to understand, interpret, and generate human language (e.g., machine translation, chatbots, sentiment analysis).
- **Computer Vision**: Enabling computers to "see" and interpret visual information (e.g., image recognition, object detection, facial recognition).
- **Robotics**: Designing and controlling robots (e.g., autonomous vehicles, industrial automation, surgical robots).
- **Data Mining & Predictive Analytics**: Discovering patterns in large datasets and making predictions about future outcomes (e.g., stock market prediction, customer churn prediction, fraud detection).
- **Healthcare**: Disease diagnosis, drug discovery, personalized medicine, medical imaging analysis.

## 10. Memory Tricks & Key Takeaways

- **Agent Components (PEAS)**: "PEAS for a perfect agent" (Performance, Environment, Actuators, Sensors).
- **Agent Types (Complexity)**: "SMALL" or "Silly Monkeys Give Unique Lessons" (Simple, Model-based, goAl-based, Utility-based, Learning).
- **Reasoning Types**: "FB" - Forward builds from Facts, Backward begins with Belief (Goal).
- **ML Types**: "SUR" - Supervised has answers (labels), Unsupervised finds patterns, Reinforcement learns by rewards.
- **Neural Network Basics**: "IHO" - Input processes, Hidden learns, Output predicts.
- **Search Algorithms**: "BFS for shortest path (if costs uniform), DFS for memory savings, A\* for optimal paths with heuristics."

**Core Idea of AI**: Creating systems that can perceive their environment, reason about it, and act intelligently to achieve goals.
**Core Idea of ML**: Enabling systems to learn from data without being explicitly programmed for each task.
