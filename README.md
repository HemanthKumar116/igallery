# Ex.08 Design of Interactive Image Gallery
## Date:21/05/2025

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
<html>
<head>
  <style>
    body {
      background: black;
      color: white;
      text-align: center;
      font-family: Arial;
    }
    .gallery img {
      width: 150px;
      height: 100px;
      margin: 10px;
      cursor: pointer;
      transition: transform 0.3s;
      border: 2px solid white;
    }
    .gallery img:hover {
      transform: scale(1.1);
    }
    #popup {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.9);
      justify-content: center;
      align-items: center;
    }
    #popup img {
      max-width: 90%;
      max-height: 90%;
    }
    footer {
      margin-top: 50px;
      font-size: 14px;
      color: white;
    }
  </style>
</head>
<body>

  <h2>Click an image to zoom</h2>

  <div class="gallery">
    <img src="2017-Rolls-Royce-Dawn-001-1600.jpg" onclick="zoom(this.src)">
    <img src="2025-Novitec-Ferrari-SF90-XX-Stradale-001-2160.jpg" onclick="zoom(this.src)">
    <img src="luxurious-car-parked-highway-with-illuminated-headlight-sunset.jpg" onclick="zoom(this.src)">
    <img src="off-road-car-fantasy-scenario.jpg" onclick="zoom(this.src)">
    <img src="porsche-911-autumn-drive.jpg" onclick="zoom(this.src)">
  </div>

  <div id="popup" onclick="closeZoom()">
    <img id="zoomedImg">
  </div>

  <footer>
    Designed by: Hemanth Kumar S 212224040115
  </footer>

  <script>
    function zoom(src) {
      document.getElementById('zoomedImg').src = src;
      document.getElementById('popup').style.display = 'flex';
    }
    function closeZoom() {
      document.getElementById('popup').style.display = 'none';
    }
  </script>

</body>
</html>
```
## OUTPUT:

![alt text](<Screenshot (373).png>)

![alt text](<Screenshot (374).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
