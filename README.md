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
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Interactive Photo Gallery</h1>

    <div class="gallery-container">
        <div class="gallery-item" onclick="openLightbox('R (1).jpeg')">
            <img src="R (1).jpeg" alt="Photo 1">
        </div>
        <div class="gallery-item" onclick="openLightbox('vijayakanth-new-photos-91560.jpg')">
            <img src="vijayakanth-new-photos-91560.jpg" alt="Photo 2">
        </div>
        <div class="gallery-item" onclick="openLightbox('56d85d61d4e0fda0a1a9e96d1dc7a6e7.jpg')">
            <img src="56d85d61d4e0fda0a1a9e96d1dc7a6e7.jpg" alt="Photo 3">
        </div>
        <div class="gallery-item" onclick="openLightbox('R.png')">
            <img src="R.png" alt="Photo 4">
        </div>
        <div class="gallery-item" onclick="openLightbox('R.jpeg')">
            <img src="R.jpeg" alt="Photo 5">
        </div>
    </div>

    <div id="lightbox" onclick="closeLightbox()">
        <span id="close-btn">&times;</span>
        <img id="lightbox-img" src="" alt="Enlarged Photo">
    </div>

    <footer>
        Designed by Kishore
    </footer>

    <script src="script.js"></script>
</body>
</html>


style css :

body {
    font-family: 'Playfair Display', serif;
    margin: 0;
    background: linear-gradient(to bottom right, #2c3e50, #34495e);
    color: #f1f2f6;
}

h1 {
    text-align: center;
    margin: 50px 0;
    font-size: 3rem;
    color: #f1c40f;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: 3px;
}

.gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 30px;
    max-width: 1200px;
    margin: 0 auto;
}

.gallery-item {
    position: relative;
    overflow: hidden;
    border-radius: 12px;
    cursor: pointer;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.gallery-item:hover {
    transform: scale(1.05);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.6);
}

#lightbox {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.95);
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 1000;
}

#lightbox img {
    max-width: 90%;
    max-height: 90%;
    border: 5px solid #f1c40f;
    border-radius: 10px;
}

#close-btn {
    position: absolute;
    top: 20px;
    right: 30px;
    font-size: 2.5rem;
    color: #f1c40f;
    cursor: pointer;
}

footer {
    text-align: center;
    padding: 15px;
    color: #f1c40f;
    background: #2f3640;
    font-size: 1rem;
}


script.js:

function openLightbox(imageSrc) {
    const lightboxImg = document.getElementById('lightbox-img');
    const lightbox = document.getElementById('lightbox');

    lightboxImg.src = imageSrc;
    lightbox.style.display = 'flex';
}

function closeLightbox() {
    const lightbox = document.getElementById('lightbox');
    lightbox.style.display = 'none';
}



```

## OUTPUT:
![image](https://github.com/user-attachments/assets/0bf932d7-a6a6-4aec-810e-67d092881d6d)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
