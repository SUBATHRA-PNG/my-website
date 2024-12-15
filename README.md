<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.5">
    <title>Journey Through Malaysia</title>
    <!-- Link to Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@1,500&family=Syne:wght@700&family=Poppins:wght@300;500&display=swap" rel="stylesheet">
    <style>
        /* Reset Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body Styles */
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f4f4f4;
        }
       
        /* Navigation Bar */
        .navbar {
            background-color: #444;
            display: flex;
            justify-content: space-around;
            padding: 15px 25px;
            position: sticky;
            top: 0;
            z-index: 10;
            border-bottom: 2px solid;
        }

        .navbar a {
            color: white;
            text-decoration: none;
            font-family: 'Syne', sans-serif;
            padding: 10px 20px;
            font-size: 18px;
            font-weight: bold;
            transition: background 0.3s ease, color 0.3s ease;
        }

        .navbar a:hover {
            background-color: #ddd;
            color: black;
            border-radius: 8px;
        }

       /* Animated Hero Section */
        .hero {
            height: 100vh;
            background: url('twin-tower_edited.jpg') no-repeat center center/cover;
            animation: moveBackground 12s infinite linear;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            position: relative;
            overflow: hidden;
        }
          @keyframes 
     moveBackground {
           0% {

     background-position: center 
top;
           }
           50% {

     background-position: center 
center;
           }
           100% {
     background-postion: center 
bottom;
           }
         }
             
        /* Hero Overlay */
        .hero::before {
            content: "";
            position: absolute;
            top: 0px;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5); /* Dark overlay */
        }

        .hero-content {
            z-index: 2;
        }

        .hero h1 {
            font-family: 'Syne', sans-serif;
            font-size: 5em;
            margin-bottom: 20px;
        }

        .hero h1 span:nth-child(2) {
            font-family: 'Playfair Display', serif;
            font-style: italic;
            color: lightpink;
        }

        .hero p {
            font-size: 1.5em;
            margin-top: 10px;
            text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.5);
        }

        /* Section Styling */
        section {
            padding: 70px;
            text-align: center;
        }

        section img, section video {
            max-width: 100%;
            height: auto;
            margin-top: 20px;
            border-radius: 10px;
        }

        .explore-btn {
            margin-top: 30px;
            font-family: 'Syne', sans-serif;
            font-size: 1em;
            padding: 10px 20px;
            background-color: lightblue;
            text-decoration: none;
            border-radius: 8px;
            color: black;
            transition: transform 0.3s ease, background-color 0.3s ease;
        }

        .explore-btn:hover {
            transform: scale(1.1);
            background-color: darkblue;
            color: white;
        }
    </style>
    <script>
        function showExploreContent() {
            document.getElementById('about-malaysia').style.display = 'block';
        }

        function showExploreMoreContent() {
            document.getElementById('explore-more-content').style.display = 'block';
        }
    </script>
</head>
<body>
    <!-- Navigation Bar -->
    <div class="navbar">
        <a href="#cultural-highlights">Cultural Highlights</a>
        <a href="#wonders">Natural Wonders</a>
        <a href="#cuisine">Cuisine</a>
        <a href="#travel-guide">Travel Guide</a>
    </div>

    <!-- Hero Section -->
    <div class="hero">
        <div class="hero-content">
            <h1><span>Journey</span> <span>Through</span> <span>Malaysia</span></h1>
            <p>Discover the rich culture and heritage of Malaysia</p>
            <br>
            <a href="malaysia-inroduction.html" class="explore-btn">Explore</a>
        </div>
    </div>

    <!-- About Malaysia Section -->
    <section id="about-malaysia" style="display: none;">
        <h2>About Malaysia</h2>
        <p>Malaysia is a beautiful country located in Southeast Asia, known for its diverse culture, breathtaking landscapes, and rich history.</p>
        <img src="about-malaysia.jpg" alt="Malaysia">
        <video controls>
            <source src="malaysia-intro.mp4" type="video/mp4">
        </video>
        <button class="explore-btn" onclick="showExploreMoreContent()">Explore More</button>
    </section>

    <!-- Sections -->
    <section id="cultural-highlights">
        <h2>Malaysia Cultural Highlights</h2>
        <br>
        <p> ~ Malaysia is a melting  pot of cultures,celebrating Malay,Chinese,Indian,and indigenous traditions.~ </p></br>
        <img src="malaysia culture.jpg" alt="Cultural celebration">
        <br>
        <br>
        <a href="cultural_festival.html" class="explore-btn">Explore More</a> 
        </br>       
    </section>

    <section id="wonders">
        <h2>Malaysia Natural Wonders</h2>
        <br>
        <p> ~ Malaysia is a treasure trove of natural wonders,offering everything from pristine rainforests and majestic mountains to idyllic islands and exotic wildlife.~ </p></br>
        <img src="natural wonders.jpg" alt="Natural Wonders">
        <br>
        <br>
        <a href="malaysia_natural _wonder.html"  class="explore-btn">Explore More</a> 
        </br>
    </section>

    <section id="cuisine">
        <h2>Malaysia Cuisine</h2>
        <br>
        <p> ~ Malaysia's culinary scene reflects its multicultural roots, combining flavors from Malay, Chinese, Indian, and indigenous communities.Each dish tells a story of the nation's rich history and cultural fusion.~ </p></br>
        <img src="malaysian foods.jpg" alt="Cuisine">
        <br>
        <br>
        <a href="malaysian_cuisine.html" class="explore-btn">Explore More</a>
        </br> 
    </section>

    <section id="travel-guide">
        <h2>Malaysia Travel Guide</h2>
        </br>
        <p> ~ Malaysia is a traveler's paradise, offering a mix modern cities,historical landmarks, lush rainforests, pristine beaches, and vibrant cultures.~ </p>
        <img src="malaysia travel guide.jpg" alt="Travel Guide">
        <br>
        <br>
        <a href="travel_guide.html"  class="explore-btn">Explore More</a> 
        </br>
    </section>


   </body>
   </html>
