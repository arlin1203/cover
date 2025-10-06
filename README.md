# Ex.06 Book Front Cover Page Design
## Date:06/10/2025

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Book Cover with Photos</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
            overflow: hidden; /* Prevent scrollbars if cover is slightly off-center */
        }

        .book-cover {
            width: 300px;
            height: 450px;
            position: relative; /* Essential for positioning child elements (like images) */
            box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5);
            font-family: 'Georgia', serif;
            text-align: center;
            border-radius: 5px; /* Slightly rounded corners for a modern feel */
            overflow: hidden; /* Ensures background image doesn't spill out */
        }

        .background-photo {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover; /* Covers the entire div without distorting aspect ratio */
            filter: brightness(60%) contrast(110%); /* Darken and add contrast to make text pop */
            z-index: 1; /* Place behind text */
        }

        .author-photo {
            position: absolute;
            bottom: 20px; /* Position from the bottom */
            left: 50%; /* Center horizontally */
            transform: translateX(-50%); /* Adjust for true centering */
            width: 60px; /* Size of the author photo */
            height: 60px;
            border-radius: 50%; /* Makes the photo circular */
            border: 3px solid #FFD700; /* Gold border around the author photo */
            object-fit: cover;
            z-index: 3; /* Place above text and background */
        }

        .cover-content {
            position: relative; /* Establishes new stacking context for its children */
            z-index: 2; /* Place text content above background image */
            display: flex;
            flex-direction: column;
            justify-content: space-between; /* Pushes title up, author down */
            height: 100%; /* Make content fill the cover */
            padding: 20px;
            box-sizing: border-box; /* Include padding in height calculation */
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7); /* Adds shadow to text for readability */
        }

        .book-title {
            color: #FFD700; /* Gold text */
            font-size: 2.2em;
            font-weight: bold;
            text-transform: uppercase;
            line-height: 1.1;
            margin-top: 30px; /* Space from the top */
        }

        .book-subtitle {
            color: #FFFFFF; /* White text */
            font-size: 1.1em;
            margin-top: 10px;
            flex-grow: 1; /* Allows subtitle area to take up available space */
            display: flex;
            align-items: center; /* Vertically center subtitle if it's short */
            justify-content: center;
        }

        .book-author {
            color: #FFD700; /* Gold text */
            font-size: 1.4em;
            font-style: italic;
            margin-bottom: 120px; /* Space above author photo */
        }
    </style>
</head>
<body>

    <div class="book-cover">
        <img src="background.jpg" alt="Book Background" class="background-photo">

        <img src="photo.jpg" alt="Author's Photo" class="author-photo">

        <div class="cover-content">
            <h1 class="book-title">The Legend of the Crimson Quill</h1>
            <h2 class="book-subtitle">A Thrilling Tale of Magic and Betrayal Across Kingdoms</h2>
            <p class="book-author">Arlin R</p>
        </div>
    </div>

</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot 2025-10-06 132838.png>)

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
