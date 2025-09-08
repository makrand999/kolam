# Kolam  

Kolam is a Tamil word for **Rangoli**, a traditional decorative art drawn on the ground, usually with rice flour, chalk powder, or rock powder.  
It is widely practiced in Tamil Nadu and other South Indian states, especially in front of homes during festivals and daily rituals.  

---

## Types of Kolams (based on rules)  

### 1. **Pulli Kolam (Dot Kolam)**  
- Constructed by placing a grid of dots (*pulli*) and then connecting the dots using straight or curved lines.  
- The arrangement of dots determines the structure of the kolam.  
- Often used for simple geometric or floral designs.  
- Example: Grids like 5×5, 7×7 dots are popular.  
![pulli kolam](https://www.google.com/url?sa=i&url=https%3A%2F%2Fin.pinterest.com%2Fpin%2F19-dots-sikku-fusion-kolambig-kolams--73605775150777740%2F&psig=AOvVaw1wGYNbmbdnRGR6vZfJDnRu&ust=1757436755269000&source=images&cd=vfe&opi=89978449&ved=0CBUQjRxqFwoTCKi15qLQyY8DFQAAAAAdAAAAABAE)  

### 2. **Sikku Kolam (Twisted Kolam)**  
- Lines and curves weave around the dots without crossing them.  
- Usually drawn in a single continuous stroke, forming loops and knots.  
- Represents infinity or unbroken continuity, symbolizing prosperity.  
- *(Insert photos here)*  

---

## L-System and Kolams  

### What is an L-System?  
- An **L-System (Lindenmayer System)** is a mathematical formalism originally developed to describe plant growth.  
- It generates complex patterns using simple rewriting rules.  
- Consists of:  
  - **Axiom (start string):** Initial state.  
  - **Production rules:** How symbols are replaced.  
  - **Iterations:** Repeatedly apply rules to grow the pattern.  

### Example Kolam with L-System  

**Rules:**  
- Axiom: `F`  
- Production: `F → F+F−F−F+F`  
- Angle: 90°  

Where:  
- `F` = move forward and draw a line  
- `+` = turn right  
- `-` = turn left  

After a few iterations, this produces a square-like fractal that resembles a kolam pattern.  

---
 
## General Ways of Coding Kolams  

### 1. **L-System Coding**  
- Define an axiom, production rules, and turning angles.  
- Use iterations to expand complexity.  
- Common for generating **fractal-like kolams**.  

### 2. **Sequential Encoding (from Waring, 2012)**  
- Square Loop Kolams (SLK) can be represented as sequences of **gestures** (building blocks of strokes).  
- These gestures start and end at fundamental positions between or around dots.  
- Gestures are grouped into four sets:  
  1. **Orthogonal gestures (O):** move around dots along grid edges.  
  2. **Diagonal gestures (D):** move around dots at diagonal positions.  
  3. **Transitional gestures (T):** connect orthogonal and diagonal gestures.  
  4. **Stylistic gestures (C, H, P):** decorative variations like circles, horns, points.  
- Each gesture is encoded with a symbol (e.g., O1, D2R, H3L).  

**Example:**  
- A simple 3×3 orthogonal kolam could be encoded as:
- [O1 O3 O4 O1] x 4
- Meaning one loop is drawn with gestures O1, O3, O4, O1, repeated 4 times symmetrically.  

- A diagonal kolam example might be:  
- [D4R D4R D4R D2R D2R] x 4
- This sequential language provides a **modular way to encode and reproduce kolams**, similar to a recipe.  
[reference](https://www.researchgate.net/profile/Timothy-Waring-2/publication/234116828_Sequential_Encoding_of_Tamil_Kolam_Patterns/links/09e4150f560aaedbf2000000/Sequential-Encoding-of-Tamil-Kolam-Patterns.pdf)
---

## Symmetries in Kolams  

Kolams often display **geometric symmetries**, which give them aesthetic balance.  

1. **Reflection Symmetry (Mirror Symmetry)**  
   - Kolam looks the same when reflected across a vertical or horizontal axis.  
   - Example: A star kolam mirrored across its center line.  

2. **Rotational Symmetry**  
   - The kolam appears unchanged after rotation (commonly 90°, 180°, or 360°).  
   - Example: Circular kolams repeated around a central point.  

3. **Translational Symmetry**  
   - A motif is repeated by shifting in space without rotation.  
   - Example: Borders made of repeating kolam units.  

4. **Glide Reflection Symmetry**  
   - Combination of reflection and translation.  
   - Example: A kolam motif mirrored and shifted along a line.  

5. **Radial Symmetry**  
   - Patterns radiate outward from a central point.  
   - Example: Floral kolams with petals extending around a dot grid.  

6. **Fractal Symmetry**  
   - Self-similar repeating patterns at different scales, often generated using L-Systems.  
   - Example: Recursive kolams where small motifs form larger motifs.  

---

 
