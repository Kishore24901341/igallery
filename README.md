# Ex.08 Design of Interactive Image Gallery
## Date:15:12:2024

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
gallery.html:


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: 'Playfair Display', serif;
            margin: 0;
            background: linear-gradient(to bottom right, #2c3e50, #34495e); /* Dark gradient background */
            color: #f1f2f6;
            background-blur: 10px;
        }
        h1 {
            text-align: center;
            margin: 50px 0;
            font-size: 3rem;
            color: #f1c40f;
            text-transform: uppercase;
            font-weight: bold;
            letter-spacing: 3px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        .gallery-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            padding: 30px;
            max-width: 1300px;
            margin: 0 auto;
        }
        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 12px;
            cursor: pointer;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            filter: grayscale(20%) contrast(1.1);
            transition: filter 0.3s ease;
        }
        .gallery-item:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.6);
        }
        .gallery-item:hover img {
            filter: grayscale(0) contrast(1.2);
        }
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.4);
            color: #f1c40f;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.4s ease;
        }
        .gallery-item:hover .overlay {
            opacity: 1;
        }
        .overlay-text {
            font-size: 2rem;
            text-transform: uppercase;
            font-weight: bold;
            letter-spacing: 2px;
        }
        footer {
            text-align: center;
            padding: 15px;
            color: #f1c40f;
            background: #2f3640;
            font-size: 1rem;
            font-weight: bold;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery-container">
        <div class="gallery-item">
            <img src="R (1).jpeg" alt="Photo 1">
            <div class="overlay">
                <div class="overlay-text">Photo 1</div>
            </div>
        </div>
        <div class="gallery-item">
            <img src="vijayakanth-new-photos-91560.jpg" alt="Photo 2">
            <div class="overlay">
                <div class="overlay-text">Photo 2</div>
            </div>
        </div>
        <div class="gallery-item">
            <img src="56d85d61d4e0fda0a1a9e96d1dc7a6e7.jpg" alt="Photo 3">
            <div class="overlay">
                <div class="overlay-text">Photo 3</div>
            </div>
        </div>
        <div class="gallery-item">
            <img src="R.png" alt="Photo 4">
            <div class="overlay">
                <div class="overlay-text">Photo 4</div>
            </div>
        </div>
    </div>

    <footer>
        Designed by Kishore
    </footer>
</body>
</html>


```

## OUTPUT:
![image](https://github.com/user-attachments/assets/0bf932d7-a6a6-4aec-810e-67d092881d6d)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
