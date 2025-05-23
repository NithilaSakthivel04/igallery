# Ex.08 Design of Interactive Image Gallery
## Date:20/05/2025

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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Cricket Image Gallery</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #3e89cb;
      margin: 0;
      padding: 20px;
      text-align: center;
    }

    h1 {
      color: #2810dd;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      margin-top: 30px;
    }

    .gallery img {
      width: 100%;
      border-radius: 10px;
      cursor: pointer;
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    .popup {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      background-color: rgba(0,0,0,0.8);
      justify-content: center;
      align-items: center;
    }

    .popup img {
      max-width: 90%;
      max-height: 90%;
      border: 5px solid white;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <h1>Cricket Image Gallery 🏏</h1>

  <div class="gallery">
    <img src="cricketer1.jpg" alt="Cricket 1">
    <img src="cricketer2.jpg" alt="Cricket 2">
    <img src="cricketer3.jpg" alt="Cricket 3">
    <img src="cricketer4.jpg" alt="Cricket 4">
    <img src="cricketer5.jpg" alt="Cricket 5">
    <img src="cricketer6.jpg" alt="Cricket 6">
    <img src="cricketer7.jpg" alt="Cricket 7">
    <img src="cricketer8.jpg" alt="Cricket 8">
    <img src="cricketer9.jpg" alt="Cricket 9">
    <img src="cricketer10.jpg" alt="Cricket 10">
    <img src="cricketer11.jpg" alt="Cricket 11">
    <img src="cricketer12.jpg" alt="Cricket 12">
  </div>

  <div class="popup" id="popup">
    <img id="popup-img" src="" alt="Popup Image">
  </div>

  <script>
    const images = document.querySelectorAll('.gallery img');
    const popup = document.getElementById('popup');
    const popupImg = document.getElementById('popup-img');

    images.forEach(image => {
      image.addEventListener('click', () => {
        popup.style.display = 'flex';
        popupImg.src = image.src;
      });
    });

    popup.addEventListener('click', () => {
      popup.style.display = 'none';
    });
  </script>
  <footer>
  <p style="text-align: center; color: rgb(6, 6, 6); font-size: 14px;">
    Designed by Nithila S
  </p>
</footer>
</body>
</html>

```
## OUTPUT:
![alt text](<Screenshot (18).png>)
![alt text](<Screenshot (19).png>)
![alt text](<Screenshot (20).png>)
![alt text](<Screenshot (21).png>)
![alt text](<Screenshot (22).png>)
![alt text](<Screenshot (23).png>)
![alt text](<Screenshot (24).png>)
![alt text](<Screenshot (25).png>)
![alt text](<Screenshot (26).png>)
![alt text](<Screenshot (27).png>)
![alt text](<Screenshot (28).png>)
![alt text](<Screenshot (29).png>)
![alt text](<Screenshot (30).png>)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
