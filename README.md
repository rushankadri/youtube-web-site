<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KRGAMAING | Minecraft Adventures Every Week</title>
    <link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet">
    <style>
        /* Custom Cursor */
        body {
            cursor: url('https://cdn.pixabay.com/photo/2017/08/30/03/57/cursor-2697409_960_720.png'), auto;
        }

        /* General Styles */
        html {
            scroll-behavior: smooth;
        }
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background-color: #121212;
            color: #fff;
            background: url('https://wallpapercave.com/wp/wp13977541.jpg') no-repeat center center fixed;
            background-size: cover; /* Minecraft background */
        }

        header {
            background-color: rgba(31, 31, 31, 0.8); /* semi-transparent for header */
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 10;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 1rem;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #00ff99;
        }

        .hero {
            height: 90vh;
            background: rgba(0, 0, 0, 0.5); /* Dark overlay for text visibility */
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 0.5rem;
            animation: fadeDown 1s ease-in-out;
            text-shadow: 2px 2px 10px rgba(0, 255, 153, 0.7); /* Text shadow */
            transition: transform 0.3s ease-in-out, color 0.3s ease-in-out;
        }

        .hero h1:hover {
            transform: scale(1.1);
            color: #00ff99; /* Hover color effect */
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            animation: fadeUp 1.5s ease-in-out;
            text-shadow: 1px 1px 5px rgba(0, 255, 153, 0.6); /* Text shadow */
            transition: transform 0.3s ease-in-out, color 0.3s ease-in-out;
        }

        .hero p:hover {
            transform: scale(1.05);
            color: #00ff99; /* Hover color effect */
        }

        .hero a {
            padding: 0.75rem 1.5rem;
            background-color: #00ff99;
            color: #121212;
            border-radius: 8px;
            font-weight: bold;
            text-decoration: none;
            transition: background-color 0.3s, transform 0.3s, text-shadow 0.3s;
        }

        .hero a:hover {
            background-color: #00cc77;
            transform: scale(1.05);
            text-shadow: 0px 0px 15px rgba(0, 255, 153, 0.9); /* Hover glow effect */
        }

        .section {
            padding: 4rem 2rem;
            text-align: center;
        }

        .video-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        iframe {
            width: 100%;
            height: 200px;
            border: none;
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        iframe:hover {
            transform: scale(1.03);
            box-shadow: 0px 0px 20px rgba(0, 255, 153, 0.5); /* Add shadow to videos on hover */
        }

        footer {
            background-color: rgba(31, 31, 31, 0.8); /* semi-transparent footer */
            padding: 1rem;
            text-align: center;
            font-size: 0.9rem;
            margin-top: 2rem;
        }

        .contact-btn {
            padding: 0.75rem 1.5rem;
            background-color: #00ff99;
            color: #121212;
            border-radius: 8px;
            font-weight: bold;
            text-decoration: none;
            transition: background-color 0.3s, transform 0.3s, text-shadow 0.3s;
        }

        .contact-btn:hover {
            background-color: #00cc77;
            transform: scale(1.05);
            text-shadow: 0px 0px 15px rgba(0, 255, 153, 0.9); /* Hover glow effect */
        }

        /* Keyframes for animation */
        @keyframes fadeDown {
            0% { opacity: 0; transform: translateY(-30px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeUp {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        /* Cursor Effect - Hover on interactive elements */
        .interactive:hover {
            cursor: pointer;
            transform: scale(1.05);
            box-shadow: 0px 0px 20px rgba(0, 255, 153, 0.5);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">KRGAMAING</div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#videos">Videos</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1 class="interactive">KRGAMAING</h1>
        <p class="interactive">Minecraft Adventures Every Week.</p>
        <a href="https://youtube.com/" target="_blank" class="interactive">Watch Latest Video</a>
    </section>

    <section class="section" id="videos" data-aos="fade-up">
        <h2 class="interactive">Featured Videos</h2>
        <div class="video-grid">
          <iframe src="https://www.youtube.com/embed/jSLK6GYakIs" allowfullscreen></iframe>
          <iframe src="https://www.youtube.com/embed/qJ-0AqFizYg" allowfullscreen></iframe>
          <iframe src="https://www.youtube.com/embed/mUY5tY7GJYc" allowfullscreen></iframe>
          <iframe src="https://www.youtube.com/embed/t3zmWuCczaU" allowfullscreen></iframe>
          <iframe src="https://www.youtube.com/embed/uKDTFah5xq8" allowfullscreen></iframe>
          <iframe src="https://www.youtube.com/embed/tieUSWwIm1k" allowfullscreen></iframe>
        </div>
    </section>

    <section class="section" id="about" data-aos="fade-right">
        <h2 class="interactive">About Me</h2>
        <p class="interactive">Hi,If you're a fan of Minecraft, you're in the right place! Dive into epic 100 Days Minecraft Survival challenges, where I take on tough adventures and try to survive in the blocky world for 100 days. Along with that, I bring you exciting gameplay, tutorials, mods, and live streams where you can interact with the community in real-time!

            Subscribe and join the adventure—let's build, explore, and have fun together as we conquer the Minecraft world one block at a time!</p>
    </section>

    <section class="section" id="contact" data-aos="fade-left">
        <h2 class="interactive">Contact Me</h2>
        <p class="interactive">Interested in collaborating or sponsoring a video? Reach out!</p>
        <a href="mailto:kadrirushan112@gmail.com" class="contact-btn interactive">Email Me</a>
    </section>

    <footer>
        &copy; 2025 KRGAMAING | All Rights Reserved
    </footer>

    <script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>
    <script>
        AOS.init({
            duration: 1000,
            once: true
        });
    </script>
</body>
</html>
