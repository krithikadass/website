# Ex.07 Restaurant Website
# Date: 19.05.2025
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
```
home
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luxury Hotel</title>
    <link rel="stylesheet" href="{% static 'css/style.css' %}">
    <style>
        body {
            background-image: url('bg.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed;
            font-family: Arial, sans-serif;
            color: #fff;
        }

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            padding: 15px 0;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.5);
            z-index: 1000;
        }

        header h1 {
            margin: 0;
            text-align: center;
            font-size: 2rem;
            color: #f4c842;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            padding: 0;
            margin: 10px 0 0;
        }

        nav ul li {
            margin: 0 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: #f4c842;
            font-weight: bold;
            font-size: 1.1rem;
        }

        .hero {
            text-align: center;
            margin-top: 150px;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 30px;
        }

        .hero a {
            text-decoration: none;
            background-color: #f4c842;
            color: #000;
            padding: 10px 20px;
            font-size: 1.2rem;
            border-radius: 5px;
        }
    </style>
</head>

<body>
    <header>
        <h1>Welcome to Hotel Paradise</h1>
        <nav>
            <ul>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <div class="hero">
        <h2>Experience the Ultimate Comfort</h2>
        <img src="dining.jpg" alt="Dining Area" style="width: 100%; max-width: 600px; border-radius: 10px;">
        <p>Relax and unwind in our luxurious rooms and world-class amenities.</p>
    </div>
</body>

</html>

about
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Us - Hotel Paradise</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            line-height: 1.6;
        }

        header {
            color: white;
            text-align: center;
            padding: 100px 20px;
        }

        header h1 {
            font-size: 3rem;
            margin: 0;
        }

        header p {
            font-size: 1.5rem;
            margin-top: 10px;
        }

        main {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        section {
            margin-bottom: 40px;
        }

        section h2 {
            font-size: 2rem;
            color: #444;
            margin-bottom: 10px;
        }

        section p {
            font-size: 1.1rem;
            margin-bottom: 10px;
        }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            background: #f4f4f4;
            margin: 10px 0;
            padding: 10px;
            border-left: 5px solid #007BFF;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px 10px;
        }

        footer p {
            margin: 5px 0;
        }

        footer a {
            color: #007BFF;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>

<body>
    <header>
        <h1>Welcome to Hotel Paradise</h1>
        <p>Your perfect getaway destination</p>
    </header>
    <main>
        <section>
            <h2>About Us</h2>
            <p>At Hotel Paradise, we pride ourselves on offering a luxurious and tranquil experience for all our guests.
                Nestled in the heart of nature, our hotel combines modern amenities with breathtaking views to create an
                unforgettable stay.</p>
        </section>
        <section>
            <h2>Our Mission</h2>
            <p>Our mission is to provide exceptional hospitality and ensure every guest feels at home. Whether you're
                here for a relaxing vacation or a business trip, we strive to exceed your expectations.</p>
        </section>
        <section>
            <h2>Why Choose Us?</h2>
            <ul>
                <li>Luxurious rooms with stunning views</li>
                <li>World-class dining experiences</li>
                <li>State-of-the-art spa and wellness center</li>
                <li>Convenient location near popular attractions</li>
                <li>Friendly and professional staff</li>
            </ul>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 Hotel Paradise. All rights reserved.</p>
        <p>
            <a href="#">Privacy Policy</a> |
            <a href="#">Terms of Service</a> |
            <a href="#">Contact Us</a>
        </p>
    </footer>
</body>

</html>

contact

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us - Hotel Paradise</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        .container {
            max-width: 800px;
            margin: 50px auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        h1 {
            text-align: center;
            color: #2c3e50;
        }

        .contact-info {
            margin-top: 20px;
            text-align: center;
        }

        .contact-info p {
            margin: 5px 0;
        }
    </style>
</head>

<body>
    <div class="container">
        <h1>Meet Our Team</h1>
        <div style="display: flex; justify-content: space-around; margin-top: 20px;">
            <div style="text-align: center;">
                <img src="chef.jpg" alt="Chef" style="width: 150px; height: 150px; border-radius: 50%;">
                <p><strong>Chef</strong></p>
            </div>
            <div style="text-align: center;">
                <img src="owner.jpg" alt="Owner" style="width: 150px; height: 150px; border-radius: 50%;">
                <p><strong>Owner</strong></p>
            </div>
            <div style="text-align: center;">
                <img src="manager.jpg" alt="Manager" style="width: 150px; height: 150px; border-radius: 50%;">
                <p><strong>Manager</strong></p>
            </div>
        </div>
    </div>
    <div class="container">
        <h1>Contact Hotel Paradise</h1>
        <div class="contact-info">
            <p><strong>Address:</strong> 123 Paradise Lane, Dream City</p>
            <p><strong>Phone:</strong> +1 234 567 890</p>
            <p><strong>Email:</strong> contact@hotelparadise.com</p>
        </div>
    </div>
</body>

</html>

menu
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hotel Menu</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: #f8f8f8;
            color: #333;
        }

        h1 {
            color: #333;
            font-size: 3rem;
            text-align: center;
            margin: 20px 0;
            font-weight: 700;
        }

        h2 {
            color: #555;
            font-size: 1.8rem;
            text-align: center;
            margin-bottom: 30px;
            font-weight: 400;
        }

        .menu {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            max-width: 1200px;
            padding: 20px;
            justify-content: center;
        }

        .menu-item {
            width: 250px;
            border: 1px solid #ddd;
            border-radius: 10px;
            overflow: hidden;
            background-color: #fff;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .menu-item img {
            width: 100%;
            height: 150px;
            object-fit: cover;
        }

        .menu-item:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
        }

        .menu-item .details {
            padding: 15px;
            text-align: center;
        }

        .menu-item .details h3 {
            font-size: 1.5rem;
            margin: 10px 0;
            color: #333;
        }

        .menu-item .details p {
            font-size: 1rem;
            color: #666;
            margin: 5px 0;
        }

        .menu-item .details .price {
            font-size: 1.2rem;
            color: #e67e22;
            font-weight: bold;
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="title">Popular Dishes</div>
        <div class="grid">
            <div class="card">
                <img src="sq-scrumptious-tiramisu-cake-cake2636exot-AA.webp" alt="Dish Image">
                <div class="card-content">
                    <h3>Tiramisu Cake</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.100.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="download (3).jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>mushroom</h3>
                    <div class="price">Rs.200.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="Veg-Puff-Recipe.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>veg puffs</h3>
                    <div class="price">Rs.20.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="Samosas-with-Potatoes-and-Peas-2-1.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>samosa</h3>
                    <div class="price">Rs.15.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="naan.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>naan and paneer butter masala</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.200.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="images.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>dosa</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.10.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="idli.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>idli</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.10.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="full meals.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>full meals</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.100.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="sweet pongal.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>sweet pongal</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.50.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="rosemilk.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>rosemilk</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.40.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="soup.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>soup</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.70.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
            <div class="card">
                <img src="noodles.jpg" alt="Dish Image">
                <div class="card-content">
                    <h3>noodles</h3>
                    <p>Sample description text for this dish.</p>
                    <div class="price">Rs.150.00</div>
                    <button>Buy Now</button>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
```
# OUTPUT:

![Screenshot 2025-05-19 205238](https://github.com/user-attachments/assets/827a5d48-26ad-4399-ab1d-74897593fede)

![Screenshot 2025-05-19 205400](https://github.com/user-attachments/assets/f987159b-e7ea-404d-bb2e-bafabd3cc004)

![Screenshot 2025-05-19 205454](https://github.com/user-attachments/assets/109b1935-0bf4-4409-866b-7abc6ff1545a)

![Screenshot 2025-05-19 205734](https://github.com/user-attachments/assets/89bcb355-9f2b-45b7-b038-4744ff3394e8)

![Screenshot 2025-05-19 205855](https://github.com/user-attachments/assets/54650748-e31f-4d13-b5cf-07c18ee46207)




# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
