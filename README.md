Starting from [this tutorial](https://youtu.be/diVWXMFqJu4?si=N2AKvZ7spW2_zAVC), I will work on converting content from my [*Google Sites*](https://sites.google.com/site/cwarden45/about-me) page.

Among the Jekyll supported themes that are [currently listed here](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll), I liked the *Cayman* theme.  However, the *UCR* Orbach Science Library video also references [https://github.com/topics/jekyll-theme](https://github.com/topics/jekyll-theme), which includes other themes such as [Academic Pages](https://academicpages.github.io/) (which acknowledges that it was forked from [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)).

While this could provide an opportunity for me to learn more about Jekyll, I believe that I can also use this a chance to review/remember how to make a basic website with HTML and CSS for a sidebar/sidenav (such as described [here](https://stackoverflow.com/questions/29960458/making-a-simple-layout-with-a-sidebar-in-html-css), [here](https://www.youtube.com/watch?v=HGTJBPNC-Gw), [here]([https://www.youtube.com/playlist?list=PL0eyrZgxdwhwNC5ppZo_dYGVjerQY3xYU], [here](https://www.youtube.com/watch?v=HgwCeNVPlo0&list=PL0eyrZgxdwhwNC5ppZo_dYGVjerQY3xYU&index=39), [here](https://www.codecademy.com/catalog/language/html-css), [here](https://www.w3schools.com/css/css_templates.asp), etc.).  So, that is my current goal.

**GENERAL NOTE**: One reason to be cautious about the use of AI is that it may cause the user to over-estimate their understanding of the material, in addition to creating problems with assessing learning.  This is similar (but not idential) to my rational to wanting to use minimal code to accomplish my goal, with understanding of all of the components of the code.

At the same time, I beleive it is also unfair to prohibit the use of AI (or *Google*) in all circumstances.  So, as part of the progress for me to regain this skill (assuming the syntex is the same or similar to ~20 years ago), I will try to be transparent in the learning/re-learning and troubleshooting process.

For example, as a starting point, I will provide example template code that could have been created with a quick search / request.

### *Google* / *Gemini* Template Example

This is one result for the search "*GitHub Pages compatible HTML and CSS for sidebar*":

Provided HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sidebar Layout</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="wrapper">
        <aside class="sidebar">
            <h2>My Site</h2>
            <nav>
                <a href="#" class="active">Home</a>
                <a href="#">About</a>
                <a href="#">Services</a>
                <a href="#">Contact</a>
            </nav>
        </aside>
        <main class="content">
            <h1>Welcome</h1>
            <p>This is the main content area.</p>
        </main>
    </div>
</body>
</html>

```

Provided CSS Code:
```
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: sans-serif;
    background-color: #f4f4f4;
}

.wrapper {
    display: flex;
    min-height: 100vh;
}

.sidebar {
    width: 250px;
    background-color: #333;
    color: #fff;
    padding: 20px;
    position: fixed;
    height: 100%;
}

.sidebar h2 {
    margin-bottom: 20px;
    font-size: 1.5rem;
}

.sidebar nav a {
    display: block;
    color: #ccc;
    text-decoration: none;
    padding: 10px 0;
    transition: color 0.2s;
}

.sidebar nav a:hover,
.sidebar nav a.active {
    color: #fff;
}

.content {
    margin-left: 250px;
    padding: 40px;
    flex: 1;
}
```

In both cases, there is a warning "**Use code with caution.**".

### *ChatGPT* Template Example

This is one result for the prompt "*Please write HTML and CSS code compatible with GitHub Pages.  I would like to have 3 HTML files of content (About Me, CV, and Links) as well as CSS stylesheet to create a sidebar to navigate between those 3 pages.*":

Template for "About Me" HTML Page:
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>About Me</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

<div class="sidebar">

    <h1>Your Name</h1>

    <ul>
        <li><a class="active" href="index.html">About Me</a></li>
        <li><a href="cv.html">CV</a></li>
        <li><a href="links.html">Links</a></li>
    </ul>

</div>

<div class="content">

<h2>About Me</h2>

<p>
Welcome! This is the About Me page.
</p>

<p>
Add a short biography here. You might include your research interests,
current position, education, and professional goals.
</p>

<p>
You can also include a professional photo or research interests later.
</p>

</div>

</body>
</html>
```

Template for "CV" HTML Page:
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Curriculum Vitae</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

<div class="sidebar">

    <h1>Your Name</h1>

    <ul>
        <li><a href="index.html">About Me</a></li>
        <li><a class="active" href="cv.html">CV</a></li>
        <li><a href="links.html">Links</a></li>
    </ul>

</div>

<div class="content">

<h2>Curriculum Vitae</h2>

<h3>Education</h3>

<ul>
<li>Ph.D. in ...</li>
<li>M.S. in ...</li>
<li>B.S. in ...</li>
</ul>

<h3>Appointments</h3>

<ul>
<li>Assistant Professor...</li>
<li>Graduate Research Assistant...</li>
</ul>

<h3>Publications</h3>

<ul>
<li>Publication 1</li>
<li>Publication 2</li>
<li>Publication 3</li>
</ul>

</div>

</body>
</html>
```

Template for "Links" HTML Page:
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Links</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

<div class="sidebar">

    <h1>Your Name</h1>

    <ul>
        <li><a href="index.html">About Me</a></li>
        <li><a href="cv.html">CV</a></li>
        <li><a class="active" href="links.html">Links</a></li>
    </ul>

</div>

<div class="content">

<h2>Useful Links</h2>

<ul>
<li><a href="https://scholar.google.com" target="_blank">Google Scholar</a></li>

<li><a href="https://github.com" target="_blank">GitHub</a></li>

<li><a href="https://orcid.org" target="_blank">ORCID</a></li>

<li><a href="https://www.linkedin.com" target="_blank">LinkedIn</a></li>

</ul>

</div>

</body>
</html>
```

Template for CSS Code:
```
/* ----------------------------
   General Styling
----------------------------- */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    display: flex;
    background: #f7f7f7;
    color: #333;
}

/* ----------------------------
   Sidebar
----------------------------- */

.sidebar {
    width: 240px;
    height: 100vh;
    position: fixed;
    background: #2c3e50;
    color: white;
    padding-top: 30px;
}

.sidebar h1 {
    text-align: center;
    margin-bottom: 35px;
    font-size: 1.6em;
}

.sidebar ul {
    list-style: none;
}

.sidebar li {
    margin: 12px 0;
}

.sidebar a {
    display: block;
    color: white;
    text-decoration: none;
    padding: 12px 25px;
    transition: 0.3s;
}

.sidebar a:hover {
    background: #34495e;
    padding-left: 35px;
}

.sidebar a.active {
    background: #1abc9c;
    font-weight: bold;
}

/* ----------------------------
   Main Content
----------------------------- */

.content {
    margin-left: 240px;
    padding: 50px;
    width: calc(100% - 240px);
}

.content h2 {
    margin-bottom: 20px;
    color: #2c3e50;
}

.content p {
    margin-bottom: 16px;
    line-height: 1.7;
}

.content ul {
    margin-left: 20px;
    margin-bottom: 20px;
}

.content li {
    margin-bottom: 8px;
}

/* ----------------------------
   Responsive Layout
----------------------------- */

@media (max-width: 700px) {

    body {
        display: block;
    }

    .sidebar {
        position: relative;
        width: 100%;
        height: auto;
    }

    .content {
        margin-left: 0;
        width: 100%;
        padding: 30px;
    }

}
```

### *Claude* Template Example

This is one result for the prompt "*Please write HTML and CSS code compatible with GitHub Pages.  I would like to have 3 HTML files of content (About Me, CV, and Links) as well as CSS stylesheet to create a sidebar to navigate between those 3 pages.*":

Template for "About Me" HTML Page:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Name — About Me</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="layout">
    <nav class="sidebar">
      <div class="sidebar-header">
        <p class="sidebar-name">Your Name</p>
        <p class="sidebar-tagline">Personal Site</p>
      </div>
      <hr class="sidebar-rule">
      <ul class="sidebar-nav">
        <li><a href="index.html" class="active">About Me</a></li>
        <li><a href="cv.html">CV</a></li>
        <li><a href="links.html">Links</a></li>
      </ul>
      <p class="sidebar-footer">&copy; 2026 Your Name</p>
    </nav>

    <main class="content">
      <p class="eyebrow">About</p>
      <h1>Hi, I'm Your Name.</h1>
      <p>
        Replace this paragraph with a short introduction: who you are, what you do,
        and what you care about. Two or three sentences is usually enough — this
        page is a first impression, not a full biography.
      </p>

      <h2>What I do</h2>
      <p>
        Describe your current role, focus area, or field. Mention the kind of
        problems you like working on, or the projects you're most proud of.
      </p>

      <h2>Outside of work</h2>
      <p>
        A line or two about interests, hobbies, or anything that gives visitors
        a sense of who you are beyond your job title.
      </p>

      <h2>Get in touch</h2>
      <p>
        Reach me at <a href="mailto:you@example.com">you@example.com</a>, or find
        more ways to connect on the <a href="links.html">Links</a> page.
      </p>
    </main>
  </div>
</body>
</html>

```

Template for "CV" HTML Page:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Name — CV</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="layout">
    <nav class="sidebar">
      <div class="sidebar-header">
        <p class="sidebar-name">Your Name</p>
        <p class="sidebar-tagline">Personal Site</p>
      </div>
      <hr class="sidebar-rule">
      <ul class="sidebar-nav">
        <li><a href="index.html">About Me</a></li>
        <li><a href="cv.html" class="active">CV</a></li>
        <li><a href="links.html">Links</a></li>
      </ul>
      <p class="sidebar-footer">&copy; 2026 Your Name</p>
    </nav>

    <main class="content">
      <p class="eyebrow">Curriculum Vitae</p>
      <h1>CV</h1>
      <p>A short summary of your professional background. You can also link to a downloadable PDF version here if you have one.</p>

      <h2>Experience</h2>

      <div class="entry">
        <div class="entry-header">
          <span class="entry-title">Job Title, Company Name</span>
          <span class="entry-date">2023 — Present</span>
        </div>
        <p class="entry-sub">City, Country</p>
        <ul>
          <li>Key responsibility or achievement in this role.</li>
          <li>Another notable contribution or result.</li>
        </ul>
      </div>

      <div class="entry">
        <div class="entry-header">
          <span class="entry-title">Previous Job Title, Previous Company</span>
          <span class="entry-date">2020 — 2023</span>
        </div>
        <p class="entry-sub">City, Country</p>
        <ul>
          <li>Key responsibility or achievement in this role.</li>
          <li>Another notable contribution or result.</li>
        </ul>
      </div>

      <h2>Education</h2>

      <div class="entry">
        <div class="entry-header">
          <span class="entry-title">Degree, Institution Name</span>
          <span class="entry-date">2016 — 2020</span>
        </div>
        <p class="entry-sub">City, Country</p>
      </div>

      <h2>Skills</h2>
      <p>List your core skills here — languages, tools, frameworks, or areas of expertise, separated by commas or grouped by category.</p>

    </main>
  </div>
</body>
</html>
```

Template for "Links" HTML Page:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Name — Links</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="layout">
    <nav class="sidebar">
      <div class="sidebar-header">
        <p class="sidebar-name">Your Name</p>
        <p class="sidebar-tagline">Personal Site</p>
      </div>
      <hr class="sidebar-rule">
      <ul class="sidebar-nav">
        <li><a href="index.html">About Me</a></li>
        <li><a href="cv.html">CV</a></li>
        <li><a href="links.html" class="active">Links</a></li>
      </ul>
      <p class="sidebar-footer">&copy; 2026 Your Name</p>
    </nav>

    <main class="content">
      <p class="eyebrow">Elsewhere</p>
      <h1>Links</h1>
      <p>Ways to find me or my work around the web.</p>

      <div class="link-grid">
        <a class="link-card" href="https://github.com/yourusername" target="_blank" rel="noopener">
          <div>
            <div class="link-label">GitHub</div>
            <div class="link-desc">Code and projects</div>
          </div>
          <span class="link-arrow">&rarr;</span>
        </a>

        <a class="link-card" href="https://linkedin.com/in/yourusername" target="_blank" rel="noopener">
          <div>
            <div class="link-label">LinkedIn</div>
            <div class="link-desc">Professional profile</div>
          </div>
          <span class="link-arrow">&rarr;</span>
        </a>

        <a class="link-card" href="mailto:you@example.com">
          <div>
            <div class="link-label">Email</div>
            <div class="link-desc">you@example.com</div>
          </div>
          <span class="link-arrow">&rarr;</span>
        </a>

        <a class="link-card" href="https://twitter.com/yourusername" target="_blank" rel="noopener">
          <div>
            <div class="link-label">Twitter / X</div>
            <div class="link-desc">Occasional thoughts</div>
          </div>
          <span class="link-arrow">&rarr;</span>
        </a>
      </div>
    </main>
  </div>
</body>
</html>
```

Template for CSS Code:
```
@import url('https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@500&display=swap');

:root {
  --paper: #faf7f1;
  --ink: #1b1f27;
  --ink-soft: #2a2f3a;
  --line: #d8d2c4;
  --accent: #b5793a;
  --accent-soft: #e8d9c0;
  --muted: #6b6558;
  --sidebar-w: 260px;
}

* { box-sizing: border-box; }

html, body {
  margin: 0;
  padding: 0;
  background: var(--paper);
  color: var(--ink);
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  line-height: 1.6;
}

.layout {
  display: flex;
  min-height: 100vh;
}

/* ---------- Sidebar ---------- */

.sidebar {
  width: var(--sidebar-w);
  flex-shrink: 0;
  background: var(--ink);
  color: var(--paper);
  padding: 2.5rem 1.75rem;
  display: flex;
  flex-direction: column;
  position: sticky;
  top: 0;
  height: 100vh;
}

.sidebar-header {
  margin-bottom: 2.5rem;
}

.sidebar-name {
  font-family: 'Fraunces', serif;
  font-size: 1.6rem;
  font-weight: 600;
  margin: 0 0 0.35rem 0;
  letter-spacing: 0.01em;
}

.sidebar-tagline {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.72rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--accent-soft);
  margin: 0;
}

.sidebar-rule {
  border: none;
  border-top: 1px solid rgba(250, 247, 241, 0.15);
  margin: 1.75rem 0;
}

.sidebar-nav {
  list-style: none;
  margin: 0;
  padding: 0;
  flex-grow: 1;
}

.sidebar-nav li {
  margin-bottom: 0.35rem;
}

.sidebar-nav a {
  display: block;
  color: rgba(250, 247, 241, 0.72);
  text-decoration: none;
  font-size: 0.95rem;
  padding: 0.55rem 0.75rem;
  border-left: 2px solid transparent;
  border-radius: 2px;
  transition: color 0.15s ease, border-color 0.15s ease, background 0.15s ease;
}

.sidebar-nav a:hover {
  color: var(--paper);
  background: rgba(250, 247, 241, 0.06);
  border-left-color: var(--accent-soft);
}

.sidebar-nav a.active {
  color: var(--paper);
  border-left-color: var(--accent);
  background: rgba(181, 121, 58, 0.15);
  font-weight: 500;
}

.sidebar-footer {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.7rem;
  color: rgba(250, 247, 241, 0.4);
  padding-top: 1.5rem;
}

/* ---------- Main content ---------- */

.content {
  flex-grow: 1;
  padding: 4rem 5vw;
  max-width: 780px;
}

.content h1 {
  font-family: 'Fraunces', serif;
  font-size: 2.4rem;
  font-weight: 600;
  margin: 0 0 0.5rem 0;
  color: var(--ink);
}

.content .eyebrow {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--accent);
  margin: 0 0 1.5rem 0;
}

.content h2 {
  font-family: 'Fraunces', serif;
  font-size: 1.35rem;
  font-weight: 600;
  margin: 2.25rem 0 0.75rem 0;
  color: var(--ink);
  border-bottom: 1px solid var(--line);
  padding-bottom: 0.4rem;
}

.content p, .content li {
  color: var(--ink-soft);
  font-size: 1rem;
}

.content a {
  color: var(--accent);
}

.content ul {
  padding-left: 1.2rem;
}

/* CV entries */

.entry {
  margin-bottom: 1.5rem;
}

.entry-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  flex-wrap: wrap;
  gap: 0.25rem 1rem;
}

.entry-title {
  font-weight: 600;
  color: var(--ink);
}

.entry-date {
  font-family: 'IBM Plex Mono', monospace;
  font-size: 0.78rem;
  color: var(--muted);
  white-space: nowrap;
}

.entry-sub {
  font-size: 0.9rem;
  color: var(--muted);
  margin: 0.1rem 0 0.4rem 0;
}

/* Links page cards */

.link-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0.9rem;
  margin-top: 1.5rem;
}

.link-card {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 1.2rem;
  background: #fff;
  border: 1px solid var(--line);
  border-radius: 6px;
  text-decoration: none;
  transition: border-color 0.15s ease, transform 0.15s ease;
}

.link-card:hover {
  border-color: var(--accent);
  transform: translateX(3px);
}

.link-label {
  font-weight: 500;
  color: var(--ink);
}

.link-desc {
  font-size: 0.85rem;
  color: var(--muted);
  margin-top: 0.15rem;
}

.link-arrow {
  font-family: 'IBM Plex Mono', monospace;
  color: var(--accent);
}

/* ---------- Mobile ---------- */

@media (max-width: 720px) {
  .layout {
    flex-direction: column;
  }

  .sidebar {
    width: 100%;
    height: auto;
    position: relative;
    padding: 1.75rem 1.5rem;
  }

  .sidebar-nav {
    display: flex;
    gap: 0.5rem;
    flex-wrap: wrap;
  }

  .sidebar-nav li {
    margin-bottom: 0;
  }

  .sidebar-rule {
    margin: 1.25rem 0;
  }

  .sidebar-footer {
    display: none;
  }

  .content {
    padding: 2.5rem 6vw;
    max-width: 100%;
  }
}
```
