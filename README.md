# The Hidden Backbone of Indian Railways 🚆

### A Graph-Based Network Analysis of India's Railway Connectivity

This project explores the structure and connectivity of the Indian Railways network using graph visualization and network analysis techniques. It identifies highly connected railway stations, important bridging stations, regional communities, and the potential impact of removing critical hubs from the network.

## 📌 Project Overview

Indian Railways is one of the world's largest railway networks. Understanding its connectivity can help reveal which stations play the most important roles in maintaining network structure.

The project models the railway system as a graph, where:
- **Nodes** represent railway stations.
- **Edges** represent connections between stations.

The network is analyzed using graph metrics, community detection, and hub-removal experiments.

## 🗺️ Network Visualization

![Indian Railways Network Visualization](4.%20Indian_Railways_Regional_Network_Final.png)

The visualization highlights the interconnected railway network, with prominent stations and regional connectivity patterns.

## 📊 Key Findings

![Key Findings Dashboard](6.%20Deliverable3_Key_Findings.png)

### 1. Most Direct Connections (Degree)

| Railway Station | Degree |
|---|---:|
| Lokmanya Tilak | 24 |
| Katni South | 20 |
| Ahmedabad | 17 |
| Howrah | 16 |
| Kolkata Chitpur | 16 |

Lokmanya Tilak has the highest number of direct connections among the analyzed stations.

### 2. Most Important Bridging Stations

Based on betweenness centrality:

| Railway Station | Betweenness Centrality |
|---|---:|
| Lokmanya Tilak | 14,687 |
| Howrah Cabin | 9,202 |
| Ahmedabad | 6,314 |
| Niz-Sariha | 6,150 |
| Thansit | 6,140 |

These stations play important roles in connecting different parts of the network.

### 3. Community Detection

- **Communities identified:** 27
- **Modularity score:** 0.926
- **Community sizes:** 2–20 stations
- **Algorithm:** Louvain

The results reveal distinct groups of closely connected railway stations.

### 4. Hub-Removal Experiment

Removing Lokmanya Tilak, which has both the highest degree and highest betweenness centrality, produces a significant structural change.

| Network Metric | Before Removal | After Removal |
|---|---:|---:|
| Connected components | 1 | 8 |
| Stations cut off | 0 | 12 |
| Pairs still reachable | 100% | 91.8% |
| Average shortest path | 5.20 | 5.71 |
| Network diameter | 10 | 13 |

This experiment demonstrates how the removal of an important hub can affect overall network connectivity.

**Additional observation:** Gorakhpur has only 3 direct links, yet removing it cuts off 15 stations, highlighting that a station's importance is not determined by degree alone.

*Note: The hub-removal experiment is a hypothetical network experiment, not a prediction of actual railway service disruption.*

## 🛠️ Tools and Technologies

- Python
- Gephi
- Graph Theory
- Network Analysis
- Network Visualization
- CSV Datasets

## 📁 Repository Contents

| File | Description |
|---|---|
| `4. Indian_Railways_Regional_Network_Final.png` | Final railway network visualization |
| `6. Deliverable3_Key_Findings.png` | Key findings and network metrics |
| `2. indian_railways_nodes_final.csv` | Railway station node dataset |
| `3. indian_railways_edges_final.csv` | Railway network edge dataset |
| `8. node_metrics.csv` | Node-level network metrics |
| `Project_Report_v2.docx` | Detailed project report |
| `7. Hidden_Backbone_Indian_Railways.pptx` | Project presentation |
| [visualizations/](visualizations/) | Five Gephi network visualization files |

## 🎯 Conclusion

This analysis shows that railway network importance depends on more than the number of direct connections. Stations with high betweenness centrality can act as critical bridges between different regions, while community detection reveals the network's underlying structure.

The hub-removal experiment further demonstrates how the removal of selected stations can influence connectivity, shortest paths, and network fragmentation.

---

**Project:** The Hidden Backbone of Indian Railways  
**Focus:** Graph Visualization and Network Analysis
