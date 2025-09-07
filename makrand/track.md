# Research Notes on Kolams  

## 6/9 – Initial Research and Observations  

- **Explored Research Papers:**  
  - Found two main approaches to representing Kolams mathematically:  
    1. **Lattice & Angle Representation** → [Reference Paper](https://ar5iv.labs.arxiv.org/html/2307.02144)  
    2. **Graph Representation (Graph Data Structures)**  
    3. (A third method exists but is less useful)  

- **Current Focus of Research Papers:**  
  - Most existing works emphasize **algorithmic or mathematical representations** of Kolams.  
  - They typically stop at **converting Kolams into computer-drawable forms** using lattices, angles, or graphs.  

- **Our Goal (Beyond Computer Drawing):**  
  - Instead of just drawing Kolams computationally, we want to **draw them in a mathematical way**.  
  - Meaning:  
    - Given a Kolam, we identify **all types of symmetries** and **other structural properties** (e.g., overlapping knots).  
    - Then, **remove the symmetries** step by step until we reach the **base unit design** (a fundamental part of the Kolam with no symmetries or properties).  
      - ⚠️ Note: Even the smallest unit design follows **traditional Kolam rules** (so it’s not entirely random).  
    - Finally, we **reconstruct the full Kolam** by reapplying the removed symmetries sequentially.  

- **Why This Approach Matters:**  
  - It allows us to show **mathematical steps** in Kolam creation.  
  - We can also demonstrate the process visually through **animation/frames**.  

---

## Key Observations  

1. **Types of Kolams:**  
   - There are multiple variations, each with its own **symmetries** and **rules**.  
   - First step → **Categorize all Kolams** and **list their properties**.  

2. **Knots and Overlaps:**  
   - A **knot** = A closed loop formed when starting and ending a curve at the same point.  
   - Kolams can have **multiple knots** that overlap.  
   - Overlapping knots form another type of **symmetry/pattern**.  
   - Idea:  
     - If two knots overlap, we can animate them using **speed-based drawing**.  
     - By adjusting the **starting points** and **drawing speed**, we can simulate their overlaps mathematically.  

---

## 7/9 – Next Goal  

- **Differentiate and Categorize Kolams**:  
  - Identify all Kolam types.  
  - Define their **properties**, **symmetries**, and **rules**.  
