# SC2001 - Algorithm Design and Analysis

This repository contains the implementation, empirical testing, and theoretical analysis for three major laboratory projects. The work focuses on algorithm optimization, graph theory, and dynamic programming.

**Team Members:** Perrin, Rohan, Alexa

## Repository Structure
*   **`lab1/mergeSort.ipynb`**: **Integration of Merge Sort & Insertion Sort.** Analysis of a hybrid sorting algorithm and finding the optimal threshold $S$.
*   **`lab2/dijkstraAlgorithm.ipynb`**: **Dijkstra’s Algorithm.** Comparison between Adjacency Matrix (Array PQ) and Adjacency List (Binary Heap) implementations.
*   **`lab3/dynamicProgram.ipynb`**: **Unbounded Knapsack Problem.** Solving the knapsack problem using a Bottom-Up Dynamic Programming approach.

---

## Project Overviews

### Lab 1: Hybrid Sorting Algorithm
This project implements a hybrid of Merge Sort and Insertion Sort. The algorithm switches to Insertion Sort when the subarray size is less than or equal to a threshold $S$.
*   **Key Objective:** Determine the optimal $S$ that minimizes key comparisons and CPU time for input sizes up to 10 million.
*   **Result:** Empirical results validate the $O(n \log n)$ complexity while showing significant real-world speedups on small subarrays due to lower overhead.

### Lab 2: Dijkstra’s Algorithm Performance
An exploration of how graph representation and priority queue selection affect the performance of Dijkstra's algorithm.
*   **Implementation A:** Adjacency Matrix + Array PQ — $O(V^2)$.
*   **Implementation B:** Adjacency List + Binary Heap — $O((V+E) \log V)$.
*   **Analysis:** Comparison across varying edge densities (Sparse to Dense) to identify the crossover point where one implementation outperforms the other.

### Lab 3: Unbounded Knapsack (Dynamic Programming)
Implementation of the Unbounded Knapsack problem using Dynamic Programming.
*   **Features:** Recursive definition, subproblem dependency graph visualization, and an iterative Bottom-Up solution.
*   **Efficiency:** $O(n \times C)$ time complexity and $O(C)$ space complexity.

---

## 🚀 How to Run

Since these projects are provided as **Jupyter Notebooks (`.ipynb`)**, you can run them using one of the following methods:

### Option 1: VS Code (Recommended)
1.  Install the **Jupyter** extension in VS Code.
2.  Open any `.ipynb` file from the `lab` folders.
3.  Select your Python kernel (top right) and click **Run All**.

### Option 2: Jupyter Lab / Notebook
1.  Install Jupyter:
    ```bash
    pip install jupyterlab
    ```
2.  Launch the interface:
    ```bash
    jupyter lab
    ```
3.  Navigate to the desired notebook and run the cells sequentially.

### Option 3: Google Colab
1.  Upload the `.ipynb` file to [Google Colab](https://colab.research.google.com/).
2.  Run the cells in the cloud environment.

---

## Requirements
The following Python libraries are required to view the plots and run the analyses:

```bash
pip install matplotlib numpy
```

*   **NumPy**: Used for data generation and array manipulations.
*   **Matplotlib**: Used for generating the empirical analysis graphs (log-log plots, runtime comparisons).
