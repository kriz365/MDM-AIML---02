# Practical 02: Performance Evaluation of Search Algorithm Paradigms

Repository for TY B.Tech. Artificial Intelligence and Machine Learning (AIML) Practical Assignment 02.

## Student Details

* **Student Name:** Ritkriti Singh

* **PRN:** `202401100017`

* **Branch:** Computer Science (Software Engineering)

* **Division / Batch:** A/A4

* **Roll No:** 18

* **Date of Submission:** 26-09-2026

* **Faculty Name:** Mr. Khushal Khairnar

## Objective

To evaluate and compare the performance of four major AI search paradigms:

1. **Uninformed Search:** Breadth-First Search (BFS) & Depth-First Search (DFS) on graph navigation.

2. **Informed Search:** $A^*$ Search & Greedy Best-First Search (GBFS) using Manhattan Distance on the 8-Puzzle.

3. **Local Search:** Hill Climbing with Restarts & Simulated Annealing on the 8-Queens problem.

4. **Constraint Satisfaction Problem (CSP):** Backtracking with Minimum Remaining Values (MRV) heuristic on the Australia Map 3-Coloring problem.

## Repository Structure

```
MDM-AIML-02/
│
├── search_algorithms_benchmark.py   # Complete executable script containing all 4 search paradigms
├── requirements.txt                 # Dependencies and package requirements
├── README.md                        # Repository documentation
└── results/                         # Benchmark terminal output and performance plots

```

## Technology / Tools Used

* **Programming Language:** Python 3.x

* **Platform / IDE:** Google Colab / Local Python Environment

* **Libraries/Packages:** `NumPy`, `Matplotlib`, `collections`, `heapq`

## Installation & Execution

1. Clone the repository:

   ```
   git clone https://github.com/aniche59/MDM-AIML-02.git
   cd MDM-AIML-02
   
   ```

2. Install dependencies:

   ```
   pip install -r requirements.txt
   
   ```

3. Run the benchmark script:

   ```
   python search_algorithms_benchmark.py
   
   ```

## Test Cases & Results Summary

| Test Case | Input | Expected Output | Actual Output | Status | 
 | ----- | ----- | ----- | ----- | ----- | 
| **Uninformed Search** | Graph Navigation (A -> GOAL) | BFS path cost optimal (Cost=11) | BFS Cost = 11, DFS Cost = 20 | **Pass** | 
| **Informed Search** | 8-Puzzle Manhattan Heuristic | $A^*$ optimal depth & low node expansion | $A^*$ Depth=2, Nodes=3 | **Pass** | 
| **Local Search** | 8-Queens Configuration | Minimize conflicts to 0 | HC Conflicts=0, SA Conflicts=1 | **Pass** | 
| **CSP Search** | Australia Map 3-Coloring | Valid 3-coloring with 0 backtracks | Backtracks=0, Checks=23 | **Pass** | 

## Conclusion

Empirical evaluations confirm that heuristic-guided search paradigms ($A^*$) and constraint propagation techniques (MRV) provide superior computational efficiency, optimal path costs, and drastically reduced node expansions compared to uninformed search strategies.