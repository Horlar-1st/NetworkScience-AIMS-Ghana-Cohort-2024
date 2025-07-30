# Social Network Analysis (AIMS-GHANA Cohort 2024–2025)

This repository presents a detailed analysis of the social interaction network within the **AIMS Ghana Cohort 2024–2025**. The goal is to explore how students interact socially and academically, identify influential individuals, discover communities, and uncover patterns that may influence collaboration, integration, and learning dynamics based on the data taken from their sitting arrangment at the cafeteria.

---

## 📁 Dataset Overview

- **Filename:** `AIMSGHANANET25.csv`
- **Description:** Contains social network data of students in the AIMS Ghana 2024–2025 cohort.
- **Data Columns:**
  - `Name` – Student's first name (used as the node label)
  - `Country` – Country of origin
  - `Background` – Academic background (e.g., Mathematics, Computer Science, Statistics, etc)
  - `Friend1`, `Friend2`, `Friend3` – Names of three students most frequently sit with at the cafeteria

Each student is represented as a **node**, and their three listed friends are connected to them as **edges**, forming a directed social interaction graph.

---

## 🎯 Project Objectives

The analysis is guided by the following key questions:

1. **Is the network connected?**
   - Investigate the existence of a giant component and isolated subgraphs.

2. **Who are the most influential people?**
   - Apply centrality measures (degree, eigenvector, betweenness, etc) to identify key players in the network.

3. **What is the degree distribution?**
   - Assess how socially connected the network is and understand the network's density.

4. **Are there communities?**
   - Use algorithms like Louvain to detect social or academic clusters.

5. **How far apart are people?**
   - Measure shortest paths and calculate average path lengths.

6. **How clustered is the network?**
   - Evaluate the clustering coefficient to reveal local groupings and triadic closures.

7. **Which connections are bridges?**
   - Identify edges that act as bridges between otherwise disconnected groups (weak ties theory).

8. **Who controls information flow?**
   - Use betweenness centrality to find nodes with influence over indirect connections.

9. **What happens if key nodes are removed?**
   - Test the robustness of the network against targeted and random node removals.

10. **How does the network look visually?**
    - Plot the graph, highlight communities, key nodes, and clusterings.

11. **What does the degree distribution tell us about social interactions?**
    - Interpret connectivity and interaction tendencies (homogeneous vs. heterogeneous network).

12. **Who are the top 5 most influential students based on degree centrality?**
    - List and interpret their roles in the cohort’s social dynamics.

13. **What role do isolated students play, and should they be integrated more?**
    - Analyze network periphery and inclusion strategies.

14. **Can we predict friendships based on common connections?**
    - Use similarity indices uisng Jaccard index for link prediction modeling.

---

## 🛠 Tools & Libraries

- **Language:** Python
- **Core Libraries:**
  - `networkx` – Graph modeling and metrics
  - `pandas` – Data loading and preprocessing
  - `matplotlib`, `seaborn` – Static plotting
  - `community` – Louvain community detection

---
## Library Needed 
- **Community** - `pip install python-louvain`
- **Networkx** - `pip install networkx`
