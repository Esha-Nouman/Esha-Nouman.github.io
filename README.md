<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Esha | Portfolio</title>
    <style>
        /* --- 1. ANIMATED GRADIENT BACKGROUND --- */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: white;
            /* The colors that the background will shift through */
            background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            overflow-x: hidden;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* --- 2. TEXT ENTRANCE ANIMATIONS --- */
        .intro-container {
            text-align: center;
            animation: slideUp 1.5s ease-out;
        }

        @keyframes slideUp {
            0% { transform: translateY(50px); opacity: 0; }
            100% { transform: translateY(0); opacity: 1; }
        }

        h1 {
            font-size: 4.5rem;
            margin-bottom: 10px;
            letter-spacing: 2px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }

        p {
            font-size: 1.5rem;
            font-weight: 300;
            opacity: 0.9;
            animation: fadeIn 3s ease-in;
        }

        @keyframes fadeIn {
            0% { opacity: 0; }
            50% { opacity: 0; } /* Delays the fade-in slightly */
            100% { opacity: 0.9; }
        }

        /* --- 3. WAVING EMOJI ANIMATION --- */
        .wave {
            display: inline-block;
            animation: waving 2.5s infinite;
            transform-origin: 70% 70%;
        }

        @keyframes waving {
            0% { transform: rotate(0.0deg) }
            10% { transform: rotate(14.0deg) }
            20% { transform: rotate(-8.0deg) }
            30% { transform: rotate(14.0deg) }
            40% { transform: rotate(-4.0deg) }
            50% { transform: rotate(10.0deg) }
            60% { transform: rotate(0.0deg) }
            100% { transform: rotate(0.0deg) }
        }

        /* --- 4. FUTURE SECTION BOXES (HIDDEN) --- */
        .future-section {
            display: none; /* This is what keeps them invisible for now */
            width: 80%;
            max-width: 800px;
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            margin-top: 50px;
            border-radius: 15px;
            backdrop-filter: blur(10px); /* Gives a cool frosted glass effect */
        }
    </style>
</head>
<body>

    <div class="intro-container">
        <h1>Hi, I'm Esha <span class="wave">👋</span></h1>
        <p>Welcome to my digital space. More coming soon!</p>
    </div>

    <section id="about" class="future-section">
        <h2>About Me</h2>
        <p>This box is ready for your content later.</p>
    </section>

    <section id="projects" class="future-section">
        <h2>My Projects</h2>
        <p>This box is ready for your content later.</p>
    </section>

    <section id="contact" class="future-section">
        <h2>Contact</h2>
        <p>This box is ready for your content later.</p>
    </section>

</body>
</html>
