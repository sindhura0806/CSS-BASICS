## Day 4: CSS Basics
# 🌟 What is CSS?

CSS = Cascading Style Sheets

-👉 HTML creates structure
-👉 CSS makes it beautiful

# Example:
HTML:

<h1>Hello</h1>

-Without CSS → Plain text
-With CSS → Colored, styled, centered

# ✅ 1️⃣ Types of CSS (3 Ways)
# 🔹 1. Inline CSS

-CSS written inside HTML tag using style attribute.

<h1 style="color: blue;">My Profile</h1>

# 🔹 2. Internal CSS

-CSS written inside <style> tag in <head> section.

<head>
  <style>
    h1 {
      color: red;
    }
  </style>
</head>

-✔ Used for single page
-❌ Not reusable for multiple pages

# 🔹 3. External CSS (Best Practice ✅)

-CSS written in separate file → style.css

# Step 1: Create style.css
h1 {
  color: green;
}

# Step 2: Link it in HTML
<head>
  <link rel="stylesheet" href="style.css">
</head>

-✔ Clean code
-✔ Used in real projects
-✔ Reusable

# ✅ 2️⃣ CSS Selectors

-Selectors are used to target HTML elements.

# 🔹 1. Element Selector

-Targets all elements of that type.
p {
  color: blue;
}
-Applies to all <p> tags.

# 🔹 2. Class Selector

-Starts with . CSS

.myclass {
  color: red;
}

HTML:
<p class="myclass">Hello</p>
-✔ Can use multiple times


# 🔹 3. ID Selector

Starts with # CSS
#title {
  color: green;
}

HTML:
<h1 id="title">Welcome</h1>

-✔ Used only once

# ✅ 3️⃣ Colors, Fonts & Text Styling
# 🎨 Colors
CSS 
color: red;        /* Name */
color: #ff0000;    /* Hex */
color: rgb(255,0,0);

# 🔤 Fonts
CSS 
font-family: Arial, sans-serif;
font-size: 18px;
font-weight: bold;

# 📝 Text Styling
CSS
text-align: center;
text-decoration: underline;
text-transform: uppercase;
letter-spacing: 2px;

# ✅ 4️⃣ Style the HTML Profile Page
# HTML :
<!DOCTYPE html>
<html>
<head>
    <title>My Profile</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="container">

        <!-- Profile Photo -->
         <h1>My Profile</h1>
        <img src="img/SRUJANA.jpeg" 
        alt="My Photo"
        class="profile-img">

        <!-- About Section -->
        <div class="section">
            <h2>About Me</h2>
            <p>
                Hello! My name is Srujana. <br>
                I am learning HTML and Web Development.<br>
                I am passionate about building websites.
            </p>
        </div>

        <!-- Skills Section -->
        <div class="section">
            <h2>My Skills</h2>
            <p>HTML</p>
            <p>CSS</p>
            <p>JavaScript</p>
        </div>

        <!-- Contact Section -->
        <div class="section">
            <h2>Contact Me</h2>
            <p>Email: srujanach2005@gmail.com</p>
            <p>
                GitHub:
                <a href="https://github.com/srujanach2005-star" target="_blank">
                    Visit My GitHub
                </a>
            </p>
        </div>

    </div>

</body>
</html>

# CSS :

body {
    background-color: #f0f8ff;
    
    font-family: Arial, sans-serif;
}


.container {
    width: 400px;
    
    margin: 40px auto;
    
    padding: 20px;
    
    background-color: white;
    
    border-radius: 10px;
    
    box-shadow: 0px 0px 10px gray;
    
    text-align: center;
}


.profile-img {
    width: 150px;
    
    height: 150px;
    
    border-radius: 50%;
    
    border: 4px solid black;
}


.section {
    margin-top: 20px;
}


h2 {
    color: black;
    
    text-transform: uppercase;
}


p {
    color: #555;
    
    font-size: 14px;
}


a {
    color: black;
    
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
    
    color: darkred;
}
.container:hover {
    transform: scale(1.05);
    
    transition: 0.3s;
}

# OUT PUT
![Day-4 Output](img/day-4-output.png)







