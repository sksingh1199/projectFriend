<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Slider Using HTML and CSS</title>
    <link rel="stylesheet" href="style9.css">
</head>
<body onload="slider()">
    <div class="banner">
        <div class="slider">
            <img src="Folder\image1.jpg" id="slideImg">
        </div>
        <div class="overlay">
            <div class="navbar">
                <div class="logo">
                    <img src="Folder\logo.png">
                </div>
                <div class="menu-icons">
                    <img src="Folder\user.png">
                    <img src="Folder\cart.png">
                    <img src="Folder\menu.png">
                </div>
            </div>

            <div class="content">
                <h1>LET'S START TO DESIGN</h1>
                <h3>Subscribe Easy Tutorials YouTude channel to watch more videos, press the bell icon to get latest updates.</h3>
                
                <div>
                    <button type="button">WATCH MORE</button>
                    <button type="button" class="btn-2">SUBSCRIBE</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        var slideImag = document.getElementById("slideImg");
        var images = new Array(
            "Folder/image1.jpg",
            "Folder/image2.jpg",
            "Folder/image3.jpg",
            "Folder/image4.jpg",
            "Folder/image5.jpg", 
            "Folder/image6.jpg"
        );
    var len = images.length;
    var i = 0;
    function slider(){
        if(i > len-1){
            i = 0;
        }
        slideImag.src = images[i];
        i++;
        setTimeout('slider()',3000);
    }
    </script>

</body>
</html>
