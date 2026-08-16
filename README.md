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

<p>
Real-world troubleshooting documentation covering Windows, Active Directory,
Networking, Linux, Microsoft 365, and Hardware support.
</p>
</header>

<nav>
<ul>
<li><a href="docs/Windows/">Windows</a></li>
<li><a href="docs/Active-Directory/">Active Directory</a></li>
<li><a href="docs/Networking/">Networking</a></li>
<li><a href="docs/Linux/">Linux</a></li>
<li><a href="docs/Microsoft-365/">Microsoft 365</a></li>
<li><a href="docs/Hardware/">Hardware</a></li>
</ul>
</nav>

<section>
<h2>Repository Structure</h2>

<ul>
<li>Windows Troubleshooting</li>
<li>Active Directory Troubleshooting</li>
<li>Networking Troubleshooting</li>
<li>Linux Troubleshooting</li>
<li>Microsoft 365 Troubleshooting</li>
<li>Hardware Troubleshooting</li>
</ul>
</section>

<script src="script.js"></script>

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
  
