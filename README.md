<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Lost Treasure of El Dorado | Unlock Ancient Secrets</title>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Cormorant+Garamond:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #D4AF37;
            --dark-gold: #8B7355;
            --bronze: #CD7F32;
            --deep-brown: #1a0f0a;
            --aged-paper: #f4e9d8;
            --shadow: #0a0604;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(5deg); }
        }

        @keyframes shimmer {
            0% { background-position: -200% center; }
            100% { background-position: 200% center; }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes glowPulse {
            0%, 100% { 
                box-shadow: 0 0 20px var(--gold),
                            0 0 40px var(--gold),
                            0 0 60px var(--bronze),
                            inset 0 0 20px rgba(212, 175, 55, 0.3);
            }
            50% { 
                box-shadow: 0 0 30px var(--gold),
                            0 0 60px var(--gold),
                            0 0 90px var(--bronze),
                            inset 0 0 30px rgba(212, 175, 55, 0.5);
            }
        }

        @keyframes coinFlip {
            0% { transform: rotateY(0deg); }
            100% { transform: rotateY(360deg); }
        }

        @keyframes torchFlicker {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.8; }
        }

        @keyframes revealContent {
            0% {
                opacity: 0;
                transform: scale(0.8) translateY(50px);
                filter: blur(10px);
            }
            100% {
                opacity: 1;
                transform: scale(1) translateY(0);
                filter: blur(0);
            }
        }

        @keyframes celebration {
            0%, 100% { transform: scale(1) rotate(0deg); }
            25% { transform: scale(1.1) rotate(-5deg); }
            75% { transform: scale(1.1) rotate(5deg); }
        }

        body {
            font-family: 'Cormorant Garamond', serif;
            background: linear-gradient(180deg, 
                #0a0604 0%,
                #1a0f0a 30%,
                #2d1810 60%,
                #1a0f0a 100%);
            color: var(--aged-paper);
            overflow-x: hidden;
            position: relative;
            min-height: 100vh;
        }

        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 30%, rgba(212, 175, 55, 0.05) 0%, transparent 50%),
                radial-gradient(circle at 80% 70%, rgba(205, 127, 50, 0.05) 0%, transparent 50%),
                url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMDAiIGhlaWdodD0iMzAwIj48ZmlsdGVyIGlkPSJhIiB4PSIwIiB5PSIwIj48ZmVUdXJidWxlbmNlIGJhc2VGcmVxdWVuY3k9Ii43NSIgc3RpdGNoVGlsZXM9InN0aXRjaCIgdHlwZT0iZnJhY3RhbE5vaXNlIi8+PGZlQ29sb3JNYXRyaXggdHlwZT0ic2F0dXJhdGUiIHZhbHVlcz0iMCIvPjwvZmlsdGVyPjxwYXRoIGQ9Ik0wIDBoMzAwdjMwMEgweiIgZmlsdGVyPSJ1cmwoI2EpIiBvcGFjaXR5PSIuMDUiLz48L3N2Zz4=');
            pointer-events: none;
            z-index: 1;
        }

        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }

        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: var(--gold);
            border-radius: 50%;
            animation: torchFlicker 3s infinite;
        }

        .container {
            position: relative;
            z-index: 2;
            max-width: 1400px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        header {
            text-align: center;
            margin-bottom: 60px;
            animation: fadeInUp 1s ease;
        }

        .ornament {
            width: 120px;
            height: 3px;
            background: linear-gradient(90deg, 
                transparent, 
                var(--gold), 
                var(--bronze), 
                var(--gold), 
                transparent);
            margin: 0 auto 30px;
            position: relative;
        }

        .ornament::before,
        .ornament::after {
            content: '◆';
            position: absolute;
            color: var(--gold);
            font-size: 12px;
            top: -9px;
        }

        .ornament::before {
            left: -15px;
        }

        .ornament::after {
            right: -15px;
        }

        h1 {
            font-family: 'Cinzel', serif;
            font-size: clamp(2.5rem, 8vw, 5rem);
            font-weight: 900;
            background: linear-gradient(135deg, 
                var(--gold) 0%,
                #ffd700 25%,
                var(--bronze) 50%,
                #ffd700 75%,
                var(--gold) 100%);
            background-size: 200% auto;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: shimmer 3s linear infinite;
            text-shadow: 0 0 30px rgba(212, 175, 55, 0.5);
            letter-spacing: 3px;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .subtitle {
            font-size: clamp(1.2rem, 3vw, 1.8rem);
            color: var(--bronze);
            font-style: italic;
            letter-spacing: 2px;
            text-transform: uppercase;
        }

        .hero {
            position: relative;
            background: linear-gradient(135deg, 
                rgba(139, 115, 85, 0.1) 0%,
                rgba(212, 175, 55, 0.05) 100%);
            border: 2px solid var(--dark-gold);
            border-radius: 20px;
            padding: 60px 40px;
            margin-bottom: 60px;
            backdrop-filter: blur(10px);
            box-shadow: 
                0 20px 60px rgba(0, 0, 0, 0.5),
                inset 0 1px 0 rgba(212, 175, 55, 0.2);
            animation: fadeInUp 1s ease 0.2s both;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, 
                var(--gold), 
                var(--bronze), 
                var(--dark-gold), 
                var(--gold));
            background-size: 300% 300%;
            border-radius: 20px;
            z-index: -1;
            opacity: 0.3;
            animation: shimmer 6s ease infinite;
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .map-icon {
            font-size: 120px;
            animation: float 6s ease-in-out infinite;
            display: block;
            margin: 0 auto 30px;
            filter: drop-shadow(0 10px 30px rgba(212, 175, 55, 0.4));
        }

        .hero h2 {
            font-family: 'Cinzel', serif;
            font-size: clamp(2rem, 5vw, 3.5rem);
            color: var(--gold);
            margin-bottom: 25px;
            text-align: center;
            font-weight: 700;
        }

        .story {
            font-size: clamp(1.1rem, 2vw, 1.4rem);
            line-height: 1.8;
            color: var(--aged-paper);
            margin-bottom: 40px;
            text-align: center;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .treasure-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }

        .treasure-item {
            background: linear-gradient(135deg, 
                rgba(26, 15, 10, 0.8) 0%,
                rgba(45, 24, 16, 0.6) 100%);
            border: 1px solid var(--dark-gold);
            border-radius: 15px;
            padding: 35px 25px;
            text-align: center;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
            animation: fadeInUp 1s ease both;
        }

        .treasure-item:nth-child(1) { animation-delay: 0.4s; }
        .treasure-item:nth-child(2) { animation-delay: 0.5s; }
        .treasure-item:nth-child(3) { animation-delay: 0.6s; }
        .treasure-item:nth-child(4) { animation-delay: 0.7s; }

        .treasure-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, 
                transparent, 
                rgba(212, 175, 55, 0.1), 
                transparent);
            transition: left 0.5s;
        }

        .treasure-item:hover::before {
            left: 100%;
        }

        .treasure-item:hover {
            transform: translateY(-10px) scale(1.02);
            border-color: var(--gold);
            box-shadow: 0 20px 40px rgba(212, 175, 55, 0.3);
        }

        .treasure-icon {
            font-size: 4rem;
            margin-bottom: 20px;
            display: block;
            animation: coinFlip 3s ease-in-out infinite;
        }

        .treasure-item h3 {
            font-family: 'Cinzel', serif;
            font-size: 1.5rem;
            color: var(--gold);
            margin-bottom: 15px;
            font-weight: 600;
        }

        .treasure-item p {
            color: var(--aged-paper);
            line-height: 1.6;
            font-size: 1.1rem;
        }

        .lock-container {
            background: radial-gradient(ellipse at center,
                rgba(212, 175, 55, 0.1) 0%,
                rgba(26, 15, 10, 0.9) 70%);
            border: 3px solid var(--gold);
            border-radius: 25px;
            padding: 70px 40px;
            text-align: center;
            position: relative;
            margin: 60px auto;
            max-width: 900px;
            animation: fadeInUp 1s ease 0.8s both, glowPulse 3s ease-in-out infinite;
            box-shadow: 
                0 30px 80px rgba(0, 0, 0, 0.7),
                inset 0 0 50px rgba(212, 175, 55, 0.1);
        }

        .lock-container::before {
            content: '✦';
            position: absolute;
            top: -20px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 40px;
            color: var(--gold);
            text-shadow: 0 0 20px var(--gold);
        }

        .chest-icon {
            font-size: 140px;
            margin-bottom: 30px;
            display: block;
            animation: float 4s ease-in-out infinite;
            filter: drop-shadow(0 15px 40px rgba(212, 175, 55, 0.6));
        }

        .lock-title {
            font-family: 'Cinzel', serif;
            font-size: clamp(2rem, 4vw, 3rem);
            color: var(--gold);
            margin-bottom: 20px;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 3px;
        }

        .lock-description {
            font-size: clamp(1.2rem, 2.5vw, 1.6rem);
            line-height: 1.8;
            color: var(--aged-paper);
            margin-bottom: 45px;
            font-style: italic;
        }

        .unlock-btn {
            font-family: 'Cinzel', serif;
            font-size: 1.4rem;
            font-weight: 700;
            padding: 25px 60px;
            background: linear-gradient(135deg, var(--gold) 0%, var(--bronze) 100%);
            color: var(--deep-brown);
            border: none;
            border-radius: 50px;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 3px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            box-shadow: 
                0 10px 30px rgba(212, 175, 55, 0.5),
                inset 0 1px 0 rgba(255, 255, 255, 0.3);
        }

        .unlock-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, 
                transparent, 
                rgba(255, 255, 255, 0.3), 
                transparent);
            transition: left 0.5s;
        }

        .unlock-btn:hover::before {
            left: 100%;
        }

        .unlock-btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 
                0 15px 40px rgba(212, 175, 55, 0.7),
                inset 0 1px 0 rgba(255, 255, 255, 0.5);
        }

        .unlock-btn:active {
            transform: translateY(-2px) scale(1.03);
        }

        /* Hidden Content Styles */
        .hidden-content {
            display: none;
            opacity: 0;
            margin: 60px auto;
            max-width: 1000px;
        }

        .hidden-content.revealed {
            display: block;
            animation: revealContent 1.5s ease forwards;
        }

        .success-banner {
            background: linear-gradient(135deg, 
                var(--gold) 0%,
                var(--bronze) 100%);
            color: var(--deep-brown);
            padding: 30px 40px;
            border-radius: 20px;
            text-align: center;
            margin-bottom: 40px;
            box-shadow: 0 20px 60px rgba(212, 175, 55, 0.6);
            animation: celebration 0.6s ease;
        }

        .success-banner h2 {
            font-family: 'Cinzel', serif;
            font-size: clamp(2rem, 4vw, 3rem);
            margin-bottom: 15px;
            font-weight: 700;
        }

        .success-banner p {
            font-size: clamp(1.1rem, 2vw, 1.4rem);
            font-style: italic;
        }

        .treasure-revealed {
            background: linear-gradient(135deg, 
                rgba(139, 115, 85, 0.15) 0%,
                rgba(212, 175, 55, 0.08) 100%);
            border: 2px solid var(--gold);
            border-radius: 20px;
            padding: 50px 40px;
            margin-bottom: 30px;
        }

        .treasure-revealed h3 {
            font-family: 'Cinzel', serif;
            font-size: clamp(1.8rem, 3vw, 2.5rem);
            color: var(--gold);
            text-align: center;
            margin-bottom: 40px;
            font-weight: 700;
        }

        .premium-content {
            background: rgba(26, 15, 10, 0.6);
            border-left: 4px solid var(--gold);
            padding: 30px;
            border-radius: 10px;
            margin-bottom: 30px;
        }

        .download-section {
            text-align: center;
            margin-top: 40px;
        }

        .download-btn {
            display: inline-block;
            font-family: 'Cinzel', serif;
            font-size: 1.3rem;
            font-weight: 700;
            padding: 20px 50px;
            background: linear-gradient(135deg, #2ecc71 0%, #27ae60 100%);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            transition: all 0.3s ease;
            box-shadow: 0 10px 30px rgba(46, 204, 113, 0.4);
            margin: 10px;
        }

        .download-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(46, 204, 113, 0.6);
        }

        .content-item {
            background: rgba(26, 15, 10, 0.8);
            border: 1px solid var(--dark-gold);
            border-radius: 15px;
            padding: 25px;
            margin-bottom: 20px;
            transition: all 0.3s ease;
        }

        .content-item:hover {
            border-color: var(--gold);
            transform: translateX(10px);
        }

        .content-item h4 {
            font-family: 'Cinzel', serif;
            color: var(--gold);
            font-size: 1.4rem;
            margin-bottom: 15px;
        }

        .content-item p {
            color: var(--aged-paper);
            line-height: 1.6;
            font-size: 1.1rem;
        }

        footer {
            text-align: center;
            padding: 40px 20px;
            color: var(--dark-gold);
            font-size: 0.95rem;
            letter-spacing: 1px;
            margin-top: 80px;
            border-top: 1px solid var(--dark-gold);
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px 15px;
            }

            .hero {
                padding: 40px 25px;
            }

            .lock-container {
                padding: 50px 25px;
            }

            .unlock-btn {
                padding: 20px 40px;
                font-size: 1.2rem;
            }

            .treasure-grid {
                grid-template-columns: 1fr;
            }

            .download-btn {
                padding: 18px 40px;
                font-size: 1.1rem;
            }
        }
    </style>
</head>
<body>
    <div class="stars" id="stars"></div>

    <div class="container">
        <header>
            <div class="ornament"></div>
            <h1>The Lost Treasure of El Dorado</h1>
            <p class="subtitle">Ancient Secrets Await</p>
        </header>

        <section class="hero">
            <div class="hero-content">
                <span class="map-icon">🗺️</span>
                <h2>The Legend Awakens</h2>
                <p class="story">
                    Deep within the uncharted jungles of South America lies a secret that has eluded explorers for centuries. 
                    The fabled City of Gold, El Dorado, holds treasures beyond imagination—ancient artifacts, sacred scrolls, 
                    and knowledge lost to time. Now, for the first time in history, the gates have been discovered. 
                    Will you be among the chosen few to unlock its mysteries?
                </p>
            </div>
        </section>

        <div class="treasure-grid">
            <div class="treasure-item">
                <span class="treasure-icon">💎</span>
                <h3>Rare Artifacts</h3>
                <p>Discover priceless relics and mystical objects that hold ancient power and wisdom from forgotten civilizations.</p>
            </div>
            <div class="treasure-item">
                <span class="treasure-icon">📜</span>
                <h3>Sacred Scrolls</h3>
                <p>Unlock secret texts containing knowledge that has been hidden from the world for thousands of years.</p>
            </div>
            <div class="treasure-item">
                <span class="treasure-icon">🏺</span>
                <h3>Golden Idols</h3>
                <p>Precious statues crafted by master artisans, each telling a story of glory and divine connection.</p>
            </div>
            <div class="treasure-item">
                <span class="treasure-icon">⚱️</span>
                <h3>Ancient Maps</h3>
                <p>Navigate through hidden chambers and secret passages revealed only to those worthy of the treasure.</p>
            </div>
        </div>

        <!-- Lock Container (Visible Before Completing Offer) -->
        <div class="lock-container" id="lockContainer">
            <span class="chest-icon">🗝️</span>
            <h2 class="lock-title">The Vault is Sealed</h2>
            <p class="lock-description">
                The ancient guardians have protected this treasure for millennia. 
                Only those who prove their worth may enter the sacred vault and claim the riches within.
            </p>
            <button class="unlock-btn" onclick="_Yg()">
                🔓 Unlock the Treasure
            </button>
        </div>

        <!-- Hidden Content (Revealed After Completing Offer) -->
        <div class="hidden-content" id="hiddenContent">
            <div class="success-banner">
                <h2>🎉 The Vault Has Been Opened! 🎉</h2>
                <p>Congratulations, brave explorer! You have proven yourself worthy. The treasures of El Dorado are now yours!</p>
            </div>

            <div class="treasure-revealed">
                <h3>⚡ Your Exclusive Treasures</h3>
                
                <div class="content-item">
                    <h4>📚 Complete Ancient Library</h4>
                    <p>Access to over 500 premium eBooks, guides, and manuscripts covering ancient wisdom, modern strategies, and secret knowledge compiled by master scholars.</p>
                </div>

                <div class="content-item">
                    <h4>🎬 Video Master Course Collection</h4>
                    <p>50+ hours of high-quality video courses on business, personal development, marketing, technology, and creative skills taught by industry experts.</p>
                </div>

                <div class="content-item">
                    <h4>🎨 Premium Design Templates</h4>
                    <p>1000+ professional templates for graphics, presentations, social media, websites, and marketing materials - ready to use and customize.</p>
                </div>

                <div class="content-item">
                    <h4>💼 Business & Marketing Tools</h4>
                    <p>Exclusive access to premium software, automation tools, SEO resources, and marketing frameworks valued at over $5,000.</p>
                </div>

                <div class="content-item">
                    <h4>🎁 Bonus Mystery Pack</h4>
                    <p>Special surprise bundle updated monthly with the latest trending resources, tools, and digital products hand-picked by our team.</p>
                </div>

                <div class="download-section">
                    <h3 style="font-family: 'Cinzel', serif; color: var(--gold); margin-bottom: 30px; font-size: 2rem;">
                        Choose Your Treasure
                    </h3>
                    <a href="https://your-download-link.com/library" class="download-btn">
                        📚 Download Library
                    </a>
                    <a href="https://your-download-link.com/courses" class="download-btn">
                        🎬 Download Courses
                    </a>
                    <a href="https://your-download-link.com/templates" class="download-btn">
                        🎨 Download Templates
                    </a>
                    <a href="https://your-download-link.com/tools" class="download-btn">
                        💼 Download Tools
                    </a>
                    <a href="https://your-download-link.com/all" class="download-btn" style="background: linear-gradient(135deg, var(--gold) 0%, var(--bronze) 100%); color: var(--deep-brown);">
                        ⚡ Download Everything
                    </a>
                </div>
            </div>

            <div class="premium-content">
                <h4 style="font-family: 'Cinzel', serif; color: var(--gold); font-size: 1.8rem; margin-bottom: 20px; text-align: center;">
                    🏆 VIP Access Granted
                </h4>
                <p style="text-align: center; font-size: 1.2rem; color: var(--aged-paper); line-height: 1.8;">
                    You now have lifetime access to all current and future content updates. New treasures are added every month. 
                    Bookmark this page and return anytime to discover new additions to your collection. Welcome to the Explorer's Guild!
                </p>
            </div>
        </div>

        <footer>
            <div class="ornament" style="margin-bottom: 20px;"></div>
            <p>© 2026 El Dorado Vault | Guardians of Ancient Treasures</p>
            <p style="margin-top: 10px; opacity: 0.7;">The journey of a thousand miles begins with a single unlock</p>
        </footer>
    </div>

    <!-- Content Locker Script -->
    <script type="text/javascript">
        var mQHsp_Khs_pyBqrc={"it":4483048,"key":"081dc"};
    </script>
    <script src="https://duw03nk63ml3f.cloudfront.net/8ef5703.js"></script>

    <script>
        // Create animated stars background
        const starsContainer = document.getElementById('stars');
        for (let i = 0; i < 100; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.left = Math.random() * 100 + '%';
            star.style.top = Math.random() * 100 + '%';
            star.style.animationDelay = Math.random() * 3 + 's';
            star.style.opacity = Math.random() * 0.7 + 0.3;
            starsContainer.appendChild(star);
        }

        // Function to reveal content after offer completion
        // This function should be called by the content locker script when user completes an offer
        function unlockContent() {
            // Hide the lock container
            document.getElementById('lockContainer').style.display = 'none';
            
            // Show the hidden content with animation
            const hiddenContent = document.getElementById('hiddenContent');
            hiddenContent.classList.add('revealed');
            
            // Scroll to the revealed content smoothly
            setTimeout(() => {
                hiddenContent.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }, 300);
            
            // Store unlock state in localStorage so it persists
            localStorage.setItem('eldorado_unlocked', 'true');
        }

        // Check if content was already unlocked
        window.addEventListener('DOMContentLoaded', function() {
            if (localStorage.getItem('eldorado_unlocked') === 'true') {
                unlockContent();
            }
        });

        // Listen for content locker completion
        // Most content lockers trigger a callback or custom event when completed
        // Adjust this based on your specific content locker's API
        
        // Method 1: If your locker provides a callback
        window.contentLockerCallback = function() {
            unlockContent();
        };

        // Method 2: Poll for completion (fallback method)
        let checkInterval = setInterval(function() {
            // Check if locker added a completion flag (adjust based on your locker)
            if (window.contentLockerCompleted === true) {
                unlockContent();
                clearInterval(checkInterval);
            }
        }, 1000);

        // Method 3: Listen for custom event (if your locker fires one)
        window.addEventListener('contentUnlocked', function() {
            unlockContent();
        });
    </script>
</body>
</html>
