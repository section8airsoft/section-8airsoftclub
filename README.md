section-8airsoftclub/
├── index.html
├── about.html
├── gallery.html
├── events.html
├── join.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── main.js
├── images/
│   └── logo.png
│   └── banner.jpg
├── CNAME
└── README.md
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Section-8 Airsoft Club Strumica</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="events.html">Events</a></li>
        <li><a href="join.html">Join Us</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <img src="images/banner.jpg" alt="Section-8 Banner">
    <h1>COMING SOON</h1>
    <p>Join the Brotherhood — Section-8 Airsoft Club Strumica</p>
    <a href="join.html" class="btn">Become a Member</a>
  </section>

  <footer>
    <p>© 2026 Section-8 Airsoft Club Strumica</p>
  </footer>
</body>
</html>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #111;
  color: #eee;
}

header {
  background: #000;
  padding: 10px;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 20px;
}

nav a {
  color: #eee;
  text-decoration: none;
  font-weight: bold;
}

.hero {
  text-align: center;
  padding: 50px;
  background: url('../images/banner.jpg') no-repeat center;
  background-size: cover;
}

.hero h1 {
  font-size: 48px;
  color: #fff;
  text-transform: uppercase;
}

.hero p {
  font-size: 20px;
  color: #f00;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 20px;
  background: #f00;
  color: #fff;
  text-decoration: none;
  font-weight: bold;
}
section-8airsoftclub.mk
name: Deploy Website

on:
  push:
    branches:
      - main

jobs:
  build-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

  
