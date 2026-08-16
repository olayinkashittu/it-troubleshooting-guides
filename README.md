## Repository Structure

- docs/
  - Active-Directory/
  - Hardware/
  - Linux/
  - Microsoft-365/
  - Networking/
  - Windows/
- images/
- index.html
  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IT Troubleshooting Guides</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

<header>
    <h1>IT Troubleshooting Guides</h1>
    <p>Windows | Active Directory | Networking | Linux | Microsoft 365 | Hardware</p>
</header>

<nav>
    <ul>
        <li><a href="#windows">Windows</a></li>
        <li><a href="#networking">Networking</a></li>
        <li><a href="#microsoft365">Microsoft 365</a></li>
        <li><a href="#linux">Linux</a></li>
        <li><a href="#hardware">Hardware</a></li>
        <li><a href="#active-directory">Active Directory</a></li>
    </ul>
</nav>

<main>

<section id="windows">
    <h2>Windows</h2>
    <ul>
        <li>Blue Screen Troubleshooting</li>
        <li>Slow Computer Troubleshooting</li>
        <li>Software Installation Troubleshooting</li>
        <li>Windows Update Troubleshooting</li>
    </ul>
</section>

<section id="networking">
    <h2>Networking</h2>
    <ul>
        <li>DHCP Troubleshooting</li>
        <li>DNS Troubleshooting</li>
        <li>IP Configuration Commands</li>
        <li>Network Connectivity Troubleshooting</li>
        <li>VPN Troubleshooting</li>
        <li>Wi-Fi Troubleshooting</li>
    </ul>
</section>

<section id="microsoft365">
    <h2>Microsoft 365</h2>
    <ul>
        <li>Mailbox Issues</li>
        <li>Outlook Troubleshooting</li>
        <li>Password Reset</li>
        <li>Microsoft Teams Troubleshooting</li>
    </ul>
</section>

<section id="linux">
    <h2>Linux</h2>
    <ul>
        <li>File Permissions</li>
        <li>Networking Commands</li>
        <li>SSH Troubleshooting</li>
        <li>User Management</li>
    </ul>
</section>

<section id="hardware">
    <h2>Hardware</h2>
    <ul>
        <li>Bluetooth Troubleshooting</li>
        <li>Keyboard Troubleshooting</li>
        <li>Monitor Troubleshooting</li>
        <li>Printer Troubleshooting</li>
    </ul>
</section>

<section id="active-directory">
    <h2>Active Directory</h2>
    <ul>
        <li>Account Lockout</li>
        <li>Group Policy</li>
        <li>Organizational Units</li>
        <li>Password Reset</li>
        <li>User Management</li>
    </ul>
</section>

</main>

</body>
</html>
- script.js

document.addEventListener("DOMContentLoaded", function () {

    const sections = document.querySelectorAll("section");

    sections.forEach(function (section) {

        section.addEventListener("click", function () {

            this.scrollIntoView({
                behavior: "smooth"
            });

        });

    });

    console.log("IT Troubleshooting Guides loaded successfully.");

});
- style.css
body {
    font-family: Arial, sans-serif;
    margin: 40px;
    line-height: 1.6;
}

header {
    text-align: center;
    margin-bottom: 40px;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav li {
    display: inline-block;
    margin-right: 15px;
}

section {
    margin-top: 40px;
}

h1,
h2 {
    border-bottom: 1px solid;
    padding-bottom: 10px;
}

a {
    text-decoration: none;
}

ul li {
    margin-bottom: 8px;
}
- README.md
  
