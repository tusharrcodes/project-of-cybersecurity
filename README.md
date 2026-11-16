# 🛡️ SSH & Web Honeypot Dashboard

<p align="center">
  <b>A clean, interactive cybersecurity honeypot dashboard built with pure HTML, CSS & JavaScript.</b>
</p>

<p align="center">
  <a href="#-live-demo">Live Demo</a> •
  <a href="#-features">Features</a> •
  <a href="#-how-it-works">How It Works</a> •
  <a href="#-project-structure">Project Structure</a> •
  <a href="#-getting-started">Getting Started</a>
</p>

---

## 🚀 Live Demo

**[▶️ Open the Honeypot Dashboard](https://tusharrcodes.github.io/project-of-cybersecurity/)**

> Replace the link above with your GitHub Pages URL after enabling GitHub Pages.

---

## 📌 About The Project

**SSH & Web Honeypot Dashboard** is an educational cybersecurity project that demonstrates how a honeypot can collect and visualize suspicious login activity.

The project provides a simulated environment for monitoring:

- 🔐 SSH login attempts
- 🌐 Web login attempts
- 👤 Common usernames
- 🔑 Common passwords
- 🌍 Source IP addresses
- 🕒 Attack timestamps
- 🤖 User-agent information
- 🚨 Security alerts
- 📊 Attack activity statistics

The interface is designed as a modern security operations dashboard so that attack activity can be understood at a glance.

> ⚠️ **Important:** This GitHub Pages version is a **frontend simulation for educational/demo purposes**. It does not expose a real SSH server or collect traffic from external attackers.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🛡️ Honeypot Dashboard | Modern cybersecurity monitoring interface |
| 🔐 SSH Simulation | Generates fake SSH attack events |
| 🌐 Web Login Simulation | Generates fake web credential attempts |
| 🚨 Attack Alerts | Displays real-time simulated alerts |
| 📊 Attack Chart | Visualizes attack activity |
| 👤 Username Analysis | Shows frequently targeted usernames |
| 🔑 Password Analysis | Shows commonly attempted passwords |
| 🌍 IP Analysis | Tracks simulated source IP addresses |
| 🧾 Attack Logs | Displays recent attack details |
| 💾 Local Storage | Keeps demo data in the browser |
| 📥 JSON Export | Download attack data as a report |
| 📱 Responsive UI | Works on desktop, tablet and mobile |
| 📦 Zero Dependencies | No frameworks or packages required |

---

## 🖥️ Dashboard Preview

The dashboard contains:

```text
┌─────────────────────────────────────────────────────────────┐
│              🛡️ SSH & Web Honeypot                         │
│             Attack Monitoring Dashboard                     │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  Total Attacks   SSH Attacks   Web Attacks   Source IPs    │
│       10              5             5             4        │
│                                                             │
├─────────────────────────────┬───────────────────────────────┤
│                             │                               │
│      📊 Attack Activity     │       👤 Top Usernames       │
│                             │                               │
│      ▂ ▅ ▃ ▇ ▆ █ ▄         │       admin       4          │
│      ▁ ▃ ▅ ▄ ▇ ▆ █         │       root        3          │
│                             │       guest       2          │
│                             │                               │
├─────────────────────────────┼───────────────────────────────┤
│                             │                               │
│      🧾 Attack Logs         │       🌐 Source IPs           │
│                             │                               │
│      SSH  192.168.1.10      │       192.168.1.10    4       │
│      WEB  10.0.0.25         │       10.0.0.25       3       │
│                             │                               │
└─────────────────────────────┴───────────────────────────────┘
```

---

## 🧠 How It Works

The project simulates attacker behaviour inside the browser.

### 1. Simulate an SSH Attack

Click:

**`Simulate SSH Attack`**

The application generates a simulated event containing:

```text
Service      → SSH
Source IP    → Random simulated IP
Username     → Random common username
Password     → Random common password
User-Agent   → Random client
Timestamp    → Current browser time
```

### 2. Simulate a Web Attack

Click:

**`Simulate Web Login`**

A fake web credential attempt is generated and added to the dashboard.

### 3. Generate Multiple Attacks

Click:

**`Generate 10 Attacks`**

The dashboard automatically creates ten simulated attack events.

### 4. Store Data

Attack events are stored using the browser's:

```text
localStorage
```

This means the dashboard can remember the demo data even after refreshing the page in the same browser.

### 5. Export Data

Click:

**`Download Report`**

The application generates a JSON file containing the simulated attack data.

---

## 🏗️ Technology Stack

### Frontend

- **HTML5** — page structure
- **CSS3** — responsive dashboard design
- **JavaScript** — simulation, statistics and interaction
- **Canvas API** — attack activity chart
- **LocalStorage API** — browser-side data persistence

### No External Dependencies

This project does **not** require:

- React
- Node.js
- Python packages
- Flask
- Bootstrap
- jQuery
- Database server
- Backend server

Just open the HTML file and run it.

---

## 📂 Project Structure

```text
ssh-web-honeypot/
│
├── index.html       # Main honeypot dashboard
├── README.md        # Project documentation
└── assets/          # Optional images/screenshots
```

If you use GitHub Pages, `index.html` should be located in the repository's root directory.

---

## ⚡ Getting Started

### Option 1 — Run Locally

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

Enter the project directory:

```bash
cd YOUR-REPOSITORY
```

Then open:

```text
index.html
```

in your browser.

### Option 2 — Run on GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`.
3. Upload this `README.md`.
4. Open **Settings → Pages**.
5. Select **Deploy from a branch**.
6. Select the `main` branch and `/root` folder.
7. Save the settings.
8. GitHub will provide your live website URL.

Your project will then be accessible through GitHub Pages.

---

## 🎮 Demo Controls

| Button | Action |
|---|---|
| `Simulate SSH Attack` | Creates one fake SSH attack |
| `Simulate Web Login` | Creates one fake web attack |
| `Generate 10 Attacks` | Creates ten simulated attacks |
| `Reset Data` | Clears all browser-stored attack data |
| `Download Report` | Downloads attack data as JSON |

---

## 📊 Information Collected By The Demo

Each simulated attack contains:

```json
{
  "time": "Current browser time",
  "service": "SSH or WEB",
  "ip": "Simulated IP address",
  "username": "Simulated username",
  "password": "Simulated password",
  "agent": "Simulated user-agent"
}
```

All values are generated locally for demonstration purposes.

---

## 🔐 Security & Ethics

This project is intentionally designed as a **safe educational simulation**.

It does **not**:

- ❌ Attack external systems
- ❌ Scan the internet
- ❌ Collect real people's credentials
- ❌ Provide a real SSH shell
- ❌ Execute attacker commands
- ❌ Attempt unauthorized access

It is intended for learning about:

- Honeypots
- Cybersecurity monitoring
- Attack detection
- Security dashboards
- Log analysis
- Frontend development

Only deploy a real honeypot in an environment you own or have explicit authorization to monitor.

---

## 🎓 Project Objectives

This project demonstrates the following cybersecurity concepts:

- **Honeypot technology**
- **Attack logging**
- **Credential attack detection**
- **IP-based monitoring**
- **Security alerts**
- **Threat visualization**
- **Incident monitoring**
- **Security dashboard design**

It also demonstrates practical frontend development using vanilla HTML, CSS and JavaScript.

---

## 🔮 Future Improvements

Possible future versions could include:

- [ ] Real backend API
- [ ] SQLite/PostgreSQL storage
- [ ] Real SSH honeypot in an isolated lab
- [ ] Real-time WebSocket monitoring
- [ ] GeoIP visualization
- [ ] Attack heat map
- [ ] Login attempt rate detection
- [ ] Brute-force detection
- [ ] Email/Discord security alerts
- [ ] Admin authentication
- [ ] Docker deployment
- [ ] SIEM integration

---

## ⭐ If You Like This Project

If this project helped you learn something about cybersecurity or web development, consider giving the repository a ⭐ on GitHub.

---

## 👨‍💻 Author

**Tushar Bajpai & Aviral**

Cybersecurity • Web Development • Security Monitoring

---

<p align="center">
  <b>🛡️ Learn. Monitor. Detect. Secure.</b>
</p>
