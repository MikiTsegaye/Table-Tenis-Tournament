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

