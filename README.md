# 📜 Timeline Tactician

**Subject:** History / Technology (chronological reasoning)
**File:** `history-game.html`

## 🌐 Play Online
```

```

## 📖 About
A chronological ordering puzzle. Each round presents 5 cards representing real-world events, inventions, or milestones (e.g. the Printing Press, the Moon Landing, the first smartphone) in a shuffled order. Tap two cards to swap their positions until they're arranged from **oldest to newest**, then submit to check your answer.

## 🎮 How to Play
1. Each round shows 5 cards from a themed category (e.g. *Communication Inventions*, *Space Exploration Milestones*).
2. Tap/click one card to **select** it — it lifts up.
3. Tap/click a second card to **swap** their positions.
4. Arrange the cards from **OLDEST (left)** to **NEWEST (right)**.
5. Press **Submit** to check your order:
   - Correct positions turn **green**
   - Incorrect positions turn **red** and shake
6. An incorrect submission costs 1 life (❤️) — but the cards reset so you can keep adjusting and resubmit.
7. A correct full order gives a score bonus (including a time bonus) and advances to the next round.
8. Complete all 4 rounds before running out of lives or time!

## ✅ Features
- Start screen + instructions screen
- Score tracking (partial credit for each correctly placed card, plus bonuses for a perfect round)
- 3 lives (❤️)
- 45-second timer per round (visual shrinking bar)
- 4 themed rounds: Communication Inventions, Space Exploration, Transportation, Computing & Internet Era
- Click/tap-to-swap mechanic — works reliably on both desktop and mobile (no drag-and-drop required)
- Sound effects + a "ticking clock" themed looping background music (Web Audio API, no external files)
- End-game screen with star rating (⭐ 1–3) based on final score
- Play Again button
- Mute/unmute toggle

## 🛠️ Customization
Key constants near the top of the `<script>` section:
- `TOTAL_ROUNDS` — number of rounds (default: 4, matches the number of categories)
- `STARTING_LIVES` — number of lives (default: 3)
- `ROUND_TIME` — seconds per round (default: 45)
- `categories` array — each category has a `title` and a list of 5 `{name, year, emoji}` items; add new categories or edit existing ones to change content. The correct order is automatically calculated by sorting on `year`.

## 💻 Running Locally
Just open `history-game.html` in any modern browser — no installation or build steps required. For live-reload while editing, use the VS Code "Live Server" extension.
