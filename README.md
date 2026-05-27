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
├── script.js
├── README.md
└── images/
