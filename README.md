# Recipe.Plan

Created before sophmore year

JS

const express = require('express');
const app = express();


app.use(express.static('public'));


app.get('/', (req, res) => {
  res.sendFile(__dirname + '/public/lay.html');
});


const port = 3000;
app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});

CSS

body, h1, h2, p, ul, li, form {
    margin: 0;
    padding: 0;
  }
  
  
  body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
  }
  
  header {
    background-color: #333;
    color: #fff;
    padding: 20px;
  }
  
  nav ul {
    list-style-type: none;
  }
  
  nav ul li {
    display: inline;
    margin-right: 10px;
  }
  
  nav ul li a {
    color: #fff;
    text-decoration: none;
  }
  
  main {
    padding: 20px;
  }
  
  section {
    margin-bottom: 20px;
  }
  
  h1, h2 {
    margin-bottom: 10px;
  }
  
  form input, form textarea {
    display: block;
    margin-bottom: 10px;
    width: 100%;
    padding: 5px;
  }
  
  form button {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
  }

  HTML

  <!DOCTYPE html>
<html>
<head>
  <title>ALL-STARZ</title>
  <link rel="stylesheet" type="text/css" href="lay.css" href="lay.js">
</head>
<body>
  <header>
    <h1>Recipe Plans</h1>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
  
  <main>
    <section>
      <h2>About</h2>
      <p>The Consumption Planners </p>
    </section>
    
    <section>
      <h2>Services</h2>
      <ul>
        <li>Recipes</li>
        <li>Preference</li>
        <li>Menu</li>
      </ul>
    </section>
    
    <section>
      <h2>Contact</h2>
      <form>
        <input type="text" placeholder="Your Name">
        <input type="email" placeholder="Your Email">
        <textarea placeholder="Message"></textarea>
        <button type="submit">Send</button>
      </form>
    </section>
  </main>
  
  <footer>
    <p>&copy; 2023 Specter All rights reserved.</p>
  </footer>
</body>
</html>
  
