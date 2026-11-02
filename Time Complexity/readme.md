# ⏱️ Master Time Complexity Analysis

Calculating time complexity allows you to measure how the runtime of your algorithm grows relative to the input size ($n$). Follow this structured guide and cheat sheet to analyze code efficiently.

---

## 📐 Core Rules of Big O Notation

When determining the final complexity, always apply this fundamental rule:
> **Ignore constants and lower-order terms.** 

### Mathematical Example:
$$\mathcal{O}(3n^2 + 5n + 10) \longrightarrow \mathcal{O}(n^2)$$
* *Why?* As $n$ grows toward infinity, the $n^2$ term dominates the runtime. Constants (like $3$) and lower-order terms (like $5n$ and $10$) become insignificant.

---

## 📑 Java Code Pattern Cheat Sheet

| Java Code Pattern | Time Complexity | Growth Classification |
| :--- | :--- | :--- |
| **Single statement** (e.g., `int x = 1 + 2;`) | $\mathcal{O}(1)$ | Constant Time |
| **Loop dividing by 2** (e.g., binary search structures) | $\mathcal{O}(\log n)$ | Logarithmic Time |
| **One loop** running $n$ times | $\mathcal{O}(n)$ | Linear Time |
| **Two separate loops** running sequentially | $\mathcal{O}(n + n) = \mathcal{O}(n)$ | Linear Time |
| **Nested loop plus a single loop** | $\mathcal{O}(n^2 + n) = \mathcal{O}(n^2)$ | Quadratic Time |
| **Two nested loops** | $\mathcal{O}(n^2)$ | Quadratic Time |
| **Three nested loops** | $\mathcal{O}(n^3)$ | Cubic Time |

---

## 🔍 How to Analyze Any Block of Code

1. **Break it down:** Look at your code line by line and identify the independent blocks or loops.
2. **Assign complexity to each part:** Use the cheat sheet above to map code structures to their individual Big O values.
3. **Combine the blocks:** 
   * If code blocks run **one after another**, *add* their complexities together.
   * If code blocks are **nested**, *multiply* their complexities together.
4. **Simplify:** Drop the coefficients and keep only the fastest-growing term.
