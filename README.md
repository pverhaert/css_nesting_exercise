# CSS Nesting Exercise 🌱

## Overview
In this exercise, you'll learn to use native CSS nesting to transform a standard CSS file into a more maintainable and organized structure. You'll work with a complete website layout featuring navigation, cards, and interactive elements, refactoring the CSS to use modern nesting techniques.

## Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/Vince-Colson-TM/css_nesting_exercise.git
   ```
2. Open `index.html` in your browser
3. Review the current `styles.css` file structure

## Part 1: Navigation Component
### Task
Refactor the navigation styles using CSS nesting.

### Requirements
- Nest all navigation-related styles within the `.nav` selector
- Move the mobile menu media query into the relevant nested structure
- Maintain the hover state for navigation links

### Example of CSS Nesting
```css
/* Simple nesting example */
.parent {
    color: blue;
    
    .child {
        color: red;
        
        &:hover {
            color: green;
        }
    }
}
```

## Part 2: Button Components
### Task
Refactor button styles to use nesting for variants and states.

### Requirements
- Nest primary and secondary button styles within the main button class
- Add hover and focus states using nesting
- Include transition effects for smooth state changes

### Example of State Nesting
```css
.element {
    background: white;
    
    &:hover {
        background: gray;
    }
    
    &.variant {
        /* Variant styles ( class="element variant" )*/
    }
}
```

## Part 3: Card Component
### Task
Refactor the card component using CSS nesting.

### Requirements
- Nest all card-related styles within the main card selector
- Add hover effects for cards using nested selectors
- Use flexbox for the card layout structure
- Maintain proper spacing and typography

### Success Criteria
- Cards should maintain their current appearance
- Hover effects should work smoothly
- All styles should be properly nested
- Layout should be responsive using flexbox

## Part 4: Responsive Layout
### Task
Integrate media queries within their respective components.

### Requirements
- Nest media queries within their related components
- Ensure responsive behavior matches the original design
- Use consistent breakpoints throughout (768px and 480px)

### Example of Nested Media Queries
```css
.component {
   
   /* Base styles for mobile-first */

   @media (min-width: 480px) {
      /* Styles for screens larger than 480px (tablet and up) */
   }

   @media (min-width: 768px) {
      /* Styles for screens larger than 768px (tablet landscape and up) */
   }

   & .child {
      /* Child styles for mobile by default */

      @media (min-width: 480px) {
         /* Styles for screens larger than 480px (tablet and up) */
      }

      @media (min-width: 768px) {
         /* Styles for screens larger than 768px (tablet landscape and up) */
      }
   }
}
```

## Part 5: Footer Component (Bonus)
### Task
Create a new footer component using CSS nesting.

### Requirements
- Create a responsive footer with multiple columns
- Include hover states for links
- Use nested media queries for responsive design
- Add a bottom border and copyright section

### Example Structure
```html
<footer class="footer">
    <div class="footer-content">
        <div class="footer-section">
            <h3>About</h3>
            <ul>
                <li><a href="#">Our Story</a></li>
                <li><a href="#">Team</a></li>
            </ul>
        </div>
        <!-- Add more sections as needed -->
    </div>
</footer>
```

## ✅ Learning Outcomes
By completing this exercise, you will:  
✔ Learn **how to use native CSS nesting** for better style organization.  
✔ Understand **how to structure media queries** within relevant components.  
✔ Discover the benefits of **grouping related styles** together for readability and maintainability.  
✔ Implement **hover, focus, and active states** using nesting for clean code.  
✔ Improve the **responsiveness and maintainability** of your design with native CSS nesting. 
