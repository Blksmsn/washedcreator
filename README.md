# Washed Creator Website Documentation

## Introduction
The **Washed Creator** website is designed to showcase high-quality short-form content services and creative solutions. This document provides an overview of the code structure, styling guidelines, form functionality, technologies used, and deployment guidelines.

---

## Project Structure
The project follows a structured format to ensure maintainability and scalability.

```
/washedcreator
│── index.html             # Main landing page
│── styles.css             # Global stylesheet for the website
│── script.js              # JavaScript functionality for interactive elements
│── /assets                # Contains images, icons, and other media files
│── /fonts                 # Custom font files used throughout the website
│── /components            # Reusable HTML sections like header and footer
│── /config                # Configuration files related to the project
│── /contact               # Contact form handling files
│── /portfolio             # Portfolio showcase section
│── README.md              # Project documentation
```

---

## Technologies Used
The following technologies and tools were used to develop the Washed Creator website:

- **HTML5** - Structuring the web pages
- **CSS3** - Styling and layout design
- **JavaScript (ES6+)** - Adding interactivity
- **Google Fonts** - Custom typography for branding consistency
- **GitHub Pages** - Hosting the static website

---

## CSS Styling Standards
The website follows a **consistent branding and design language**. Here are the key styling conventions:

### Typography:
- **Headings (H1, H2, H3):** Space Mono, bold.
- **Body text:** Lekton, regular.
- **Button Text:** Uppercase, Space Mono.

### Color Scheme:
- **Primary Color:** American Yellow `#EAB003`
- **Secondary Color:** Charcoal `#333333`
- **Background Color:** Off-White `#F5F5F5`
- **Text Color:** Black `#000000`

### Layout & Spacing:
- Uses **CSS Flexbox & Grid** for responsive design.
- Maintains **consistent padding/margin** for a clean, structured look.

---

## Form Functions
The **contact form** handles user inquiries and submits data via JavaScript.

### Features:
- **Validation:** Checks for required fields before submission.
- **AJAX Submission:** Prevents page reload on submit.
- **Error Handling:** Displays error messages for invalid inputs.

### Code Snippet (JavaScript Example):
```js
document.getElementById("contact-form").addEventListener("submit", function(event) {
    event.preventDefault();
    let name = document.getElementById("name").value;
    let email = document.getElementById("email").value;
    if (name === "" || email === "") {
        alert("Please fill in all required fields.");
    } else {
        alert("Form submitted successfully!");
    }
});
```

---

## Deployment Instructions
To deploy or update the website, follow these steps:

1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-repo/washedcreator.git
   ```

2. **Navigate to the Project Directory**
   ```sh
   cd washedcreator
   ```

3. **Open `index.html` in a browser** to preview the site locally.

4. **Commit and push changes** to update the live version on GitHub Pages.
   ```sh
   git add .
   git commit -m "Updated website content"
   git push origin main
   ```

---

## Future Enhancements
- Implement a CMS for easier content updates.
- Add blog functionality for additional content marketing.
- Integrate analytics for performance tracking.

---

For any questions or further modifications, please refer to the repository or contact the development team.



