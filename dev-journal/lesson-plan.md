
# Intro Web Development Fun - Lesson Plan

This lesson will cover Git, GitHub, HTML, CSS, and JavaScript. Readers will have a simple web-page hosted at a real URL at the end.

## Prerequisites

- [Download VS Code](https://code.visualstudio.com)
  - Purpose: Code Editor
  - Install Extension [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Download Git](https://git-scm.com/downloads)
  - Purpose: Code Source Control
- [Create GitHub Account](https://github.com)
  - Purpose: Cloud Source Code Platform

## Getting Started

### 1) Create a GitHub Code Repository
*(Purpose: Back-up your code and make it accessible to GitHub so it's easy to attach to a real URL)*

1. Log in to [GitHub](https://github.com)
2. Click the "New" button in the Repositories section.
3. Give it a name like `web-dev-fun` click "Create repository"

### 2) Clone the Repository
*(Purpose: Make a linked copy of your repository locally on your computer so you can add code to it)*

1. Using your File Explorer (Mac: Finder), create a code folder in a location of your choosing. You can use an existing folder like My Documents if you so choose, but I will reference this folder as your "code folder".
2. Open VS Code, select File > Open Folder (Mac: Open), and open your code folder
3. In VS Code use Alt+` to open the terminal
4. On your GitHub Repository page, click `Clone or download` and copy the clone URL
5. Type `git clone `, space, CTRL+V to paste the GitHub clone URL, and Enter/Return to execute the command
6. In VS Code select File > Open Folder (Mac: Open) and open the newly created repository folder which will have the same name you gave it on the website
7. Set local username and email to your GitHub account
 - `git config user.name uidclr`
 - `git config user.email crahman@wisc.edu`


### 3) Set up HTML, CSS, and JavaScript

1. Create an index.html file and paste **Snippet-1**:
   - Add a header (e.g. `<h1>Experimental Utilities</h1>`) 
   - Add a description (e.g. `<p>This is a page created by Cory Leigh Rahman to test web programming!</p>`)
2. Run the app by clicking Go Live in the bottom-right corner
   - This creates a temporary local server and serves the web page to the URL http://localhost:5500
   - Servers automatically look for a file named `index.html` as a starting point, that's how it knows what to show
3. Create empty `style.css` adjacent to the index.html and paste  **Snippet-2**
   - Just before the closing `</head>` tag, add `<link rel="stylesheet" href="style.css">`
   - Add another style to it, like try selecting `p` or `body` and use the attributes `color` or `background-color` 
4. Create empty `script.js` file adjacent to the index.html
   - Just before the closing `</html>` tag, add `<script src="script.js"></script>`
   - Add a button to the HTML Body (e.g. `<button id="info-button">&#9432; More Info</button>`)

**Snippet-1 (HTML):**
```html
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Web Dev Fun</title>
    <meta name="description" content="Web Dev Fun">
    <meta name="author" content="Cory Leigh Rahman">
  </head>
  <body>
    
  </body>
</html>
```

**Snippet-2 (CSS):**
```css
h1 {
  font-family: Arial;
  color: darkgray;
}
```

**Snippet-3 (JS):**
```javascript
console.log("JavaScript is working from the script.js file!");
document.querySelector("#info-button").addEventListener("click", function (e) {

});
```

### 4) Content: Fun with Text Replacement ?

### 5) Content: Another activity... ?

### X) Play with Git & Make a Commit

### Y) Turn on GitHub Pages and select the Master branch

## Troubleshooting tips

- Extensions
  - CTRL+SHIFT+P > Search "Reload Window", hit enter
  - File > Preferences > Settings > Search for the name of the extension and make sure it's enabled
- Git
  - Make sure it was added to the PATH on installation
  - File > Preferences > Settings > Search for "git.path", edit in settings.json, add path to the local Git installation.