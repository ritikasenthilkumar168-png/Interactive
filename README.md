# Ex.08 Design of Interactive Image Gallery
## Date:05.10.2025

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
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Multiple Images Enlarge on Click</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Comic+Neue:wght@700&display=swap');
  body {
    background: linear-gradient(120deg, #ffe7a0 0%, #ffb6b9 100%);
    font-family: 'Comic Neue', 'Comic Sans MS', cursive, sans-serif;
    margin: 0;
    padding: 0;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
  }
  h1 {
    color: #e94f37;
    margin-bottom: 30px;
    text-shadow: 2px 2px 8px #fff;
    font-size: 2.5rem;
    letter-spacing: 2px;
  }
  .shinchan-icon {
    width: 80px;
    height: auto;
    margin-bottom: 10px;
    border-radius: 50%;
    box-shadow: 0 2px 8px rgba(233, 79, 55, 0.15);
    background: #fffbe7;
    border: 2px solid #e94f37;
  }
  .image-container {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
    justify-content: center;
    margin-bottom: 40px;
  }
  .clickable-image {
    width: 150px;
    height: auto;
    margin: 10px;
    cursor: pointer;
    transition: transform 0.3s cubic-bezier(.25,.8,.25,1), box-shadow 0.3s;
    border-radius: 18px;
    box-shadow: 0 2px 8px rgba(233, 79, 55, 0.15);
    border: 3px dashed #e94f37;
    background: #fffbe7;
  }
  .clickable-image:hover {
    box-shadow: 0 4px 16px rgba(233, 79, 55, 0.25);
    border-color: #ffb6b9;
  }
  .enlarged {
    transform: scale(2);
    z-index: 10;
    position: relative;
    box-shadow: 0 8px 32px rgba(233, 79, 55, 0.35);
    border-color: #e94f37;
  }
  .shinchan-note {
    color: #e94f37;
    font-size: 1.1rem;
    margin-bottom: 20px;
    background: #fffbe7;
    padding: 10px 20px;
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(233, 79, 55, 0.10);
    border: 1px solid #ffb6b9;
  }
</style>
</head>
<body>

<img class="shinchan-icon" src="shinchan_icon.png" alt="Shinchan" />
<h1>Shinchan's Fun Gallery</h1>
<div class="shinchan-note">
  <b>Secret messages for you.. silence!🤫🤫</b><br>
  Ready to read? Okeiii... Let's go!😜<br>
</div>
<div class="image-container">
  <div style="display: flex; flex-direction: column; align-items: center;">
    <img class="clickable-image" src="i1.jpeg" alt="Shinchan 1" />
    <div class="shinchan-caption">You are so cute😻🩷.</div>
  </div>
  <div style="display: flex; flex-direction: column; align-items: center;">
    <img class="clickable-image" src="i2.jpeg" alt="Shinchan 2" />
    <div class="shinchan-caption">You are funny😂🤏🏽.</div>
  </div>
  <div style="display: flex; flex-direction: column; align-items: center;">
    <img class="clickable-image" src="i3.jpeg" alt="Shinchan 3" />
    <div class="shinchan-caption">You are smart🧠.</div>
  </div>
  <div style="display: flex; flex-direction: column; align-items: center;">
    <img class="clickable-image" src="i4.jpeg" alt="Shinchan 4" />
    <div class="shinchan-caption">You are so humble🫡(THE GENTLEMAN).</div>
  </div>
  <div style="display: flex; flex-direction: column; align-items: center;">
    <img class="clickable-image" src="i5.jpeg" alt="Shinchan 5" />
    <div class="shinchan-caption">You are so strong💪🏽</div>
  </div>
  <div style="display: flex; flex-direction: column; align-items: center;">
    <img class="clickable-image" src="i7.jpeg" alt="Shinchan 6" />
    <div class="shinchan-caption">You are just perfect in my eyes...(THE DONALD DUCK🦆)😭🎀🫠</div>
  </div>
  .shinchan-caption {
    font-family: 'Comic Neue', 'Comic Sans MS', cursive, sans-serif;
    color: #e94f37;
    background: #fffbe7;
    border-radius: 8px;
    padding: 6px 14px;
    margin-top: 8px;
    font-size: 1.05rem;
    box-shadow: 0 1px 4px rgba(233, 79, 55, 0.10);
    border: 1px solid #ffb6b9;
    text-align: center;
    max-width: 180px;
  }
</div>

<script>
  const images = document.querySelectorAll('.clickable-image');

  images.forEach(img => {
    img.addEventListener('click', () => {
      img.classList.toggle('enlarged');
    });
  });
</script>

</body>
</html>
```

## OUTPUT:


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
