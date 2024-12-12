# Ex.07 Restaurant Website
## Date:

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
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Courgette&family=Merienda:wght@300..900&display=swap" rel="stylesheet">
    <title>DJ RESTAURANT</title>
    <style>
        body {
            margin: 0;
            font-family: 'Merienda', cursive;
            background: url('resturant home page.jpg') no-repeat center center fixed;
            background-size: cover;
            color: rgb(234, 245, 16);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            text-align: center;
            padding: 50px 20px;
            background: rgba(0, 0, 0, 0.5);
            border-bottom: 2px solid goldenrod;
        }

        header h1 {
            font-size: 80px;
            letter-spacing: 10px;
            margin: 0;
            text-shadow: 2px 2px 8px black;
        }

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.7); 
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.5);
            z-index: 1000;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 10px 20px;
            display: flex;
            justify-content: center;
        }

        nav li {
            margin: 0 20px;
        }

        nav a {
            text-decoration: none;
            color:azure;
            font-size: 18px;
            font-weight: 600;
            padding: 10px 20px;
            border-radius: 5px;
        }

        

        main {
            flex: 1;
            padding: 40px;
            text-align: center;
            background: rgba(255, 255, 255, 0.1); 
            margin: 20px auto;
            max-width: 900px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.7);
            animation: fadeInUp 1.5s ease-in-out;
        }

        main p {
            font-size: 24px;
            font-weight: 400;
            line-height: 1.5;
            color:blue;
            text-shadow: 1px 1px 3px black;
        }

        footer {
            background: rgba(0, 0, 0, 0.8); 
            color: white;
            text-align: center;
            padding: 20px 0;
            border-top: 2px solid greenyellow;
            box-shadow: 0 -4px 6px rgba(0, 0, 0, 0.5);
        }

        footer p {
            margin: 5px 0;
            font-size: 16px;
        }

        footer a {
            color: goldenrod;
            text-decoration: none;
            margin: 0 10px;
            font-size: 18px;
            transition: color 0.3s ease-in-out;
        }

        footer a:hover {
            color: #d4af37;
        }

       
    </style>
</head>
<body>
    <header>
        <h1>DJ RESTAURANT!!!!!</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#" title="Home">Home</a></li>
            <li><a href="menu.html" title="menu">menu</a></li>
            <li><a href="adminis.html" title="adminis">Administration</a></li>
            <li><a href="contact.html" title="Contact Us">Contact Us</a></li>
        </ul>
    </nav>
    <main>
        <p>Welcome to DJ Restaurant </p>
        <p>This the place for party</p>
    </main>
    <footer>
        <p>&copy; 2023 DJ Restaurant | Designed by: <b>SANTHA BABU G</b></p>
        <p>
            <a href="#" title="Facebook">Facebook</a> |
            <a href="#" title="Twitter">Twitter</a> |
            <a href="#" title="Instagram">Instagram</a>
        </p>
    </footer>
</body>
</html>

menu.html


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu Arena</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg,yellow, #e0e0e0);
            color: #333;
        }
        header {
            background-color:crimson;
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: rgba(0, 0, 0, 0.3);
        }
        header h1 {
            margin: 0;
            font-size: 48px;
        }
        header p {
            font-size: 18px;
            margin-top: 5px;
            font-weight: lighter;
        }
        .menu-section {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }
        .menu-section h2 {
            text-align: center;
            margin-bottom: 20px;
            font-size: 32px;
            color: #2a008b;
            border-bottom: 3px solid #ddd;
            display: inline-block;
            padding-bottom: 5px;
        }
        .menu-grid {
            display: flex;
            gap: 30px;
        }
        .menu-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .menu-item:hover {
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .menu-item h3 {
            margin: 15px 0 10px;
            font-size: 18px;
            color: #333;
        }
        .menu-item p {
            color: #555;
            font-size: 12px;
            margin: 0 10px 15px;
        }
        .menu-item .price {
            font-weight: bold;
            font-size: 15px;
            color: #33008b;
            margin-bottom: 15px;
        }
        footer {
            text-align: center;
            padding: 15px 0;
            background-color: #333;
            color: white;
            margin-top: 40px;
        }
    </style>
</head>
<body>

<header>
    <h1>Delicious food</h1>
    <p>Your favorite spot for authentic Indian non-veg meals</p>
</header>

<div class="menu-section">
    <h2>Chicken</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="biryani image.webp" alt="biriyani">
            <h3>biriyani</h3>
            <p>Fragrant rice cooked with chicken, spices, and herbs.</p>
            <div class="price">₹150</div>
        </div>
        <div class="menu-item">
            <img src="bbq image.avif" alt="bbq">
            <h3>bbq</h3>
            <p>Slow-cooked mutton with aromatic</p>
            <div class="price">₹350</div>
        </div>
        <div class="menu-item">
            <img src="chicken 65.jpg" alt="chicken 65">
            <h3>chicken 65</h3>
            <p>slow cook and moisture</p>
            <div class="price">₹300</div>
        </div>
        <div class="menu-item">
            <img src="chicken gril image.jpg" alt="chicken gril">
            <h3>chicken gril</h3>
            <p>full chicken boiled slowly in fire</p>
            <div class="price">₹250</div>
        </div>
        <div class="menu-item">
            <img src="chicken strick.jpg" alt="chicken strick">
            <h3>chicken strick</h3>
            <p>A simple, aromatic  dish cooked in fire.</p>
            <div class="price">₹100</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Veg</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="dosa image.webp" alt="Crispy dosa">
            <h3>Crispy Dosa</h3>
            <p>Rostted in brownish color</p>
            <div class="price">₹180</div>
        </div>
        <div class="menu-item">
            <img src="egg fried image.jpg" alt="egg fried ">
            <h3>egg fried </h3>
            <p>Spicy and soft rice and with chicken .</p>
            <div class="price">₹220</div>
        </div>
        <div class="menu-item">
            <img src="idli image.jpg" alt="idli">
            <h3>idli</h3>
            <p>So soft</p>
            <div class="price">₹50</div>
        </div>
        <div class="menu-item">
            <img src="meels image.avif" alt="meels">
            <h3>meels</h3>
            <p>Delicious and type of food</p>
            <div class="price">₹280</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Mutton and sweets</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="mutton image.webp" alt="mutton">
            <h3>mutton</h3>
            <p>mutton is marinated in flavorful spices.</p>
            <div class="price">₹220</div>
        </div>
        <div class="menu-item">
            <img src="noodle image.jpg" alt="noodles">
            <h3>noodles</h3>
            <p>noodles with chicken</p>
            <div class="price">₹280</div>
        </div>
        <div class="menu-item">
            <img src="ragi ball image.jpg" alt="ragi ball">
            <h3>ragi ball</h3>
            <p>healthly and tastly</p>
            <div class="price">₹50</div>
        </div>
        <div class="menu-item">
            <img src="sweet image.webp" alt="sweet">
            <h3>sweet</h3>
            <p>different type of sweet</p>
            <div class="price">₹250</div>
        </div>
        <div class="menu-item">
            <img src="juice image.jpg" alt="juice">
            <h3>juice</h3>
            <p>Different type of juice</p>
            <div class="price">₹70</div>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2024 Delicious Indian Bites. All rights reserved.</p>
</footer>

</body>
</html>

adminis.html


<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chefs</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@700&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color:yellow;
        }

        header {
            text-align: center;
            background-color: #0e6ff5;
            padding: 20px 0;
        }

        header h1 {
            font-family: "Caveat", cursive;
            font-size: 50px;
            color: white;
            margin: 0;
        }


        .chefs-container {
            display: flex;
            gap: 20px;
            padding: 40px;
            margin: auto;
        }

        .chef-card {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
        }

        .chef-card:hover {
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .chef-card img {
            width: 100%;
            object-fit: contain; 
            max-height: 300px; 
        }

        .chef-details {
            padding: 20px;
        }

        .chef-details h1 {
            font-size: 20px;
            color: rgb(181, 101, 29);
            margin: 10px 0;
        }

        .chef-details h2,
        .chef-details h3 {
            font-size: 16px;
            color: rgb(85, 85, 85);
            margin: 5px 0;
        }

       
        footer {
            text-align: center;
            background-color:aliceblue;
            color:brown;
            padding: 10px 0;
            margin-top: 20px;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>

  
    <header>
        <h1>Cooking chef</h1>
    </header>

    
    <div class="chefs-container">
        <div class="chef-card">
            <img src="damodaran chef.jpg" alt="Chef Dhamu">
            <div class="chef-details">
                <h1>Mr. Dhamu</h1>
                <h2>Designation: Sous Chef</h2>
                <h3>Experience: 6 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="chef-venkatesh-bhat.jpg" alt="Chef Venkat">
            <div class="chef-details">
                <h1>Mr. Vennkat</h1>
                <h2>Designation: Executive Chef</h2>
                <h3>Experience: 7 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="koushik chef.jpg" alt="Chef koushik">
            <div class="chef-details">
                <h1>Mr. koushik</h1>
                <h2>Designation: Saucier Chef</h2>
                <h3>Experience: 2 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="seema chef.jpg" alt="Chef seema">
            <div class="chef-details">
                <h1>Miss seema</h1>
                <h2>Designation: Pastry Chef</h2>
                <h3>Experience: 3 years</h3>
            </div>
        </div>

        <div class="chef-card">
            <img src="santha babu.jpg" alt=" leaner santha babu">
            <div class="trainer">
                <h1>Mr santha babu</h1>
                <h2>Designation: Pastry Chef</h2>
                <h3>Experience: 1 year</h3>
            </div>
        </div>
    </div>
    
   
    <footer>
        <p>&copy; 2024 Foodie's Paradise. All rights reserved.</p>
    </footer>

</body>
</html>

contact.html

<html>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&display=swap" rel="stylesheet">
        <title>Contact Us</title>
        <style>
            #n1{
                position: relative;
                color:chartreuse;
                font-size: 60px;
                padding-left: 380px;
                left: 0px;
                top: 190px;
                letter-spacing: 5px;
            }
            body{
                background-image: url("contact image.avif");
                background-repeat: no-repeat;
                background-size: 1700px 950px;
            }
            #n2{
                position:relative;
                color: aliceblue;
                font-size: 80px;
                padding-left: 480px;
                top: 140px;
                letter-spacing: 3px;
                font-family: "Dancing Script", cursive;
            }
            #n3{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                top: 255px;
                padding-left: 240px;
            }
            #n4{
                position: relative;
                color:darkmagenta;
                font-size:31px;
                top: 205px;
                padding-left: 170px;
                letter-spacing: 2px;
            }
            #n5{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                top: 60px;
                padding-left: 680px;
            }
            #n6{
                position: relative;
                color:crimson;
                font-size:35px;
                top: 8px;
                padding-left: 505px;
            }
            #n7{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                bottom: 135px;
                padding-left: 1155px;
            }
            #n8{
                position: relative;
                color:darksalmon;
                font-size: 31px;
                bottom: 187px;
                padding-left: 950px;
                text-align: center;
            }

           
            a {
                color:hotpink;
                text-decoration: none;
                cursor: pointer;
            }

      
            a:hover {
                text-decoration: underline;
            }
            
        </style>
    </head>
    <body>
        <h1 id="n1">With Your Love And Kindness</h1>
        <h2 id="n2">Quality and Taste</h2>
        <h5 id="n3">Phone:</h5>
        <h5 id="n4">
            <a href="tel:+918877445522">+91 8877445522</a>
        </h5>
        <h5 id="n5">Email:</h5>
        <h5 id="n6">
            <a href="mailto:djrestaurant@gmail.com"><b>djrestaurant@gmail.com</b></a>
        </h5>
        <h5 id="n7">Location:</h5>
        <h5 id="n8">
            <a href="dj restarurant"><b> dj restaurant in chennai-600 035</b></a>
        </h5>
    </body>
</html>

```

## OUTPUT:
![alt text](<Screenshot 2024-12-12 201728.png>) 

![alt text](<Screenshot 2024-12-12 201715.png>) 
![alt text](<Screenshot 2024-12-12 201739.png>) 
![alt text](<Screenshot 2024-12-12 201751.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
