# AVL-slides.md

# Rotating Binary Search Trees — Slides Deck

**Build instructions**  
1. Open the sample deck: https://docs.google.com/presentation/d/1dNxjecHEiY9uJ2qs7a1nnK_2UZaYBDG5IzOfCwPLHP4/edit?usp=drivesdk  
2. File → Make a copy  
3. Replace every slide’s content with the outline below  
4. Keep 100% of the original theme, master layout, fonts, colors, footer, transitions, and diagram style  
5. Use the linked visualizers to create or screenshot tree diagrams (embed as images)  
6. Speaker notes copied verbatim where provided

### Slide 1 — Title
**Title:** Rotating Binary Search Trees  
**Subtitle:** Self-balancing with rotations — AVL & Splay  
**Your Name • February 18, 2026**  
Visual: side-by-side balanced vs degenerate tree (use mermaid export or screenshot)  
Speaker note: “Today we fix the #1 reason BSTs go bad in real code.”

### Slide 2 — Agenda
- 0–5 Hook & review  
- 5–20 Rotations  
- 20–35 AVL trees  
- 35–45 Splay trees  
- 45–50 Comparison & homework  

### Slide 3 — The Problem (Hook)
Image: 10-node right-skew tree (1→10)  
Text: “Search for 10 is now O(n). We need O(log n) always.”  
Speaker note: Ask class “What input order kills a BST?”

### Slide 4 — Rotation Intuition
“Rotations preserve BST order while changing shape.”  
Two animated diagrams (before/after) — right rotation on node 2 in 1-2-3 tree.  
Speaker note: “Think of it as rotating a mobile — nothing falls out of sorted order.”

### Slide 5 — Right Rotation Mechanics
Code-like pseudocode + before/after tree diagrams.  

```pseudocode
right_rotate(X):
  Y = X.left
  X.left = Y.right
  Y.right = X
  return Y
```
Speaker note: Walk through pointers step-by-step.

### Slide 6 — Left Rotation (symmetric)
Mirror of previous slide.

### Slide 7 — Rotation Practice (activity slide)
Three small trees on left.  
“Rotate each on your Jamboard — 3 minutes.”  
Speaker note: Call on students live.

### Slide 8 — AVL Trees — Balance Rule
Every node: |h(left) – h(right)| ≤ 1  
Store `height` field.  
Visual: height numbers on nodes.

### Slide 9 — The Four AVL Cases
Four quadrants, each with:
- LL → single right rotate  
- RR → single left rotate  
- LR → left-then-right  
- RL → right-then-left  
(Use four small before/after pairs — copy from USF or Vaidehi drawings)

### Slide 10 — AVL Insert Walkthrough
Step-by-step animation (or 4 slides merged) of inserting 10,20,30,25 → triggers LR double rotation.  
Speaker note: “This is the moment rotations save us.”

### Slide 11 — AVL Live Demo
QR code + link: https://www.cs.usfca.edu/~galles/visualization/AVLtree.html  
“Everyone open and follow along.”

### Slide 12 — Splay Trees — No Balance Bookkeeping
“On every access, splay the node to root.”  
Zig / Zig-Zig / Zig-Zag diagrams.  
Speaker note: “Recently used keys bubble to root for free.”

### Slide 13 — Splay Example
Sequence: search 5, search 5 again, search 9.  
Show tree shape change (screenshots from USF Splay viz).

### Slide 14 — Splay Live Demo
Link: https://www.cs.usfca.edu/~galles/visualization/SplayTree.html  
“Try repeated searches — watch amortization in action.”

### Slide 15 — AVL vs Splay Comparison Table
(Exact table from lesson plan above)  
Speaker note: “AVL = predictable, Splay = locality wins.”

### Slide 16 — Real-World Usage
- AVL: databases needing strict worst-case  
- Splay: caches, compilers, OS kernels  
- Next week: Red-Black (color + rotations)

### Slide 17 — Homework
1. Read BaseCS AVL article  
2. Screenshot one double rotation from VisuAlgo  
3. (Stretch) Finish AVL insert starter code  
Link to starter in chat.

### Slide 18 — Thank You + Q&A
Big tree diagram (balanced AVL).  
“See you next class — rotations are now in your toolbox.”

**End of deck.**  
Total: 18 slides — matches sample length and pacing. All diagrams and links ready. Duplicate the sample now and you’ll have the deck live in <10 minutes.