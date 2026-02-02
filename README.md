# 🏆 LEC Versus 2026 Predictor

An interactive simulation tool designed for League of Legends esports fans. This tool allows users to predict the outcomes of the final week of the **LEC Versus 2026** regular season, automatically generate the final standings, and simulate the entire Double Elimination playoff bracket.

## 🚀 Key Features

### 1. Regular Season (Week 4)

* **One-Click Predictions**: Simply click on a team's button to declare them the winner of their match.
* **Live Standings**: The leaderboard updates instantly as you make your predictions.
* **Tie-break Engine**: The simulator strictly follows official "Head-to-Head" rules. If two teams are tied in wins, the result of their direct confrontation (past or predicted) determines their rank.

### 2. Playoff Bracket (Double Elimination)

* **Automatic Seeding**: The top 8 teams from the standings are automatically placed into the Upper Bracket.
* **Dynamic Lower Bracket**: Losers from the Upper Bracket are automatically dropped into the appropriate slots in the Lower Bracket following the official LEC format.
* **Score Management**: Manual score entry for every match to track series results (e.g., 2-1, 3-2).
* **Bo3 & Bo5 Formats**: Visual distinction and logic for Best-of-3 and Best-of-5 series (Grand Final and Lower Finals).

---

## 📂 Project Structure

```bash
├── index.html   # Main layout and bracket containers
├── style.css    # Custom UI styling, animations, and scrollbars
└── script.js    # Calculation logic, tie-break engine, and state management

```

---

## 🛠️ Setup & Installation

1. **Download/Clone** the project files.
2. Ensure that all three files (`index.html`, `style.css`, `script.js`) are located in the same directory.
3. Open `index.html` in any modern web browser (Chrome, Firefox, or Edge recommended).

---

## ⚖️ Simulation Rules

### Standings Calculation

The team ranking is calculated based on the following hierarchy:

1. **Win Count**: Total accumulated wins (Initial + Predicted).
2. **Dynamic Head-to-Head**: If Team A beats Team B during the season (or in your predictions), they will be ranked higher in case of a tie.
3. **Alphabetical Order**: Used only as a final tie-breaker if teams are perfectly tied.

### Playoff Progression

* **Advancing**: Click on a team's name within the bracket to advance them to the next round.
* **Dropping to Lower**: If you change the winner of an Upper Bracket match, the new loser is automatically updated and sent to the Lower Bracket.
* **Fearless Draft**: While the tool does not manage the draft phase, the UI reflects the Bo3/Bo5 rules inherent to the 2026 Fearless format.

---

## 🎨 Customization

To update the current standings (pre-Week 4) or change team names, edit the `teams` and `headToHead` constants at the beginning of the `script.js` file.

---

## 📝 License

This project is free to use for the LEC community.

*Developed with passion for the European competitive scene.* 🎮🔥

---
