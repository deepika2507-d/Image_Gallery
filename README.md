<img width="1920" height="1200" alt="Screenshot (716)" src="https://github.com/user-attachments/assets/5990847e-ee4e-40bb-a62f-6112755eae4a" /># Ex.07 Design of Interactive Image Gallery

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
IMAGE.HTML
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Image Gallery</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-image: url('bg3.jpg');
            background-repeat: no-repeat;
            background-size: cover;
        }

        header {
            text-align: center;
            font-size: 30px;
            font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            color: white;
        }

        div img {
            width: 300px;
            height: 300px;
            cursor: pointer;
            border-radius: 10px;
        }
        .img{
            overflow: hidden;
        }
        div{
            transition: 0.25s;
        }

        div :hover {
            transform: scale(1.1);
            border-radius: 10px;
        }
        
        
        .col1 {
            display: flex;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }
        .col2 {
            display: flex;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }

        

        span {
            color: white;
            position: absolute;
            top: 5%;
            right: 5%;
            font-size: 50px;
            cursor: pointer;
        }
        #dis{
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.8);
            position: fixed;
            top: 0;
            bottom: 0;
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 100;
        }
        #dis img{
            width: 500px;
            height: 600px;
        }
        .footer{
            text-align: center;
            margin-bottom:5%;
            background-color:whitesmoke;
            color:rgb(11, 10, 10);
            font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            font-size: 25px;
        }
    </style>
    
</head>

<body>
    <header>
        <h1>My Image Gallery</h1>
    </header>
    <section id="dis">
        <img src="bg3.jpg" alt="" id="disimg">
        <span class="cls" onclick="closes()">&times;</span>
        
    </section>
    <div class="col1">
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 185649.png" onclick="opens(this.src)" id="img1" alt="">
        </div>
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 185833.png" onclick="opens(this.src)" id="img2" alt="">
        </div>
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 185947.png" onclick="opens(this.src)" id="img3" alt="">
        </div>
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 190059.png" onclick="opens(this.src)" id="img4" alt="">
        </div>
    </div>
    <div class="col2">
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 190216.png" onclick="opens(this.src)" id="img5" alt="">
        </div>
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 190650.png" onclick="opens(this.src)" id="img6" alt="">
        </div>
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 190823.png" onclick="opens(this.src)" id="img7" alt="">
        </div>
        <div class="img">
            <img src="c:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2026-03-16 191112.png" onclick="opens(this.src)" id="img8" alt="">
        </div>

    </div>
    <div class="footer">
        <footer>
            Designed by DEEPIKA V &copy; 2024 
       </footer>
    </div>
    

    <script>
        var dis=document.getElementById("dis");
        var disimg=document.getElementById("disimg");
        function opens(image){
            dis.style.display="flex";
            disimg.src=image;
        }
        function closes(){
            dis.style.display="none";

        }
    </script>

</body>

</html>

```

## OUTPUT
<img width="1920" height="1200" alt="Screenshot (724)" src="https://github.com/user-attachments/assets/d3f82df1-49ba-4d12-9204-699fab07be76" />

<img width="1920" height="1200" alt="Screenshot (723)" src="https://github.com/user-attachments/assets/115228fb-08cb-4238-ab3c-1d4854ab4478" />

<img width="1920" height="1200" alt="Screenshot (722)" src="https://github.com/user-attachments/assets/b84d4a5b-3d82-4744-92b0-43648d569c94" />

<img width="1920" height="1200" alt="Screenshot (721)" src="https://github.com/user-attachments/assets/2c7abb32-eaf2-4a0d-9b28-60a7d117d76c" />

<img width="1920" height="1200" alt="Screenshot (720)" src="https://github.com/user-attachments/assets/829d4b03-95a2-4b10-a6bf-a0158c9cc402" />

<img width="1920" height="1200" alt="Screenshot (719)" src="https://github.com/user-attachments/assets/3d875473-f56f-47c9-80dc-07eaf20d618c" />

<img width="1920" height="1200" alt="Screenshot (718)" src="https://github.com/user-attachments/assets/222ca74c-3232-4ff2-a149-31146824e25f" />

<img width="1920" height="1200" alt="Screenshot (717)" src="https://github.com/user-attachments/assets/4ee2235d-0f01-4510-9a7d-4fdc176d15a4" />

<img width="1920" height="1200" alt="Screenshot (716)" src="https://github.com/user-attachments/assets/5fadde60-2dd3-41d6-84f7-54fc7e4c4404" />


## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
