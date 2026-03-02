# HoverPage 🎓  

This is a personal desktop-based UI project I built to practice advanced hover effects and layered interaction behavior using only **HTML and CSS**.  

The page is titled **Result Room** and displays semester results inside a structured card layout.  

Instead of keeping everything static, I wanted the interface to feel responsive to user interaction without writing a single line of JavaScript. The main goal was to experiment with **transform effects, smooth transitions, hover chaining, element targeting, and visibility control** purely through CSS.

This project is intentionally designed for **desktop view only** and does not include responsive behavior.

---

## 🧠 The Concept Behind It  

Rather than designing a simple result layout, I focused on interaction flow.

When the user hovers over the **main container**, all semester cards shrink slightly. This creates a background reaction effect, making the UI feel alive and layered instead of flat.

Then, when hovering over a specific semester card:

- The card scales up slightly  
- It rotates a little  
- The transition remains smooth and controlled  

This contrast between shrinking background cards and the active highlighted card creates a clean visual hierarchy.

Another idea I experimented with was **delayed visibility**.  

The result status — “Passed” or “Failed” — is hidden by default and only appears when the card is hovered. This keeps the design minimal while adding a subtle reveal effect.

---

## 🎨 Styling Strategy  

The layout is structured using **Flexbox**, which keeps all semester cards evenly aligned inside the main container.

Each card includes:

- Fixed width and height  
- Rounded borders  
- Consistent spacing  
- Clean background styling  

### Result Logic  

- The first three semesters are marked as **Passed**.  
  - On hover, they display a **green border**.  
  - This provides a strong and positive visual signal.  

- The fourth semester is marked as **Failed**.  
  - Instead of editing HTML, I targeted it using a position selector (`nth-child`).  
  - On hover, its border changes to a **reddish tone**.  

This small difference helped me understand how to style a specific element differently without modifying the HTML structure.

Result text colors are controlled using ID selectors:

- Passed → lighter success color  
- Failed → darker reddish tone  

This makes the outcome visually clear even before reading the text.

---

## 🔧 Key Features  

- **Container-Based Hover Effect** – Entire section reacts when hovered  
- **Layered Transform Effects** – Combination of `scale()` and `rotate()`  
- **Smooth Transitions** – Controlled timing for clean animations  
- **Selective Targeting** – Styled specific card using `nth-child`  
- **Opacity-Based Visibility Control** – Result text appears only on hover  
- **Flexbox Layout System** – Even alignment and structured spacing  

---

## 📂 Project Structure  

- `index.html` – Contains both structure and internal CSS styling  
- `MainImg.jpg` – Image used inside each semester card  
- `README.md` – Project documentation  

---

## 🖥 Desktop Preview
![Desktop View](https://github.com/omshigupta/HoverPage/blob/main/Snapshot.png)
