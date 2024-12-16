# Ex.07 Restaurant Website
## Date:16-12-2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Butterfly - Home</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #fdfcfb;
        }

        *, *::before, *::after {
            box-sizing: border-box;
        }

        header {
            background: linear-gradient(90deg, #ff7f50, #ff4500);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        header img {
            height: 60px;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 500;
            margin: 0 15px;
            transition: color 0.3s;
            font-size: 1.1rem;
        }

        header nav a:hover {
            color: #ffd700;
        }

        .banner {
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 50px 20px;
            background: url('banner-placeholder.jpg') no-repeat center center/cover;
            position: relative;
            overflow: hidden;
            height: 400px;
            color: white;
            text-align: center;
        }

        .banner:after {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 0;
        }

        .banner-content {
            position: relative;
            z-index: 1;
            max-width: 600px;
        }

        .banner-content h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            font-family: 'Playfair Display', serif;
            color: #ffd700;
        }

        .banner-content p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .banner-content a {
            background: #ff6347;
            color: white;
            padding: 12px 25px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            transition: background 0.3s ease;
            font-size: 1rem;
        }

        .banner-content a:hover {
            background: #e53e2e;
        }

        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 50px 20px;
            background: #fff8ef;
            gap: 30px;
        }

        .feature {
            background: white;
            border-radius: 12px;
            padding: 25px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            flex: 1;
            max-width: 300px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
        }

        .feature img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .feature h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: #ff4500;
        }

        .feature p {
            font-size: 1rem;
            color: #666;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ff4500;
        }

        @media (max-width: 768px) {
            .banner {
                height: auto;
                padding: 30px 20px;
            }

            .banner-content h1 {
                font-size: 2.5rem;
            }

            .features {
                gap: 20px;
                padding: 20px;
            }

            header nav a {
                margin: 0 10px;
                font-size: 0.9rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="banner">
        <div class="banner-content">
            <h1>Welcome to Butterfly</h1>
            <p>Experience the finest flavors and a cozy ambiance at Butterfly. We serve happiness on a plate!</p>
            <a href="#features">Explore Now</a>
        </div>
    </div>

    <section id="features" class="features">
        <div class="feature">
            <img src="ambi.jpg" alt="Cozy Ambiance">
            <h3>Cozy Ambiance</h3>
            <p>Enjoy your meals in a warm, welcoming, and beautifully designed space.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Butterfly. All rights reserved. | <a href="#">Privacy Policy</a></p>
    </footer>
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Butterfly - Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #fdfcfb;
        }

        *, *::before, *::after {
            box-sizing: border-box;
        }

        header {
            background: linear-gradient(90deg, #ff7f50, #ff4500);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 500;
            margin: 0 15px;
            transition: color 0.3s;
            font-size: 1.1rem;
        }

        header nav a:hover {
            color: #ffd700;
        }

        .menu-container {
            padding: 50px 10%;
            text-align: center;
            background-color: #fff8ef;
        }

        .menu-container h1 {
            font-size: 3rem;
            color: #ff4500;
            margin-bottom: 30px;
            font-family: 'Playfair Display', serif;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .menu-item {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .menu-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 4px solid #ff4500;
        }

        .menu-details {
            padding: 20px;
            text-align: left;
        }

        .menu-details h3 {
            font-size: 1.8rem;
            color: #ff6347;
            margin-bottom: 10px;
        }

        .menu-details p {
            font-size: 1rem;
            color: #666;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-size: 1.4rem;
            font-weight: bold;
            color: #e53e2e;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 50px;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ff4500;
        }

        @media (max-width: 768px) {
            header nav a {
                margin: 0 10px;
                font-size: 0.9rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <h1>Butterfly</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="menu-container">
        <h1>Our Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="briyani.jpg" alt="Spaghetti">
                <div class="menu-details">
                    <h3>Chicken Briyani</h3>
                    <p class="price">₹250/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="rice.jpeg" alt="Pizza">
                <div class="menu-details">
                    <h3>Chicken Rice</h3>
                    <p class="price">₹160/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="fish.jpg" alt="Lasagna">
                <div class="menu-details">
                    <h3>Fish Fry</h3>
                    <p class="price">₹180/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="KUTTU-PORATTA.jpg" alt="Salad">
                <div class="menu-details">
                    <h3>Kothu Parotta</h3>
                    <p class="price">₹190/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="grill.jpeg" alt="Risotto">
                <div class="menu-details">
                    <h3>Chicken Grill</h3>
                    <p class="price">₹400/-</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 Butterfly. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Butterfly - Contact Us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(to bottom, #fff8ef, #fdfcfb);
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(90deg, #ff7f50, #ff4500);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        header img {
            height: 50px;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 500;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1.1rem;
        }

        header nav a:hover {
            color: #ffd700;
        }

        .contact-banner {
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(to bottom, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('contact.jpeg') no-repeat center center/cover;
            color: white;
            height: 300px;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.8);
        }

        .contact-banner h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            color: #ffd700;
        }

        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 40px 20px;
            gap: 30px;
            background: #fff8ef;
        }

        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .contact-details:hover, .contact-form:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        .contact-details h2, .contact-form h2 {
            font-size: 2.2rem;
            margin-bottom: 20px;
            color: #ff4500;
            text-align: center;
        }

        .contact-details p {
            margin: 15px 0;
            font-size: 1rem;
            color: #555;
        }

        .contact-details img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .contact-form label {
            font-size: 1rem;
            color: #555;
            margin-bottom: 5px;
            display: block;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
            transition: border 0.3s ease;
        }

        .contact-form input:focus, .contact-form textarea:focus {
            border-color: #ff7f50;
            outline: none;
        }

        .contact-form textarea {
            height: 120px;
            resize: none;
        }

        .contact-form button {
            width: 100%;
            padding: 12px;
            background: #ff4500;
            color: white;
            font-size: 1.2rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .contact-form button:hover {
            background: #e53e2e;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px 0;
            margin-top: 40px;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ff4500;
        }

        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }

            .contact-banner h1 {
                font-size: 2.5rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="contact-banner">
        <h1>Contact Us</h1>
    </div>

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            <p><strong>Address:</strong> Butterfly, Chennai, Tamil Nadu, India</p>
            <p><strong>Phone:</strong> +91 8668141112</p>
            <p><strong>Email:</strong> butterfly@gmail.com</p>
            <p><strong>Hours:</strong> Mon-Sun: 10 AM - 10 PM</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Butterfly. All rights reserved. | <a href="#">Privacy Policy</a></p>
    </footer>

</body>
</html>

admin.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Butterfly - Administration</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            color: #333;
            background: linear-gradient(to bottom, #fff8ef, #fdfcfb);
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(90deg, #ff7f50, #ff4500);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        header h1 {
            font-size: 2rem;
            font-weight: bold;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 600;
            margin: 0 15px;
            font-size: 1.1rem;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ffd700;
        }

        .admin-container {
            padding: 50px 20px;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 3rem;
            color: #ff4500;
            margin-bottom: 40px;
            font-family: 'Playfair Display', serif;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .admin-item {
            background: white;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .admin-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        .admin-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .admin-details {
            padding: 20px;
        }

        .admin-details h3 {
            font-size: 1.8rem;
            color: #ff7f50;
            margin-bottom: 10px;
        }

        .admin-details p {
            font-size: 1rem;
            color: #555;
            line-height: 1.5;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ff4500;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <h1>Butterfly</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="admin-container">
        <h1>Our Leadership Team</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="my.jpg" alt="CEO">
                <div class="admin-details">
                    <h3>Jones</h3>
                    <p>CEO - Leading Butterfly with a vision of excellence and innovation in hospitality.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="maneger.jpg" alt="Manager">
                <div class="admin-details">
                    <h3>Joel</h3>
                    <p>Manager - Ensures smooth operations and a great dining experience for all guests.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="dhamu1.jpeg" alt="Master Chef">
                <div class="admin-details">
                    <h3>Dhamu</h3>
                    <p>Master Chef - Brings authentic Italian flavors to every dish served.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="MODIJI.png" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Modi</h3>
                    <p>Assistant Managing Director - Supporting the team with strategy and execution excellence.</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 Butterfly. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>
</html>

```


## OUTPUT:
![alt text](<Screenshot (5).png>)
![alt text](<Screenshot (6).png>)
![alt text](<Screenshot (7).png>)
![alt text](<Screenshot (8).png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
