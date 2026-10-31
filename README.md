# DAA - Greedy Algorithms (C Implementations)

This repository contains C implementations of classic **Greedy Algorithm** problems commonly studied in **Design and Analysis of Algorithms (DAA)**.

## 📌 Problem Overview

| # | File Name | Problem Name | Greedy Strategy | Time Complexity |
|---|---|---|---|---|
| 1 | `1-G-Coin Problem` | Indian Coin Change Problem | Always pick the largest denomination note/coin $\le V$ | $\mathcal{O}(D)$ where $D$ is denomination count |
| 2 | `2-G-Burger Problem` | Burger / Calorie Minimization | Sort items in descending order to minimize power multiplier | $\mathcal{O}(N \log N)$ |
| 3 | `2-G-Cookies Problem` | Assign Cookies | Sort greed factors and cookie sizes; assign smallest possible valid cookie | $\mathcal{O}(N^2 + M^2)$ (Bubble Sort) / $\mathcal{O}(N \log N + M \log M)$ |
| 4 | `4-G-Array Sum max problem` | Maximize $\sum (A[i] \times i)$ | Sort array in ascending order to pair larger numbers with larger indices | $\mathcal{O}(N \log N)$ |
| 5 | `5-G-Product of Array elements-Minimum` | Min Product of Two Arrays | Sort array $A$ ascending and array $B$ descending to pair max with min | $\mathcal{O}(N \log N)$ |

---

## 📖 Problem Details

### 1. Coin Change Problem (`1-G-Coin Problem`)
- **Objective:** Find the minimum number of currency notes needed to make an amount $V$.
- **Denominations:** `{1000, 500, 100, 50, 20, 10, 5, 2, 1}`
- **Approach:** Iteratively divide the remaining amount by the largest available denomination and update the remainder.

### 2. Burger Problem (`2-G-Burger Problem`)
- **Objective:** Given calorie values for $n$ burgers, minimize the total effort calculated as $\sum_{i=0}^{n-1} (\text{calorie}_i \times 3^i)$.
- **Approach:** Eat higher calorie burgers first (sorted descending) so they are multiplied by smaller powers of 3 ($3^0, 3^1, 3^2, \dots$).

### 3. Cookies Problem (`2-G-Cookies Problem`)
- **Objective:** Maximize the number of satisfied children given greed factors $g$ and cookie sizes $s$.
- **Approach:** Sort both arrays; satisfy children with the smallest possible cookie that meets or exceeds their greed factor.

### 4. Array Sum Max Problem (`4-G-Array Sum max problem`)
- **Objective:** Maximize the sum $\sum_{i=0}^{n-1} (A[i] \times i)$ after rearranging elements.
- **Approach:** Sort array in non-decreasing order so higher values get multiplied by larger index weights.

### 5. Minimum Product of Two Arrays (`5-G-Product of Array elements-Minimum`)
- **Objective:** Given two arrays $A$ and $B$, rearrange them to minimize $\sum (A[i] \times B[i])$.
- **Approach:** Sort one array in ascending order and the other in descending order to pair the largest values of one with the smallest of the other.

---

## 🚀 How to Run

Compile and run any solution using GCC (or Clang):

```bash
# Example: Compile Burger Problem
gcc "2-G-Burger Problem" -o burger

# Run executable
./burger
```

---

## 📱 Quick Access (QR Code)

Scan the QR code below to access this repository directly on your mobile device:

<div align="center">
  <img src="./repo-qr.png" alt="Repository QR Code" width="180"/>
  <br/>
  <sub><b>https://github.com/Sanjay-AI-ML/DAA-GREEDY-ALGORITHM</b></sub>
</div>

---

## 👤 Author
- **Sanjay R** ([@Sanjay-AI-ML](https://github.com/Sanjay-AI-ML))
