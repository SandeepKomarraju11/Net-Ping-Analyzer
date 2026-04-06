# Net-Ping-Analyzer

⚠ Disclaimer

This tool is created strictly for academic and defensive cybersecurity learning. It should only be used on systems you own or have explicit permission to test.

Any misuse of this tool for unauthorized network probing is illegal. The developer is not responsible for misuse.

📌 Overview

NetPing Analyzer is a Python-based command-line utility designed to perform basic network diagnostics using ICMP (ping).

It allows users to:

Resolve domain names into IP addresses Execute customizable ping commands Analyze response behavior Generate a structured report

This project is developed as part of an Ethical Hacking lab exercise.

✨ Key Features

✔ Domain → IP resolution using socket ✔ Cross-platform support (Windows/Linux/macOS) ✔ Flexible ping parameter selection ✔ Real-time output display ✔ Automatic report generation ✔ Simple and interactive CLI

🛠 System Requirements Python 3.6+ No external libraries required

Uses built-in modules:

subprocess socket platform datetime sys 📦 Setup Instructions git clone cd netping-analyzer python netping_analyzer.py 🚀 How to Use Run the script Enter a target domain (e.g., google.com) Select a ping mode Provide value (or use default) View results Save report (optional) 📡 Available Modes Mode Description count Number of packets size Packet size ttl Time-to-live value timeout Response wait time flood Continuous ping df Don't fragment test 🖥 Example Output [INFO] Domain: google.com [INFO] IP Address: 142.250.183.14

Running: ping -c 4 google.com

Reply from 142.250.183.14: time=45ms Reply from 142.250.183.14: time=42ms Reply from 142.250.183.14: time=44ms Reply from 142.250.183.14: time=43ms

Summary: Packets Sent: 4 Packets Received: 4 Loss: 0% Average Time: ~43ms 📁 Project Layout netping-analyzer/ │ ├── netping_analyzer.py ├── reports/ │ └── report_*.txt └── README.md 👤 Author

Your Name Here

🎓 Academic Context

Developed as part of a cybersecurity / ethical hacking practical to understand ICMP-based network probing techniques.

Repository
