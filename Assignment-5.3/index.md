Here is the complete code for your Assignment 5.3 — Typography Showcase Page.

To complete this assignment, create two files in the same folder on your computer: index.html and style.css.

1. The HTML File (index.html)
Save this code as index.html. It imports two complementary Google Fonts (Playfair Display for headings and Inter for body text) and is structured into the 3 required sections: Heading Styles, Paragraph Styles, and Text Emphasis.

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Typography Showcase Page</title>
    <!-- Step 1: Import Google Fonts (Playfair Display & Inter) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
    
    <!-- Link External Stylesheet -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Typography Showcase</h1>
        <p class="subtitle">An exploration of hierarchy, font pairing, spacing, and text styling.</p>
    </header>

    <main>
        <!-- Section 1: Heading Styles -->
        <section class="typography-section">
            <h2>1. Heading Styles</h2>
            <p class="section-desc">Headings use <strong>Playfair Display</strong> with adjusted letter-spacing and font-weights.</p>
            
            <h1 class="demo-h1">Heading Level 1 (H1)</h1>
            <h2 class="demo-h2">Heading Level 2 (H2)</h2>
            <h3 class="demo-h3">Heading Level 3 (H3)</h3>
            <h4 class="demo-h4">Heading Level 4 (H4)</h4>
        </section>

        <!-- Section 2: Paragraph Styles -->
        <section class="typography-section">
            <h2>2. Paragraph Styles</h2>
            <p class="section-desc">Paragraphs use <strong>Inter</strong> with optimized line-height and max-widths for readability.</p>
            
            <p class="demo-lead">
                Lead Paragraph: Typography is the art and technique of arranging type to make written language legible, readable, and appealing when displayed.
            </p>
            <p class="demo-body">
                Standard Body Paragraph: Good typography establishes a clear visual hierarchy, giving readers effortless entry points and intuitive transitions between sections. By adjusting line-height, letter-spacing, and font weights, designers can transform standard text into an engaging visual experience.
            </p>
            <p class="demo-small">
                Small / Muted Paragraph: Used for captions, metadata, disclaimers, or secondary reference notes.
            </p>
        </section>

        <!-- Section 3: Text Emphasis & Formatting -->
        <section class="typography-section">
            <h2>3. Text Emphasis &amp; Formatting</h2>
            <p class="section-desc">Demonstrating <code>font-style</code>, <code>text-decoration</code>, and <code>text-align</code> properties.</p>
            
            <div class="emphasis-grid">
                <div class="emphasis-card">
                    <h3>Italic &amp; Oblique</h3>
                    <p class="demo-italic">This text uses font-style: italic for subtle emphasis.</p>
                </div>
                <div class="emphasis-card">
                    <h3>Text Decorations</h3>
                    <p class="demo-underline">This text has an underline decoration.</p>
                    <p class="demo-line-through">This text has a line-through decoration.</p>
                    <p class="demo-overline">This text has an overline decoration.</p>
                </div>
                <div class="emphasis-card">
                    <h3>Text Alignment</h3>
                    <p class="demo-center">Centered alignment for special headers or callouts.</p>
                    <p class="demo-right">Right-aligned text block layout example.</p>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 Typography Showcase. Created for Assignment 5.3.</p>
    </footer>

</body>
</html>
2. The CSS File (style.css)
Save this code as style.css in the exact same folder as your index.html file.

CSS
/* Global Reset */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

/* Step 2 & 3: Set body fonts (Inter for body), colors, and background */
body {
    font-family: 'Inter', sans-serif;
    background-color: #f8f9fa;
    color: #212529;
    line-height: 1.7;
    padding: 40px 20px;
}

/* Header Styling */
header {
    text-align: center;
    max-width: 800px;
    margin: 0 auto 50px auto;
}

/* Step 2 & 4: Set heading font (Playfair Display) */
header h1 {
    font-family: 'Playfair Display', serif;
    font-size: 3rem;
    font-weight: 700;
    color: #1a2a3a;
    letter-spacing: 1px;
    margin-bottom: 10px;
}

.subtitle {
    font-size: 1.15rem;
    color: #6c757d;
    font-weight: 300;
    letter-spacing: 0.5px;
}

/* Main Container & Sections */
main {
    max-width: 900px;
    margin: 0 auto;
}

.typography-section {
    background-color: #ffffff;
    padding: 40px;
    margin-bottom: 30px;
    border-radius: 12px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
}

.typography-section > h2 {
    font-family: 'Playfair Display', serif;
    font-size: 1.8rem;
    color: #0066cc;
    border-bottom: 2px solid #e9ecef;
    padding-bottom: 10px;
    margin-bottom: 15px;
}

.section-desc {
    font-size: 0.95rem;
    color: #6c757d;
    margin-bottom: 25px;
}

/* ==========================================================
   Step 3, 4 & 5: Heading Styles (Playfair Display)
   ========================================================== */
.demo-h1 {
    font-family: 'Playfair Display', serif;
    font-size: 2.5rem;
    font-weight: 700;
    line-height: 1.2;
    letter-spacing: -0.5px;
    margin-bottom: 15px;
    color: #111;
}

.demo-h2 {
    font-family: 'Playfair Display', serif;
    font-size: 2rem;
    font-weight: 700;
    line-height: 1.3;
    letter-spacing: 0px;
    margin-bottom: 15px;
    color: #222;
}

.demo-h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem;
    font-weight: 400;
    font-style: italic;
    line-height: 1.4;
    letter-spacing: 0.5px;
    margin-bottom: 15px;
    color: #333;
}

.demo-h4 {
    font-family: 'Inter', sans-serif;
    font-size: 1.15rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin-bottom: 10px;
    color: #495057;
}

/* ==========================================================
   Step 3 & 5: Paragraph Styles (Inter with Line-Height & Letter-Spacing)
   ========================================================== */
.demo-lead {
    font-size: 1.2rem;
    font-weight: 300;
    line-height: 1.8;
    letter-spacing: 0.2px;
    color: #343a40;
    margin-bottom: 20px;
}

.demo-body {
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.7;
    letter-spacing: 0.3px;
    color: #495057;
    margin-bottom: 20px;
}

.demo-small {
    font-size: 0.85rem;
    font-weight: 300;
    line-height: 1.5;
    letter-spacing: 0.5px;
    color: #adb5bd;
}

/* ==========================================================
   Step 4: Text Emphasis & Alignment Demonstrations
   ========================================================== */
.emphasis-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.emphasis-card {
    background-color: #f8f9fa;
    border: 1px solid #e9ecef;
    padding: 20px;
    border-radius: 8px;
}

.emphasis-card h3 {
    font-size: 1.1rem;
    margin-bottom: 12px;
    color: #1a2a3a;
}

/* Specific text-decoration & font-style rules */
.demo-italic {
    font-style: italic;
    color: #495057;
}

.demo-underline {
    text-decoration: underline;
    text-decoration-color: #0066cc;
    text-underline-offset: 4px;
}

.demo-line-through {
    text-decoration: line-through;
    color: #6c757d;
}

.demo-overline {
    text-decoration: overline;
}

.demo-center {
    text-align: center;
    font-weight: 600;
    color: #0066cc;
}

.demo-right {
    text-align: right;
    font-style: italic;
}

/* Footer Styling */
footer {
    text-align: center;
    margin-top: 50px;
    color: #6c757d;
    font-size: 0.9rem;
}
Assignment Requirements Summary
Google Fonts (Step 1): Imported two complementary families (Playfair Display for headings and Inter for body text).

Distinct Fonts (Step 2): Applied serif headings (Playfair Display) and clean sans-serif body text (Inter).

Font Sizes & Weights (Step 3): Varied sizes from 2.5rem (H1) to 0.85rem (small), with weights ranging from 300 (light) to 700 (bold).

Text Properties (Step 4): Applied text-align (center, right), text-decoration (underline, overline, line-through), and font-style (italic).

Spacing (Step 5): Adjusted letter-spacing and line-height for optimal readability and visual rhythm.

Sections (Step 6): Divided the layout into 3 distinct sections: Heading Styles, Paragraph Styles, and Text Emphasis.