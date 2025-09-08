<img width="1080" height="1080" alt="image" src="https://github.com/user-attachments/assets/18360def-4644-4460-acda-c2921704f6c7" /># Kolam  

Kolam is a Tamil word for **Rangoli**, a traditional decorative art drawn on the ground, usually with rice flour, chalk powder, or rock powder.  
It is widely practiced in Tamil Nadu and other South Indian states, especially in front of homes during festivals and daily rituals.  

---

## Types of Kolams (based on rules)  

### 1. **Pulli Kolam (Dot Kolam)**  
- Constructed by placing a grid of dots (*pulli*) and then connecting the dots using straight or curved lines.  
- The arrangement of dots determines the structure of the kolam.  
- Often used for simple geometric or floral designs.  
- Example: Grids like 5×5, 7×7 dots are popular.  
 ![pulli kolam](https://scontent.fnag4-5.fna.fbcdn.net/v/t39.30808-6/481095256_567211586365537_4910231756980644710_n.jpg?stp=dst-jpg_s1080x2048_tt6&_nc_cat=105&ccb=1-7&_nc_sid=833d8c&_nc_ohc=V5J9dqK_OxIQ7kNvwHrx44j&_nc_oc=Adm3X5UJMvjnDvxNTwS3pbiWm06x4rkBgIva6tgu_MwJ7gyWEvlRb27GQsgYEVcmdNrwNsa-TlcumZWhj5nDwTAf&_nc_zt=23&_nc_ht=scontent.fnag4-5.fna&_nc_gid=TJ26TT4lZtAbdzSvI8iN-A&oh=00_AfZLMj8yi6pSP54wB8sj3gUIJafPTmpr_TOBqXp-NdzosA&oe=68C4EFD4)
### 2. **Sikku Kolam (Twisted Kolam)**  
- Lines and curves weave around the dots without crossing them.  
- Usually drawn in a single continuous stroke, forming loops and knots.  
- Represents infinity or unbroken continuity, symbolizing prosperity.  
![sikku kolam](https://scontent.fnag4-1.fna.fbcdn.net/v/t39.30808-6/471442349_971997481409555_3846218596965428532_n.jpg?stp=dst-jpg_p526x296_tt6&_nc_cat=102&ccb=1-7&_nc_sid=127cfc&_nc_ohc=RB1eNQeK1RoQ7kNvwG0brXE&_nc_oc=Adk3x3DGlud4F43OE5oRz3MS0_OUBJM9fVdk8w66JF_91JC8tsY9BUd5qFoE18FKFA2jdOZRf4nvqCRvURQiN3uf&_nc_zt=23&_nc_ht=scontent.fnag4-1.fna&_nc_gid=GfSilGzRWWC4KMlIPz1lrQ&oh=00_Afbbn59rzF5MSHgmuKG1oBF7tFtAGX3NipOy9nbj6M2dZQ&oe=68C4CF92)  

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

 
