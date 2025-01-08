### Reflection: Lessons Learned and Areas for Improvement

During the completion of this project, I identified several areas where I can improve and streamline my workflow for future projects. Here’s a summary of key takeaways:

---

#### **1. Aligning Separate Containers**
In this project, I used separate containers for the navigation bar and hero section. While this approach keeps the code modular and organized, I faced challenges aligning their content horizontally.

**Improvement for Future Projects:**
- Ensure consistent **padding** or use a **shared wrapper** to maintain alignment across sections.
- Example:
  ```css
  .header, .hero-section {
    padding: 0 32px; /* Consistent padding */
  }
  ```
  Or:
  ```html
  <div class="main-wrapper">
    <div class="header">...</div>
    <div class="hero-section">...</div>
  </div>
  ```
  ```css
  .main-wrapper {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 32px;
  }
  ```

---

#### **2. Simplifying CSS**
I wrote more CSS than others, primarily because the task had specific styling requirements. While my CSS was well-organized and documented, I could improve by leveraging reusable utility classes and global styles for common elements.

**Improvement for Future Projects:**
- Use utility classes for frequently used styles like alignment and buttons.
- Normalize text styles globally to reduce repetition.
- Example:
  ```css
  /* Utility Classes */
  .text-center {
    text-align: center;
  }
  .btn-primary {
    padding: 12px 24px;
    background-color: #2979ff;
    color: white;
    border: none;
    border-radius: 4px;
  }

  /* Global Text Styles */
  h1, h2, p {
    font-family: 'Roboto', sans-serif;
    margin: 0;
  }
  ```

---

#### **3. Debugging Font Import**
I successfully imported the Roboto font and verified it was being used via browser DevTools. This task reinforced my understanding of font integration and debugging.

**Improvement for Future Projects:**
- Expand my knowledge of font weights and proper importing techniques for flexibility.
- Example:
  ```html
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  ```

---

#### **4. Planning for Reusability**
While the project requirements dictated specific styles, I learned the importance of identifying opportunities for reusable components and utility classes. This will reduce future CSS code duplication.

**Improvement for Future Projects:**
- Identify repetitive patterns early and abstract them into reusable styles.
- Example:
  ```css
  .card {
    border: 1px solid #eee;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  ```

---

### Final Thoughts
This project was a valuable learning experience. I navigated challenges in alignment, organisation, and styling while reinforcing my understanding of **Flexbox** and font integration. Moving forward, I’ll continue refining my approach to reusable styles, alignment consistency, and layout planning to create cleaner and more maintainable projects.
