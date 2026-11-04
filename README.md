# 🧭 PathMind AI — Interactive Spatial Routing Engine

**PathMind AI** is an interactive algorithm visualization platform that demonstrates how intelligent search algorithms navigate weighted graphs to discover optimal paths. Designed with a modern Cognitive AI SaaS-inspired interface, it transforms complex graph traversal concepts into an intuitive, real-time visual experience.

Explore how algorithms evaluate nodes, calculate path costs, prioritize routes, and make decisions through interactive maps, live telemetry, and step-by-step execution.

---

## ✨ Key Features

### 🗺️ 1. Interactive Cartography
- Explore interactive, map-inspired weighted graph environments.
- Drag and reposition city nodes dynamically.
- Automatically recalculate Euclidean heuristic values `h(n)` and edge distances.
- Visualize connections and weighted routes between nodes.

### ⏯️ 2. Step-by-Step Algorithm Playback
- Play and pause algorithm execution in real time.
- Navigate through individual execution steps.
- Scrub through the algorithm's execution timeline.
- Observe how the Frontier (Open List) evaluates and prioritizes nodes.
- Understand the complete decision-making process behind pathfinding.

### 📊 3. Live Node Telemetry

Monitor the three fundamental evaluation parameters of A*:

| Parameter | Description |
|---|---|
| **g(n)** | Actual cost from the starting node to the current node. |
| **h(n)** | Estimated cost from the current node to the destination. |
| **f(n)** | Total estimated path cost, calculated as `f(n) = g(n) + h(n)`. |

Watch these values update dynamically as the algorithm explores the graph.

### ⚡ 4. Multi-Algorithm Benchmarking

Compare different search strategies and understand their efficiency, behavior, and optimality.

Supported algorithms:

- **A* Search:** Uses actual path cost and heuristic estimation to find an optimal path under suitable heuristic conditions.
- **Dijkstra's Algorithm:** Explores nodes based on the lowest accumulated path cost.
- **Greedy Best-First Search:** Prioritizes nodes based only on heuristic distance to the destination.
- **Breadth-First Search (BFS):** Explores nodes level by level, finding minimum-edge paths in unweighted graphs.

Compare node expansions and execution behavior across algorithms.

### 🌍 5. Diverse Map Presets

Experiment with different graph configurations and routing scenarios:

- **India National Highway Network:** Explore a map-inspired representation of Indian highway connections.
- **European Rail Network:** Experiment with interconnected railway-style routes.
- **Heuristic Trap:** Understand how misleading heuristic estimates can influence search decisions and trigger backtracking.
- **Random City Layouts:** Generate procedurally created graph environments for additional experimentation.

---

## 🛠️ Tech Stack

PathMind AI is built using lightweight web technologies without requiring a frontend framework or build pipeline.

| Technology | Purpose |
|---|---|
| HTML5 | Application structure and interface |
| Tailwind CSS | Responsive styling and UI design |
| Vanilla JavaScript | Algorithm implementation, application logic, and state management |
| Inline SVG | Interactive graph rendering and dynamic node manipulation |
| DOM API | Real-time visualization and interface updates |

**Architecture:** Zero-build, static web application.

---

## 🚀 Getting Started

PathMind AI is a self-contained static application. No package manager, framework installation, or build process is required.

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.).
- Git (optional, for cloning the repository).

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/Ashwin-singh07/pathmind-ai.git
```

**2. Navigate to the project directory**

```bash
cd pathmind-ai
```

**3. Launch the application**

Simply open `index.html` in your preferred web browser.

Alternatively, use VS Code with the Live Server extension for local development.

---

## 🧠 Understanding the A* Algorithm

At the core of PathMind AI is the A* Search Algorithm, an informed search algorithm that combines the actual cost of reaching a node with an estimated cost of reaching the destination.

Its evaluation function is:

`f(n) = g(n) + h(n)`

Where:

- **g(n):** Cost of the path from the starting node to node `n`.
- **h(n):** Estimated cost from node `n` to the goal.
- **f(n):** Estimated total cost of a path through node `n`.

At each iteration, A* selects the node with the lowest estimated total cost, evaluates its neighbors, and updates their path costs when a better route is discovered.

With an admissible heuristic and appropriate implementation conditions, A* guarantees an optimal solution.

---

## 📂 Project Structure

```text
pathmind-ai/
│
├── index.html          # Main application interface
├── README.md           # Project documentation
└── assets/             # Optional static assets
```

*Note: The structure above is illustrative. Adjust it according to the actual repository files.*

---

## 🎯 Project Objectives

- Visualize the internal working of informed and uninformed search algorithms.
- Demonstrate how heuristic functions influence search efficiency.
- Provide an interactive environment for understanding weighted graph traversal.
- Compare different pathfinding strategies through visual benchmarking.
- Make complex Artificial Intelligence search concepts easier to understand through experimentation.

---

## 🔮 Future Enhancements

Potential improvements include:

- Custom graph creation with user-defined nodes and weighted edges.
- Additional algorithms such as IDA*, Bidirectional Search, and Beam Search.
- Advanced performance analytics and execution statistics.
- Exportable algorithm execution traces.
- Custom heuristic configuration and admissibility testing.
- Responsive mobile-first visualization experience.

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome!

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add: your feature description"
   ```

4. Push your branch:

   ```bash
   git push origin feature/your-feature
   ```

5. Open a Pull Request.

---

## 📜 License

This project is open-source. A license can be added to the repository to define the terms under which others may use, modify, and distribute the project.

---

<p align="center">
  <strong>PathMind AI</strong><br>
  Making intelligent pathfinding visible, interactive, and understandable.
</p>
