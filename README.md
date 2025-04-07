# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.

>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled HTML Page</title>
    <!-- Linking the external CSS file -->
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1 id="mainHeading" class="headerText">Welcome to My Web Page</h1>
        <img src="https://via.placeholder.com/350x150" alt="Placeholder Image" class="mainImage" />
    </header>

    <main>
        <section class="contentSection">
            <p class="paragraphText">This is a sample paragraph. It demonstrates the use of different font styles and spacing.</p>
            <div id="contactInfo">
                <h2>Contact Information</h2>
                <p>You can contact us at info@example.com or via the form below.</p>
            </div>
        </section>
        <form>
            <input type="text" id="nameInput" placeholder="Your Name">
            <input type="email" id="emailInput" placeholder="Your Email">
            <button type="submit" id="submitBtn">Submit</button>
        </form>
    </main>

    <footer>
        <p class="footerText">Copyright 2021. All Rights Reserved.</p>
    </footer>
</body>
</html>
/* style.css */

/* 1. Using an ID selector to style the main heading */
#mainHeading {
    color: #333;
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 20px 0;
    border-bottom: 2px solid #ddd;
}

/* 2. Using a Class selector for general text styling */
.headerText, .paragraphText, .footerText {
    color: #666;
    font-family: 'Open Sans', sans-serif;
}

/* 3. Using a Class selector to style an image */
.mainImage {
    max-width: 100%;
    height: auto;
    margin: 20px 0;
    border: 5px solid #ccc;
    border-radius: 10px;
}

/* General styling for spacing and alignment */
body {
    margin: 0;
    padding: 20px;
    font-family: 'Merriweather', serif;
    line-height: 1.6;
}

/* Form styling */
form {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 30px;
}

/* Button styling */
#submitBtn {
    padding: 10px 20px;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
#submitBtn:hover {
    background-color: #45a049;
}

/* Contact Info Section Spacing */
#contactInfo {
    margin: 30px 0;
}

/* Footer Text Styling */
.footerText {
    text-align: center;
    margin: 20px 0;
    color: #666;
}

/* Additional margin and padding examples for other elements can be added as needed */
