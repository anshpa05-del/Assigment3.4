HTML
<div class="header">
  <div class="logo">My Website</div>
  <div class="menu">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </div>
</div>

<div class="main-content">
  <div class="post">
    <div class="title">Understanding Semantic HTML</div>
    <div class="text">Semantic HTML makes web pages more accessible and easier to read.</div>
    <img src="html-code.png">
  </div>
  <div class="sidebar">
    <h3>Related Links</h3>
    <a href="#">Accessibility Tips</a>
  </div>
</div>

<div class="footer">
  <p>&copy; 2026 My Website</p>
</div>
After (Semantic HTML Solution)
HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assignment 3.4 — Semantic HTML & Accessibility</title>
</head>
<body>

    <!-- Step 1 & 2: Header and Nav -->
    <header>
        <h1>My Website Logo / Brand</h1>
        <nav aria-label="Main Navigation">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Step 1 & 3: Main content wrapper -->
    <main>
        <!-- Step 1: Article for standalone content -->
        <article>
            <header>
                <h2>Understanding Semantic HTML</h2>
                <p>Published by <a href="#author">Jane Doe</a></p>
            </header>
            
            <section>
                <p>Semantic HTML elements clearly describe their meaning to both the browser and the developer. They improve screen reader accessibility and SEO.</p>
                <!-- Step 5: Meaningful alt text -->
                <img src="html-code.png" alt="A screenshot showing an HTML code editor with color-coded semantic tags like article and section.">
            </section>
        </article>

        <!-- Step 1: Aside for secondary/related content -->
        <aside aria-labelledby="sidebar-title">
            <h3 id="sidebar-title">Related Resources</h3>
            <ul>
                <li><a href="#accessibility">A Guide to Web Accessibility Standards</a></li>
                <li><a href="#seo">Top 5 SEO Best Practices for 2026</a></li>
            </ul>
        </aside>
    </main>

    <!-- Step 1: Footer -->
    <footer>
        <p>&copy; 2026 My Website. All rights reserved.</p>
        <p><a href="#privacy">Privacy Policy</a></p>
    </footer>

</body>
</html>
Key Accessibility Checklist Met:
Semantic Structure (Steps 1–3): Used <header>, <nav>, <main>, <article>, <section>, <aside>, and <footer> instead of generic <div> wrappers.

Heading Hierarchy (Step 4): Follows a logical order starting with an <h1> for the branding/page title, followed by <h2> for article titles, and <h3> for sidebar headings without skipping levels.

Meaningful Alt Text (Step 5): The image alt text describes what the image shows and its context, rather than just saying "image".

Understandable Links & Sections (Step 6): Used descriptive link text and added ARIA landmarks (aria-label, aria-labelledby) to distinguish navigation and sidebar regions.

Submission Note:
To complete your submission (GitHub repo), make sure to include:

The updated HTML code file.

A "Before" screenshot showing the old div-structured webpage.

An "After" screenshot showing the newly styled semantic webpage.