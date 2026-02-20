## Day 4: CSS Basics
🌟 What is CSS?
## CSS = Cascading Style Sheets

-👉 HTML creates structure -👉 CSS makes it beautiful

Example:
HTML:

Hello
-Without CSS → Plain text -With CSS → Colored, styled, centered

## ✅ 1️⃣ Types of CSS (3 Ways)
# 🔹 1. Inline CSS
-CSS written inside HTML tag using style attribute.

## My Profile
# 🔹 2. Internal CSS
-CSS written inside <style> tag in section.

<style> h1 { color: red; } </style>
-✔ Used for single page -❌ Not reusable for multiple pages

# 🔹 3. External CSS (Best Practice ✅)
-CSS written in separate file → style.css

Step 1: Create style.css
h1 { color: green; }

Step 2: Link it in HTML
-✔ Clean code -✔ Used in real projects -✔ Reusable

## ✅ 2️⃣ CSS Selectors
-Selectors are used to target HTML elements.

# 🔹 1. Element Selector
-Targets all elements of that type. p { color: blue; } -Applies to all

tags.

# 🔹 2. Class Selector
-Starts with . CSS

.myclass { color: red; }

HTML:

Hello

-✔ Can use multiple times
# 🔹 3. ID Selector
Starts with # CSS #title { color: green; }

HTML:

Welcome
-✔ Used only once

## ✅ 3️⃣ Colors, Fonts & Text Styling
# 🎨 Colors
CSS color: red; /* Name / color: #ff0000; / Hex */ color: rgb(255,0,0);

# 🔤 Fonts
CSS font-family: Arial, sans-serif; font-size: 18px; font-weight: bold;

# 📝 Text Styling
CSS text-align: center; text-decoration: underline; text-transform: uppercase; letter-spacing: 2px;

## ✅ 4️⃣ Style the HTML Profile Page
# HTML :

*<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sindhura's profile</title>
    <!--External CSS-->
    <link rel="stylesheet" href="style.css">

    <!-- Internal CSS -->
    <style>
        body {
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
        }

        .section {
            background-color: white;
            margin: 20px;
            padding: 15px;
            border-radius: 10px;
        }

        .skills p {
            color: darkgreen;
            font-weight: bold;
        }
    </style>
</head>

<body align="center">
    <!-- Inline CSS -->
    <h2 style="color: darkblue;">My Profile</h2>

    <img src="myself.jpeg" 
         alt="My Photo"
         width="150"
         height="150"
         style="border-radius:50%;">

    <div class="section">
        <h2>About Me</h2>
        <p>
            Hello! My name is Sindhura <br>
            I am learning Full stack Web development<br>
            I am pursuing my bachelors degree in Computer science and Engineering.
        </p>
    </div>

    <div class="section skills">
        <h2>My Skills</h2>
        <p>HTML</p>
        <p>CSS</p>
        <p>Java script</p>
    </div>

    <div class="section">
        <h2>Contact Me</h2>
        <p>Email:sindhura@gmail.com</p>
        <p>
            GitHUb:
            <a href="https://github.com/username" target="_blank">
                Visit my Github
            </a>
        </p>
    </div>

</body>

</html>


## CSS :


h2 {

    text-transform: uppercase;

}


a {

    text-decoration: none;
    color:purple;
    
}

a:hover {

    color:red;
    
}

img {

    margin-top:10px;

}

# OUT PUT
![Day-4 Output](../DAY-4-output.png)
