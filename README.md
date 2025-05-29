<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Simple Tab Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    .navbar {
      display: flex;
      background-color: #333;
    }
    .navbar button {
      background-color: #333;
      color: white;
      border: none;
      padding: 14px 20px;
      cursor: pointer;
      font-size: 16px;
      flex: 1;
    }
    .navbar button:hover {
      background-color: #575757;
    }
    .content {
      display: none;
      padding: 20px;
    }
    .active {
      display: block;
    }
  </style>
</head>
<body>

  <div class="navbar">
    <button onclick="showTab('home')">Home</button>
    <button onclick="showTab('about')">About Me</button>
    <button onclick="showTab('projects')">Projects</button>
  </div>

  <div id="home" class="content active">
    <h2>Home</h2>
    <p>Welcome to my personal website!</p>
  </div>

  <div id="about" class="content">
    <h2>About Me</h2>
    <p>Hello! I'm a developer with a passion for building things on the web.</p>
  </div>

  <div id="projects" class="content">
    <h2>Projects</h2>
    <p>Here are some projects I've worked on recently.</p>
  </div>

  <script>
    function showTab(tabId) {
      const contents = document.querySelectorAll('.content');
      contents.forEach(content => content.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }
  </script>

</body>
</html>
