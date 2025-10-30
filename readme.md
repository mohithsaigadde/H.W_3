# Dynamic Multiplication Table
*A web application that generates an interactive multiplication table based on user input.*

---

##  Overview
This project creates a **dynamic multiplication table** where users can input horizontal and vertical integer ranges (between −50 and 50) and instantly view a computed table of products.  
It demonstrates client-side form validation, DOM manipulation, and responsive table design using **HTML**, **CSS**, and **JavaScript**.

---

##  File Structure
| File | Description |
|------|--------------|
| `m.html` | Main HTML file containing page structure, form elements, and embedded JavaScript logic |
| `style.css` | External stylesheet defining layout, spacing, and color theme |
| `README.md` | Project documentation and usage guide |

---

##  Features
-  User input for horizontal and vertical numeric ranges  
-  Real-time validation with helpful error messages  
-  Prevents invalid input (e.g., start > end or values outside −50..50)  
-  Automatically generates a clean, scrollable table  
-  Sticky header and left column for easy viewing  
-  Clear button to reset fields and output instantly  
-  Fully responsive card-style layout  

---

##  How to Run
1. Download both files:
   ```
   m.html
   style.css
   ```
2. Keep them in the **same folder**.  
3. Open `m.html` in any modern web browser (Chrome, Edge, Firefox, Safari).  
4. Enter integer ranges and click **“Generate Table”**.  
5. Use **“Clear”** to reset all inputs and remove the table.

---

##  How It Works
1. The user enters four integer values:
   - Horizontal start (`hStart`)
   - Horizontal end (`hEnd`)
   - Vertical start (`vStart`)
   - Vertical end (`vEnd`)
2. JavaScript validates:
   - All are integers  
   - Start ≤ End for both axes  
   - Range is within −50 to 50  
   - Table cell count ≤ 10,000  
3. If valid, a `<table>` is dynamically built in the DOM with:
   - Top row: horizontal multipliers  
   - Left column: vertical multiplicands  
   - Body: multiplication results (`x * y`)  
4. If invalid, the system displays a red error message under the form.

---

##  Input / Output Example

**Input:**
```
Horizontal start: 1
Horizontal end: 5
Vertical start: 5
Vertical end: 8
```

**Output Table:**

| × | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| 5 | 5 | 10 | 15 | 20 | 25 |
| 6 | 6 | 12 | 18 | 24 | 30 |
| 7 | 7 | 14 | 21 | 28 | 35 |
| 8 | 8 | 16 | 24 | 32 | 40 |

---

##  Design & Styling
- **Layout:** Card-based container with soft shadows and padding  
- **Grid System:** 4-column form layout using CSS Grid  
- **Colors:** Light neutral background (`#f2f6fa`) with teal and gray accents  
- **Sticky Headers:** Both row and column headers stay visible when scrolling  
- **Responsive Design:** Automatically fits different screen sizes (desktop/laptop/tablet)

---

##  Dependencies
No external libraries required — works entirely with:
- **HTML5**
- **CSS3**
- **Vanilla JavaScript (ES6)**

---

##  Known Issues / Limitations
- Large input ranges (close to 100×100) may slow rendering slightly.
- Table resets completely when cleared (no undo).

---

##  Author
**Name:** Mohith Sai Gadde  
**Course:** COMP.4610 — GUI Programming I  
**Instructor:** Prof.Wenjin Zhou  
**Institution:** University of Massachusetts Lowell  
**Semester:** Fall 2025  

---

##  License
This project is created for educational purposes.  
Free to use and modify with proper credit to the author.

---

##  Acknowledgements
- HTML/CSS structure inspired by standard web form layouts  
- JavaScript validation and dynamic DOM rendering written from scratch for this assignment
