# 🏓 Table Tennis Tournament

A real-time table tennis tournament tracker with a built-in **parimutuel betting system** using virtual Fun Points (FP). Built as a single-page web app powered by Firebase.

> **[🔴 Live Demo](https://table-tenis-tournament.onrender.com)**

---

## ✨ Features

- **🏟️ Group Stage** — 4 groups of 4 players with live W/L/Pts standings
- **🏆 Knockout Bracket** — Quarterfinals → Semifinals → Final with automatic winner propagation
- **💰 Parimutuel Betting** — Place bets with Fun Points on upcoming matches; odds shift in real time based on the pool
- **📊 Live Leaderboard** — Track everyone's FP balance and betting stats
- **🔐 Authentication** — Firebase Auth with email/password (login & register)
- **⚙️ Admin Panel** — Manage users, edit players/groups, set match results, and resolve bets
- **📱 Mobile-First** — Fully responsive with hamburger sidebar and bottom-sheet modals
- **🔄 Real-Time Sync** — All data synced live via Firebase Realtime Database

---

## 📂 Project Structure

```
├── assets/              # Images (logo, backgrounds)
├── css/
│   └── tournament.css   # Custom styles (match cards, brackets, badges)
├── scripts/
│   ├── build.sh             # Generates config.js from env vars at deploy
│   └── config.example.js    # Firebase config template
├── index.html           # Redirect → tournament.html
├── tournament.html      # Main app (HTML + JS)
├── render.yaml          # Render deployment config
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

- A [Firebase](https://firebase.google.com/) project with **Authentication** (Email/Password) and **Realtime Database** enabled

### Local Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/MikiTsegaye/Table-Tenis-Tournament.git
   cd Table-Tenis-Tournament
   ```

2. **Create your config file**
   ```bash
   cp scripts/config.example.js config.js
   ```

3. **Fill in your Firebase credentials** in `config.js`

4. **Open `tournament.html`** in a browser — that's it, no build step needed!

### Deploy to Render

1. Connect your GitHub repo as a **Static Site** on [Render](https://render.com)
2. Set **Build Command** to `bash scripts/build.sh`
3. Set **Publish Directory** to `.`
4. Add your Firebase credentials as **Environment Variables**:

   | Variable | Description |
   |---|---|
   | `FIREBASE_API_KEY` | Firebase API key |
   | `FIREBASE_AUTH_DOMAIN` | e.g. `your-project.firebaseapp.com` |
   | `FIREBASE_DATABASE_URL` | e.g. `https://your-project-default-rtdb.firebaseio.com` |
   | `FIREBASE_PROJECT_ID` | Firebase project ID |
   | `FIREBASE_STORAGE_BUCKET` | e.g. `your-project.firebasestorage.app` |
   | `FIREBASE_MESSAGING_SENDER_ID` | Sender ID |
   | `FIREBASE_APP_ID` | Firebase App ID |
   | `FIREBASE_MEASUREMENT_ID` | Google Analytics measurement ID |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML/CSS/JS |
| Styling | [Tailwind CSS](https://tailwindcss.com/) (CDN) + custom CSS |
| Auth | Firebase Authentication |
| Database | Firebase Realtime Database |
| Hosting | [Render](https://render.com) (Static Site) |

---

## 📸 Screenshots

<details>
<summary>Click to expand</summary>

### Login
The app greets users with a clean login/register overlay.

### Group Stage
Four groups with live win/loss standings and qualification badges.

### Knockout Bracket
Visual bracket with match cards, live odds bars, and bet buttons.

### Betting Modal
Pick a winner, set your wager, and see estimated payout before confirming.

</details>

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
