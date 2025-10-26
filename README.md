Minimum Spanning Tree (MST) Algorithms Analysis
Overview

This project implements and analyzes two fundamental Minimum Spanning Tree algorithms — Prim’s and Kruskal’s — to compare their performance on graphs of different sizes. The program is written in Java and includes automated graph generation, execution time measurement, operation counting, and JSON output for visualization.

Features

Implementation of Prim’s and Kruskal’s algorithms

Automatic generation of random connected graphs

Performance comparison based on:

Execution time (ms)

Number of operations

Results exported in JSON format

Visualization and statistical analysis in Python

Graphs generated:

5 small (30 nodes)

10 medium (300 nodes)

10 large (1000 nodes)

3 extra large (1300, 1600, 2000 nodes)

Project Structure
MSTProject/
├── pom.xml
├── output.json
├── visualize_mst.py
├── plot_performance.py
├── plot_operations.py
└── src/
    └── main/java/org/example/
        ├── Main.java
        ├── model/
        │   ├── Graph.java
        │   └── Edge.java
        ├── alg/
        │   ├── PrimKruskal.java
        │   ├── MSTResult.java
        │   └── UnionFind.java
        └── io/
            └── IOUtils.java

Technologies

Java 17

Maven

Jackson (for JSON handling)

JUnit (for testing)

Python 3

Matplotlib, NetworkX

How to Run
Java (Data Generation)

Open the project in IntelliJ IDEA

Run Main.java

The file output.json will be generated in the root directory

Python (Visualization)

Run:

python plot_performance.py
python plot_operations.py


This will generate:

performance_by_category.png

operations_complexity_analysis.png

Example Results
Performance by Category

Operations Complexity Analysis

Conclusion

Both Prim’s and Kruskal’s algorithms produce the same MST cost for all graphs, but their time and operation complexity differ. Kruskal performs better on sparse graphs, while Prim becomes more efficient for dense graphs due to its adjacency list structure and priority queue optimization
