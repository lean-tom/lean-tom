# Hi, I'm lean-tom! 👋

I am a mathematics enthusiast and formal verification engineer dedicated to bridging high-level mathematical intuition with machine-checked rigor. I focus on the formalization of complex mathematical problems using **Lean 4**.

Currently, I am a lead contributor to the **[dwrensha/compfiles](https://github.com/dwrensha/compfiles)** project, formalizing olympiad-level challenges to push the boundaries of what is possible in automated reasoning.

---

## 💎 Featured Project: IMO 2025 Problem 6 (The Matilda Problem)
**[World's First Complete Formalization without `sorry`]**

I have successfully formalized the complete solution for the most notorious problem of IMO 2025. This project involves **~4,700 lines of verified Lean 4 logic**, making it a benchmark for managing extreme complexity in formal systems.

### 🛠️ Technical Innovations

#### 1. Lower Bound (Necessity - Topological Combinatorics)
We established the lower bound $n + 2\sqrt{n} - 3$ by applying the **Erdős–Szekeres Theorem** through a novel topological lens:
- **Set-Theoretic Topological Partitioning**: Replaced error-prone analytic boundary step functions with discrete set intervals (unions/intersections). This eliminated manual `max`/`min` casework at the boundaries where LIS/LDS relations shift.
- **Topological Pivot Strategy**: Engineered a "topological pivot" region to resolve the "Disjoint Case," allowing identification of pivot properties without explicit analytic intersection coordinates.
- **Boundary Filtering**: Implemented systematic filtering ($0 < x < k^2-1$) to handle grid edges, removing "out-of-bounds" labels and ensuring the formal count matches the upper bound perfectly.

#### 2. Upper Bound (Sufficiency - Elementary Number Theory)
For the $n=k^2$ case, I developed an original explicit construction:
- **Index-Based Fiber Construction**: Defined integer forms $val\_s(p)$ and $val\_t(p)$ to partition the grid into disjoint fibers using Gaussian brackets.
- **Lattice-Point Congruence**: Identified black squares as lattice points where $val\_s, val\_t \equiv 0 \pmod{k^2+1}$.
- **Geometric Verification**: Formally verified that each Matilda tile corresponds to a $k \times k$ square, resulting in exactly $k^2 + 2k - 3$ tiles covering all white squares.

### 📈 Status & Engineering Excellence
- **Verified**: `lake build` completed successfully (1994 jobs) with zero errors.
- **Up-to-date**: Fully compatible with **Lean v4.28.0-rc1** and the latest **Mathlib** standards (Pairwise, Std.Refl, etc.).
- **Human-AI Symbiosis**: This proof was architected by me and implemented in collaboration with **Gemini 3 Pro**. I performed the rigorous decomposition into granular lemmas, while the AI assisted in implementation and tactical bridging.

---

## 🟢 Other Notable Formalizations

- **IMO 1999 P3**  Combinatorics
- **IMO 1986 P3**  Combinatorics
- **IMO 1971 P6**  Combinatorics
- **IMO 1968 P6**  Nuber Theory
- **IMO 1961 P2**  Weitzenböck’s Inequality 

---

## 🧩 Technical Outlook & Interests

- **Scalable AI Reasoning**: I am exploring how extreme-scale formalizations (like my 4,700-line Matilda proof) can serve as "Ground Truth" data for the next generation of reasoning-capable LLMs.
- **AI-Assisted Formal Engineering**: Developing workflows where human mathematical architecture guides AI-driven implementation to achieve machine-checked rigor at scale.
- **Proof Visualization**: Utilizing **Lean Blueprints** to map and manage dependency graphs of large-scale formal proofs.

---

*"Mathematics is not about numbers, equations, computations, or algorithms: it is about understanding." — William Paul Thurston*
