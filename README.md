# it-troubleshooting-guides
it-troubleshooting-guides/
│
├── index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>IT Troubleshooting Guides</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>

    <header>
        <h1>IT Troubleshooting Guides</h1>
        <p>Step-by-step solutions for common IT support issues.</p>
    </header>

    <nav>
    <button id="darkModeToggle">Toggle Dark Mode</button>
        <ul>
            <li><a href="#network">Network Issues</a></li>
            <li><a href="#printer">Printer Problems</a></li>
            <li><a href="#slowpc">Slow PC</a></li>
            <li><a href="#email">Email Issues</a></li>
        </ul>
    </nav>

    <main>

        <section id="network" class="guide-card">
            <h2>Network Connectivity Issues</h2>
            <p>Common fixes for internet and network problems.</p>

            <ol>
                <li>Check Ethernet/Wi-Fi connection.</li>
                <li>Restart router and computer.</li>
                <li>Run network diagnostics.</li>
                <li>Use <code>ipconfig /release</code> and <code>ipconfig /renew</code>.</li>
                <li>Ping gateway and external websites.</li>
            </ol>

            <button onclick="showMessage('Network troubleshooting completed.')">
                Mark as Resolved
            </button>
        </section>

        <section id="printer" class="guide-card">
            <h2>Printer Troubleshooting</h2>
            <p>Basic printer issue resolution steps.</p>

            <ol>
                <li>Ensure printer is powered on.</li>
                <li>Check USB or network connection.</li>
                <li>Restart print spooler service.</li>
                <li>Reinstall printer drivers.</li>
                <li>Clear stuck print jobs.</li>
            </ol>

            <button onclick="showMessage('Printer troubleshooting completed.')">
                Mark as Resolved
            </button>
        </section>

        <section id="slowpc" class="guide-card">
            <h2>Slow Computer Performance</h2>
            <p>Improve system speed and responsiveness.</p>

            <ol>
                <li>Check Task Manager for high CPU usage.</li>
                <li>Disable unnecessary startup apps.</li>
                <li>Run antivirus scan.</li>
                <li>Delete temporary files.</li>
                <li>Upgrade RAM or SSD if necessary.</li>
            </ol>

            <button onclick="showMessage('PC optimization completed.')">
                Mark as Resolved
            </button>
        </section>

        <section id="email" class="guide-card">
            <h2>Email Troubleshooting</h2>
            <p>Fix common Outlook and email problems.</p>

            <ol>
                <li>Verify internet connection.</li>
                <li>Check mail server settings.</li>
                <li>Clear mailbox storage.</li>
                <li>Reconfigure Outlook profile.</li>
                <li>Test sending and receiving emails.</li>
            </ol>

            <button onclick="showMessage('Email issue resolved.')">
                Mark as Resolved
            </button>
        </section>

    </main>

    <footer>
        <p>Created by Olayinka Shittu | IT Support Portfolio</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
├── style.css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f7fa;
    color: #333;
    line-height: 1.6;
}

header {
    background-color: #0d6efd;
    color: white;
    text-align: center;
    padding: 40px 20px;
}

header h1 {
    margin-bottom: 10px;
    font-size: 2.5rem;
}

nav {
    background-color: #222;
    padding: 15px;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style: none;
    flex-wrap: wrap;
}

nav ul li {
    margin: 10px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

nav ul li a:hover {
    color: #0d6efd;
}

main {
    max-width: 1000px;
    margin: auto;
    padding: 30px 20px;
}

.guide-card {
    background-color: white;
    margin-bottom: 25px;
    padding: 25px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.guide-card h2 {
    color: #0d6efd;
    margin-bottom: 15px;
}

.guide-card p {
    margin-bottom: 15px;
}

.guide-card ol {
    padding-left: 20px;
    margin-bottom: 20px;
}

button {
    background-color: #0d6efd;
    color: white;
    border: none;
    padding: 12px 20px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
}

button:hover {
    background-color: #084298;
}

footer {
    text-align: center;
    background-color: #222;
    color: white;
    padding: 20px;
    margin-top: 30px;
}
├── script.js
function showMessage(message) {
    alert(message);
}

console.log("IT Troubleshooting Guides Loaded Successfully");
├── README.md
# IT Troubleshooting Guides

A collection of IT troubleshooting documentation and step-by-step support guides for common technical issues.

## Features

- Network troubleshooting guides
- Printer issue resolution
- Slow computer performance fixes
- Email troubleshooting procedures
- Beginner-friendly IT support documentation

## Technologies Used

- HTML5
- CSS3
- JavaScript

## Project Structure

it-troubleshooting-guides/
│
├── index.html
├── style.css
├── script.js
└── README.md

## Purpose

This project demonstrates practical IT support knowledge and troubleshooting processes commonly used in helpdesk and system administration roles.

## How to Run

1. Download or clone the repository
2. Open `index.html` in your browser

## Future Improvements

- Add dark mode
- Add search functionality
- Include more troubleshooting categories
- Add screenshots and diagrams

## Author

Olayinka Shittu  
IT Support Administrator
└── images/
