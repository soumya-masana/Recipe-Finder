# RECIPE FINDER

This is a simple yet powerful recipe finder application built entirely within a single HTML file. It leverages React and Tailwind CSS loaded via CDNs to create a modern, interactive user experience without requiring any build tools, package managers (like npm), or a complex development setup.

The application features a sleek, dark-themed, and responsive design, allowing users to quickly search for recipes based on a single ingredient.

# Features

**Ingredient-Based Search:** Find recipes by typing in an ingredient. (Chicken, Avocado, Egg, Broccoli, etc)

**Interactive Recipe Cards:** Browse results in a clean, responsive grid layout.

**Detailed Recipe Modal:** Click any recipe to see its image, a full ingredient list, and step-by-step instructions.

**Loading & Error States:** Clear user feedback with a loading spinner and user-friendly error messages.

**Responsive Design:**  The interface works beautifully on all screen sizes.

**Dynamic Feedback:**

- Displays a loading spinner while fetching data.

- Shows clear error messages for failed network requests.

- Provides a user-friendly message when no recipes are found for a search term.

**Resilient API Fetching:** Automatically retries a failed network request up to 3 times with an exponential backoff delay, making the app more robust against temporary network issues.

**Image Fallbacks:** Gracefully handles missing recipe images by displaying a clean placeholder instead of a broken image icon.

Zero-Build Setup: Runs instantly in any modern browser with no installation or compilation steps needed.

# How to Run
This project is designed for maximum simplicity.

**Save the Code:** Save the provided code as an index.html file.

**Open in Browser:** Open the index.html file in any modern web browser (like Chrome, Firefox, Safari, or Edge).

# How It Works: A Technical Overview
This project runs directly in the browser without any server or build process by loading all necessary libraries from a Content Delivery Network (CDN). Here’s how the pieces fit together:

**Tailwind CSS:** The entire styling is handled by the Tailwind CSS library, loaded from its CDN. It scans the class names in your HTML and applies the appropriate styles on the fly.

**React & ReactDOM:** The core React libraries are included via <script> tags, making the React and ReactDOM global variables available for use.

**Babel Standalone**: This is the key to using JSX directly in the browser. The <script type="text/babel"> tag tells the Babel library to find that script, transpile the JSX code (like <App />) into regular React.createElement() JavaScript calls, and then execute it. This removes the need for a pre-compilation step.

# Technologies Used
**React (v18):** For building the component-based UI.

**ReactDOM (v18):** For rendering the React components to the DOM.

**Babel Standalone:** For in-browser JSX transpilation.

**Tailwind CSS:** For all styling.

**TheMealDB API:** The free and open API used for fetching recipe data.

# API Reference
This application uses the free TheMealDB API for all recipe data.

**Search recipes by ingredient:**

https://www.themealdb.com/api/json/v1/1/filter.php?i={ingredient}
**Lookup full meal details by ID:**

https://www.themealdb.com/api/json/v1/1/lookup.php?i={meal_id} 

# Google Gemini Pro

https://g.co/gemini/share/c078be5f5547
