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
    <h3>ESP-WROOM-32 Touch Detector and Counter</h3>
    <p>This project revolves around the use of the ESP-WROOM-32 touch modules within the pins of the microcontroller. The main purpose is to be able to use the touch sensors to detect specifically where (which pin) the detection occurred in and to increment the detection count from the EEPROM. This was done in the Arduino IDE in the language of C++. Ensure that the board can communicate with the Host on COM(1-5) in Serial Communication. Respective drivers for the communication may be needed.</p>
    <h3>ESP-WROOM-32 Web Server and Basic Calculator</h3>
    <p>This project was made on the ESP-WROOM-32 as a basic functioning web server and a calculator. The main purpose is to demonstrate the capabilities of the WiFi module of the ESP32 to function as a local web server and to show that data can be sent/received on WiFi.</p>
![IMG_8383](https://github.com/user-attachments/assets/9e9ca487-0941-4810-a7cb-6a665259ea7a)
![IMG_8380](https://github.com/user-attachments/assets/e3dd1495-492b-45d6-a313-ad6510701241)
![IMG_8381](https://github.com/user-attachments/assets/6ef9f766-2cb4-44d0-adfa-83d4a6d9d22a)

  </div>

  <script>
    function showTab(tabId) {
      const contents = document.querySelectorAll('.content');
      contents.forEach(content => content.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }
  </script>

</body>
