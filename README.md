# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Image Gallery</title>
  <style>
    body {
  font-family: Arial, sans-serif;
  background-color: #f3f3f3;
  margin: 0;
  padding: 0;
}

.gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  padding: 20px;
  justify-content: center;
}

.gallery-item {
  width: 200px;
  height: auto;
  cursor: pointer;
  border: 2px solid #ddd;
  transition: transform 0.2s;
}

.gallery-item:hover {
  transform: scale(1.05);
}

.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  justify-content: center;
  align-items: center;
}

.modal-content {
  max-width: 80%;
  max-height: 80%;
}

.close {
  position: absolute;
  top: 20px;
  right: 30px;
  font-size: 30px;
  color: white;
  cursor: pointer;
}

  </style>
  <script>
    function openModal(image) {
  const modal = document.getElementById('imageModal');
  const modalImg = document.getElementById('modalImage');
  
  modal.style.display = "flex";
  modalImg.src = image.src;
}

function closeModal() {
  const modal = document.getElementById('imageModal');
  modal.style.display = "none";
}

  </script>
</head>
<body>
  <div class="gallery">
    <img src="c:\Users\admin\Desktop\image 1 new web.jpeg" alt="Image 1" class="gallery-item" onclick="openModal(this)">
    <img src="c:\Users\admin\Desktop\image 2 new web.jpeg" alt="Image 2" class="gallery-item" onclick="openModal(this)">
    <img src="c:\Users\admin\Desktop\image 3 web.jpeg" alt="Image 3" class="gallery-item" onclick="openModal(this)">
    <img src="c:\Users\admin\Desktop\image 4 web.jpeg" alt="Image 4" class="gallery-item" onclick="openModal(this)">
    <img src="c:\Users\admin\Desktop\image 5 web.jpeg" alt="Image 5" class="gallery-item" onclick="openModal(this)">

  </div>

  <!-- Modal -->
  <div id="imageModal" class="modal" onclick="closeModal()">
    <span class="close">&times;</span>
    <img class="modal-content" id="modalImage">
  </div>

  <script src="script.js"></script>
</body>
</html>
```

## OUTPUT
![image](https://github.com/user-attachments/assets/aa46f2a2-fdc2-420d-9d3b-11018c0e8f76)


## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
