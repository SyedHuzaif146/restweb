# Ex.07 Restaurant Website
## Date: 03.05.2025

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
#### home.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>McDonald's</title>
    <style>
        /* Reset and full height layout */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html, body {
            height: 100%;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: url('bg.jpg') no-repeat center center fixed;
            background-size: cover;
            display: flex;
            flex-direction: column;
        }

        /* Center container */
        .container {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 40px 20px;
            background-color: rgba(255, 255, 255, 0.92); /* semi-transparent background */
        }

        .container h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
            color: #da291c; /* McDonald's red */
        }

        .container p {
            font-size: 1.3rem;
            color: #333;
        }

        .button-group {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }

        .btn {
            background-color: #ffbc0d; /* McDonald's yellow */
            color: #000;
            padding: 0.8rem 1.5rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #f5a700;
        }

        footer {
            text-align: center;
            padding: 15px;
            background-color: #f1f1f1;
            font-size: 0.9rem;
            color: #555;
        }
       

    </style>
</head>
<body>
    

    <div class="container">
        <h1>Welcome to McDonald's</h1>
        <p>i'm lovin' it</p>
        <div class="button-group">
            <a href="about.html" class="btn">About</a>
            <a href="menu.html" class="btn">Menu</a>
            <a href="contact.html" class="btn">Contact Us</a>
        </div>
    </div>

    <footer>
        Designed and Developed by SHRIRAM VR
    </footer>

</body>
</html>
```
#### ABBOUT.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>About Us - McDonald's</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      background-color: #fffbe6;
      color: #333;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    header {
      background-color: #d70000;
      color: white;
      text-align: center;
      padding: 50px 20px 30px;
    }

    header h1 {
      font-size: 2.5rem;
    }

    header p {
      font-size: 1.1rem;
      margin-top: 10px;
    }

    .content {
      flex: 1;
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
      text-align: center;
    }

    .content h2 {
      font-size: 2rem;
      margin-bottom: 30px;
      color: #d70000;
    }

    .about-container {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .about-text {
      text-align: justify;
      font-size: 1rem;
      max-width: 800px;
      margin-bottom: 30px;
    }

    .about-image {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    footer {
      background-color: #f8f9fa;
      padding: 15px;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
    }

    @media (min-width: 768px) {
      .about-container {
        flex-direction: row;
        gap: 40px;
        justify-content: space-between;
      }

      .about-text {
        flex: 1;
      }

      .about-image {
        flex: 1;
        max-width: 400px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to McDonald’s</h1>
    <p>Serving smiles and iconic flavors since 1940.</p>
  </header>

  <div class="content">
    <h2>About Us</h2>
    <div class="about-container">
      <div class="about-text">
        <p>
          The story of McDonald's began in 1940 when Richard and Maurice McDonald opened the first McDonald's restaurant in San Bernardino, California. Their innovative approach to fast food service laid the foundation for what would become the world’s largest restaurant chain.
        </p>
        <p>
          In 1955, Ray Kroc joined the company and transformed McDonald's into a global franchise, emphasizing consistency, quality, and speed. From the classic Big Mac to crispy fries, McDonald’s has become synonymous with delicious, reliable meals across cultures.
        </p>
        <p>
          Today, McDonald’s operates in over 100 countries, offering a blend of international and local flavors, all while maintaining a commitment to quality, sustainability, and community impact. Whether you're grabbing a quick meal or enjoying time with family, McDonald’s remains a place where great food meets great memories.
        </p>
      </div>
      <img src="founder.jpg" alt="McDonald's Founders" class="about-image" />
    </div>
  </div>

  <footer>
    Designed and Developed by SHRIRAM VR
  </footer>

</body>
</html>
```

#### CONTACT.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contact Us - McDonald's</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #fffdf3;
      color: #333;
    }

    header {
      background-color: #d70000;
      color: white;
      padding: 1rem;
      text-align: center;
    }

    .container {
      max-width: 800px;
      margin: 2rem auto;
      padding: 1rem;
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      color: #d70000;
    }

    .contact-info {
      margin-bottom: 2rem;
    }

    .contact-info p {
      margin: 0.5rem 0;
    }

    form {
      display: flex;
      flex-direction: column;
    }

    label {
      margin: 0.5rem 0 0.2rem;
    }

    input, textarea {
      padding: 0.6rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 1rem;
    }

    textarea {
      resize: vertical;
    }

    button {
      margin-top: 1rem;
      background-color: #ffc72c;
      color: #000;
      padding: 0.7rem;
      border: none;
      border-radius: 4px;
      font-size: 1rem;
      cursor: pointer;
      font-weight: bold;
    }

    button:hover {
      background-color: #ffb300;
    }

    footer {
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
      background-color: #f1f1f1;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Contact McDonald's</h1>
  </header>

  <div class="container">
    <section class="contact-info">
      <h2>Get in Touch</h2>
      <p><strong>Address:</strong> McDonald’s India HQ, West Avenue, Mumbai, Maharashtra - 400001</p>
      <p><strong>Phone:</strong> 1800-123-4567</p>
      <p><strong>Email:</strong> support@mcdonaldsindia.com</p>
      <p><strong>Hours:</strong> 10:00 AM - 10:00 PM, All Days</p>
    </section>

    <section class="feedback-form">
      <h2>We Value Your Feedback</h2>
      <form action="#" method="POST">
        <label for="name">Your Name</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Your Email</label>
        <input type="email" id="email" name="email" required />

        <label for="message">Your Feedback</label>
        <textarea id="message" name="message" rows="5" required></textarea>

        <button type="submit">Submit Feedback</button>
      </form>
    </section>
  </div>

  <footer>
    &copy; 2025 McDonald's. All rights reserved.<br>
    Designed and Developed by SHRIRAM VR
  </footer>
</body>
</html>
```
## OUTPUT:
#### HOME.HTML
![alt text](<Screenshot 2025-05-03 093600.png>)

#### MENU.HTML
![alt text](<Screenshot 2025-05-03 093615.png>)

#### MENU.HTML
![alt text](<Screenshot 2025-05-03 093629.png>)
![alt text](<Screenshot 2025-05-03 093641.png>)

#### CONTACT.HTML
![alt text](<Screenshot 2025-05-03 093652.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
