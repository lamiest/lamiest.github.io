<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Lameist03 Webpage</title>
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
    <p>Senior Computer Engineering Jasem Alsuwaidi is ready to explore the vast and complex background of computers using the tools and knowledge gained within Khalifa University. Currently partaking in an intership opportunity in Security Industry and Regulation Agency. You will find all of my projects in the projects page and their respective links under!</p>
  </div>

  <div id="about" class="content">
    <h2>About Me</h2>
    <p>I am passionate about learning new techniques and tools to create and develop programs, web servers and pages, networks and much more. I enjoy playing competitive games and hope to be one of the best in both Engineering and gaming!</p>
  </div>

  <div id="projects" class="content">
    <h2>Projects</h2>
    <p>Here are some projects I've worked on over the years.</p>
  </div>

  <script>
    function showTab(tabId) {
      const contents = document.querySelectorAll('.content');
      contents.forEach(content => content.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }
  </script>

</body>
