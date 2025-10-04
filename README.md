# Ex.07 Restaurant Website
# Date:04\10\25
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
'''
res.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>RESTUARANT</title>
    <link rel="stylesheet" href="style.css" />
</head>

<body>

    <header>
        <div class="logo">
            <img src="logo.jpg" alt="Amma Logo">
            <h1>AMMA'S KITCHEN</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Menu</a></li>
                <li><a href="#">Management</a></li>
                <li><a href="#">Contact Us</a></li>

            </ul>
        </nav>
    </header>

    <section class="banner">
        <div class="banner-text">
            <h1> Now with New dishes!!!</h1>
            <p>"Welcoming you with Hearts of Love , plate of Dishes, Mind of Serving!" </p>
        </div>
    </section>

    <section class="cards">
        <div class="card">
            <img src="idly.jpg" alt="Menu">
            <h2>IDLY</h2>
            <p>Making your day to be delightful by our idly,vada and sambar</p>
            <a href="#">See our New menu</a>
        </div>
        <div class="card">
            <img src="dosa.jpg" alt="Menu">
            <h2>DOSAI</h2>
            <p>Aspire our golden color long dosa</p>
            <a href="#">See our New menu</a>
        </div>
        <div class="card">
            <img src="chapahi.jpg" alt="Menu">
            <h2>CHAPATHI</h2>
            <p>Making to feel light on this dish</p>
            <a href="#">See our New menu</a>
        </div>
        <div class="card">
            <img src="biryani.jpg" alt="Menu">
            <h2>BIRIYANI</h2>
            <p> Happiness of spices taste </p>
            <a href="#">See our New menu</a>
        </div>
        <div class="card">
            <img src="chicken rice.jpg" alt="Menu">
            <h2>CHICKEN RICE</h2>
            <p>Taste of roadside chickenrice with better hygenic and health</p>
            <a href="#">Book your table now</a>
        </div>
        <div class="card">
            <img src="koth.jpg" alt="Menu">
            <h2>OPENING HOURS</h2>
            <p>Timings</p>
            <ul class="hours">
                <li>Mon - Fri: 2pm - 10pm</li>
                <li>Sat: 2pm - 11pm</li>
                <li>Sun: 2pm - 9pm</li>
            </ul>
        </div>
    </section>
    <h3>Designed and designated by Rougith</h3>
    <footer>
        <img src="logo.jpg" alt="Logo small">
        <p>&copy; 2025 Amma's Kitchen</p>
        <p class="credit">💛 Design & Designated by <strong>Rougith</strong></p>
    </footer>


    <script src="script.js"></script>
</body>

</html>


#style.css
body {
    font-family: verdana, sans-serif;
    margin: 0;
    background-color: beige;
}

header {
    font-size: 25px;
    text-align: center;
    padding: 50px;
    background-color: yellow;
}

.logo {
    display: flex;
    justify-content: center;
    align-items: center;
}

.logo img {
    width: 500px;
    height: 300px;
    border-radius: 50%;
    margin-right: 20px;
}

.logo h1 {
    font-size: 3rem;
    color: #873f3f;
    letter-spacing: 2px;
}


nav {
    background-color: grey;
    padding: 20px 0;
}

nav ul {

    display: flex;
    justify-content: center;
    margin: 0;
    padding: 0;
}

nav li {
    margin: 30px;
}

nav a {
    text-decoration: none;
    color: #fff;
    font-weight: bold;
    padding: 8px 15px;
    border-radius: 30px;
    transition: background-color 0.3s;
}

nav a:hover {
    background-color: #a3c47d;
}


.banner {
    background: url("res\ back.jpg") no-repeat center center/cover;
    color: green;
    text-align: center;
    padding: 80px 20px;
    border-radius: 10px;
    margin: 20px auto;
    max-width: 90%;
}

.banner h2 {
    font-size: 4rem;
    font-weight: bold;
    margin-bottom: 10px;
}

.banner p {
    font-size: 3.5rem;
}


.cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 50px;
    margin: 40px auto;
    max-width: 1400px;
}


.card {
    background-color: aqua;
    width: 400px;
    border-radius: 20px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
    transform: translateY(-8px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}


.card img {
    width: 100%;
    height: 250px;

    object-fit: cover;
    display: block;
}

.card h3 {
    color: #333;
    margin: 15px 0 5px 0;
    font-size: 1.3rem;
}

.card p {
    color: brown;
    font-size: 2rem;
    margin: 0 20px 15px 20px;
    line-height: 1.5;
}

.card a {
    color: #2b7a2b;
    font-weight: bold;
    text-decoration: none;
    display: inline-block;
    margin-bottom: 15px;
}

.card a:hover {
    text-decoration: underline;
}


.hours {
    list-style: none;
    padding: 0;
    color: #444;
    margin: 20px 0 30px 0;
    font-size: 1.5rem;
}


footer {
    text-align: center;
    padding: 30px 10px;
    background-color: #fafafa;
    margin-top: 50px;
    border-top: 2px solid #eee;
}

footer img {
    width: 100px;
    height: 60px;
    border-radius: 50%;
}

footer p {
    margin: 5px 0;
    color: orchid;
    font-size: 40px;
}


footer .credit {
    font-size: 40px;
    color: blue;
    font-weight: bold;
    margin-top: 30px;
}

footer .credit strong {
    color: #2b7a2b;
}


Management.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration - AMMA's KITCHEN</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <h1>Our Team</h1>
    </header>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="Management.html" class="active">Administration</a></li>
            <li><a href="contact us.html">Contact Us</a></li>
            <li><a href="about us.html">Contact Us</a></li>
        </ul>
    </nav>

    <section class="cards">
        <div class="card"><img src="chef1.jpg">
            <h3>Mr.Damodaran</h3>
            <p>Head Chef</p>
        </div>
        <div class="card"><img src="chef  2.jpg">
            <h3>Mr. Venkatesh Bhat</h3>
            <p>Pastry Chef</p>
        </div>
        <div class="card"><img src="chef 3.jpg">
            <h3>Mr. Sanjeev Kapoor</h3>
            <p>Restaurant Manager</p>
        </div>
        <div class="card"><img src="chef4.jpg">
            <h3>Mr. Rakesh Raghunath</h3>
            <p>Marketing Head</p>
        </div>
        <div class="card"><img src="chef5.jpg">
            <h3>Mr. Madhampatty Rangaraj</h3>
            <p>Assistant Chef</p>
        </div>
        <div class="card"><img src="chef6.jpg">
            <h3>Mr. Deena</h3>
            <p>Public Relations</p>
        </div>
    </section>

    <footer>
        <p>© 2025 AMMA'S KITCHEN</p>
        <p class="credit">Design and Designated by <strong>Rougith</strong></p>
    </footer>
</body>

</html>

contact us.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us - Little Lemon</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <h1>Contact Us</h1>
    </header>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="administration.html">Administration</a></li>
            <li><a href="contact us.html" class="active">Contact Us</a></li>
            <li><a href="about us.html">Contact Us</a></li>
        </ul>
    </nav>

    <section class="contact">
        <h2>We’d happy to Hear From You!</h2>
        <p><strong>Address:</strong> No. 12, Main Street, Tiruvannamalai, Tamil Nadu</p>
        <p><strong>Phone:</strong> +91 00000000000</p>
        <p><strong>Email:</strong> ammakitchen@.com</p>
    </section>

    <footer>
        <p>© 2025 AMMA'S KITCHEN</p>
        <p class="credit">Design and Designated by <strong>Rougith</strong></p>
    </footer>
</body>

</html>

'''
# OUTPUT:

![alt text](<Screenshot 2025-10-04 202743.png>)


![alt text](<Screenshot 2025-10-04 203348.png>)


![alt text](<Screenshot 2025-10-04 203409.png>)


# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
