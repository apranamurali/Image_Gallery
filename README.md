# Ex.08 Design of Interactive Image Gallery
# Date: 19/11/2025

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
<html>
    <title>Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 0;
            background-size: cover;
            background-image: url('background.png');
            padding: 20px;
            min-height: 100vh;
            position: relative;
        }

        h1 {
            margin-top: 20px;
            color: rgb(22, 7, 26);
            font-size: xx-large;
            font-weight: bold;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            max-width: 800px;
            width: 100%;
            margin-top: 20px;
        }

        .photo {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            cursor: pointer;
        }

        .photo img {
            width: 150px;
            height: auto;
            border-radius: 8px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .photo img:hover {
            transform: scale(1.2);
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5);
        }

        .photo p {
            margin-top: 5px;
            font-size: 14px;
            color: #333;
        }

        footer {
            position: absolute;
            bottom: 0;
            width: 100%;
            text-align: center;
            background-color: rgba(0, 0, 0, 0.7);
            color: #fff;
            padding: 10px 0;
            font-size: 14px;
        }
    </style>

    <body>
        <h1>IMAGE GALLERY</h1>
        <div class="gallery">
            <div class="photo" onclick="openImage('god.jpg')">
                <img src="god.jpg" alt="Muruga">
                <p>Muruga</p>
            </div>
            <div class="photo" onclick="openImage('vijay.jpg')">
                <img src="vijay.jpg" alt="Thalapathy">
                <p>Thalapathy</p>
            </div>
            <div class="photo" onclick="openImage('dhoni.jpg')">
                <img src="dhoni.jpg" alt="Dhoni">
                <p>Dhoni</p>
            </div>
            <div class="photo" onclick="openImage('music.jpg')">
                <img src="music.jpg" alt="Music">
                <p>Music</p>
            </div>
            <div class="photo" onclick="openImage('movie.jpg')">
                <img src="movie.jpg" alt="Movie">
                <p>Movie</p>
            </div>
            <div class="photo" onclick="openImage('rapunzel.jpg')">
                <img src="rapunzel.jpg" alt="Rapunzel">
                <p>Rapunzel</p>
            </div>
            <div class="photo" onclick="openImage('bike.jpg')">
                <img src="bike.jpg" alt="Bike">
                <p>Bike</p>
            </div>
        </div>

        <footer>
            &copy; 2025 Designed and Developed by Roshini A.
        </footer>

        <script>
            function openImage(src) {
                const newWindow = window.open("", "_blank");
                newWindow.document.write(`
                    <html>
                        <head><title>Image Preview</title></head>
                        <body style="margin:0;display:flex;align-items:center;justify-content:center;height:100vh;background-color:#000;">
                            <img src="${src}" style="max-width:100%;max-height:100%;">
                        </body>
                    </html>
                `);
            }
        </script>
    </body>
</html>
```

## OUTPUT
<img width="1006" height="637" alt="Screenshot 2025-11-19 113412" src="https://github.com/user-attachments/assets/2e5c929e-3cd9-4915-ab51-2ec2d22090db" />
<img width="1009" height="630" alt="Screenshot 2025-11-19 113418" src="https://github.com/user-attachments/assets/bf42bc12-8985-45ee-b116-e16282ea020a" />



## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
