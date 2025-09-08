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
- *(Insert photos here)*  

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

## General Way of Coding Kolams  

1. **Define the axiom (seed):** starting symbol (e.g., `F`).  
2. **Define production rules:** specify how each symbol expands.  
3. **Choose the turning angle:** e.g., 90°, 45°, 60°, depending on the geometry.  
4. **Set the number of iterations:** higher iterations = more complexity.  
5. **Render the drawing:** interpret symbols as drawing commands.  

This allows kolams to be generated programmatically while preserving their traditional structure.  

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

 
