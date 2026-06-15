# Thiranex_WD_01
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- Optimized, SEO-Friendly Meta Tags -->
    <meta name="description" content="Personal portfolio of [Your Name], an expert in web development, showcasing modern semantic HTML5 and accessible web design.">
    <meta name="keywords" content="Portfolio, Web Developer, HTML5, Accessibility, WCAG, Frontend">
    <meta name="author" content="[Your Name]">
    
    <!-- Open Graph for Social Sharing (SEO Boost) -->
    <meta property="og:title" content="[Your Name] | Personal Portfolio">
    <meta property="og:description" content="Explore my projects, skills, and professional experience.">
    <meta property="og:type" content="website">
    
    <title>[Your Name] | Personal Portfolio</title>

    <style>
        /* CSS to ensure the 'skip to content' link works visually for keyboard users */
        .skip-link {
            position: absolute;
            top: -40px;
            left: 0;
            background: #0056b3;
            color: white;
            padding: 8px;
            z-index: 100;
            text-decoration: none;
        }
        .skip-link:focus {
            top: 0;
        }
        /* Basic visual spacing for the form */
        form { display: flex; flex-direction: column; max-width: 400px; gap: 1rem; margin-top: 1rem; }
        label { font-weight: bold; }
    </style>
</head>
<body>

    <!-- Accessibility: Skip navigation link for keyboard & screen reader users -->
    <a href="#main-content" class="skip-link">Skip to main content</a>

    <!-- Semantic Header -->
    <header role="banner">
        <h1>[Your Name]</h1>
        <p>Web Developer & Accessibility Advocate</p>
        
        <!-- Semantic Navigation with ARIA label -->
        <nav aria-label="Main Navigation" role="navigation">
            <ul>
                <!-- aria-current indicates the active page -->
                <li><a href="index.html" aria-current="page">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="projects.html">Projects</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Semantic Main Content Area -->
    <main id="main-content" role="main">

        <!-- Section with ARIA labeling -->
        <section aria-labelledby="intro-heading">
            <h2 id="intro-heading">Welcome to my Portfolio</h2>
            <p>This is a strictly semantic, fully accessible HTML5 skeleton designed to meet modern WCAG standards.</p>
        </section>

        <!-- Semantic Article for a discrete piece of content -->
        <article aria-labelledby="project-1-heading">
            <h3 id="project-1-heading">Featured Project: Accessible Web App</h3>
            <p>Details about the project go here, utilizing appropriate semantic elements to describe the scope and technologies used.</p>
            <!-- Image with descriptive alt text -->
            <img src="placeholder-project.jpg" alt="A screenshot of the accessible web app dashboard showing user analytics and high-contrast charts">
        </article>

        <!-- Accessible, Tab-Navigable Contact Form -->
        <section aria-labelledby="contact-heading">
            <h2 id="contact-heading">Get in Touch</h2>
            
            <!-- Form with an explicit ARIA label -->
            <form action="/submit" method="POST" aria-label="Contact form">
                <div>
                    <!-- Explicit label-to-input mapping via 'for' and 'id' -->
                    <label for="name">Full Name (Required)</label>
                    <input type="text" id="name" name="name" required aria-required="true" autocomplete="name">
                </div>

                <div>
                    <label for="email">Email Address (Required)</label>
                    <input type="email" id="email" name="email" required aria-required="true" autocomplete="email">
                </div>

                <div>
                    <label for="message">Your Message (Required)</label>
                    <textarea id="message" name="message" rows="5" required aria-required="true"></textarea>
                </div>

                <button type="submit">Send Message</button>
            </form>
        </section>

    </main>

    <!-- Semantic Footer -->
    <footer role="contentinfo">
        <p>&copy; 2026 [Your Name]. Built with Semantic HTML5.</p>
        <nav aria-label="Social Media Links">
            <ul>
                <li><a href="#" aria-label="Visit my LinkedIn Profile">LinkedIn</a></li>
                <li><a href="#" aria-label="Visit my GitHub Profile">GitHub</a></li>
            </ul>
        </nav>
    </footer>

</body>
</html>
