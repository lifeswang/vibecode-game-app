# Poké Ball Grid: Design and Plan

A puzzle game where you place one Poké Ball in every row, column and color zone, and no two balls can touch.

## 1. Play and analyze

### Games I played
- **Mewdoku (Meow Doku):** A cat puzzle on a colored grid. It's calm and cute, and it rewards thinking more than speed. A wrong guess costs a heart, so I slow down and check first.
- **Teriks:** A falling-block game. It's more stressful. It speeds up, and one bad move makes the next ones harder. Clearing several lines at once feels great.

### Core mechanics
- **Mewdoku:** Place a cat on a square. One cat per row, column and color zone, and cats can't touch.
- **Teriks:** Move and rotate a falling piece so it fits. It's about timing and fitting shapes.

### My chosen mechanic
Placing things on a grid under simple rules (the Meow Doku mechanic).
- I enjoyed it more because I like figuring things out more than racing a clock.
- The rules are easy to explain, but it still makes you think.
- It's doable in 1.5 hours: one action, a small grid, one way to win and one way to lose.

## 2. Game design

1. **Game name:** Poké Ball Grid
2. **One-sentence description:** A puzzle game where you place one Poké Ball in every row, column and color zone, and no two balls can touch.
3. **My twist:** It's Meow Doku, but with Poké Balls instead of cats. The "no touching" rule is the main challenge, because each ball blocks the 8 squares around it.
4. **Basic rules and goal:**
   - Tap a square to cycle through three states: ✕ (a reminder to yourself), Poké Ball, then empty.
   - **Win:** Every row, column and color zone has exactly one ball, and none of them touch.
   - **Mistakes:** If you place a ball that breaks a rule, you lose a heart and that ball disappears.
   - **Lose:** You have 5 hearts. At 0 hearts, the puzzle restarts.
   - **Start screen:** Before playing, you can type a name (optional, empty means "Guest") and tap "Start game".
   - **Score:** Fastest time wins. A timer runs while you play.
   - **High scores:** After you win, you see your time and a list of every player's time, fastest first. Scores are saved in the browser, so they only show on that device.
5. **Visual concept:** Three screens: a start screen (logo, name box, "Start game", "High scores" link), the game board, and a win screen with the time and a high score list. The board is a 4x4 grid with soft, bright colors, one color per zone. Every piece is the same simple red and white Poké Ball. Placing a ball makes it pop in. A wrong move makes the square shake and a heart disappears.
6. **MLP:** See the checklist below.

## 3. Build checklist (MLP)

Work top to bottom. Only start "Can wait" items if the must-haves are done.

### Must have
- [x] One 4x4 puzzle with a single correct answer
- [x] Three-tap cycle (✕, ball, empty)
- [x] Rule checking for rows, columns, zones and touching
- [x] 5 hearts, and the puzzle restarts at 0
- [x] "You win" screen and "Try again" button
- [x] One simple Poké Ball picture
- [x] Start screen with optional name box and "Start game" button
- [x] Timer while playing
- [x] Save scores in the browser and show every player's time, fastest first

### Can wait
- [ ] More levels and bigger boards
- [ ] Free starting ball on early levels
- [ ] Daily puzzle
- [ ] Sound effects
- [ ] Hints
- [ ] Different ball types (Great Ball, Ultra Ball)
- [ ] Mini-games and side quests

## 4. Decisions so far
- Zones are only colors. Every ball looks the same.
- A wrong ball disappears and costs one heart.
- The MLP ships one hand-made puzzle, not a random generator.
- Name is optional (default "Guest"). Score is fastest time. Scores are saved in the browser only.

## 5. How to build (read this when I say "start building")
- **Tech:** Plain HTML, CSS and JavaScript in a single `index.html` file at the repo root. No frameworks, no installs. Open it by double-clicking.
- **What to build:** The "Must have" checklist above, in order, matching `design/design-mockup.png` (four screens: start, playing, win, high scores).
- **Puzzle:** One hand-made 4x4 puzzle with a single correct answer. Zone layout and solution are in the mockup's board.
- **Scores:** Saved in the browser with `localStorage`. Show every player's time, fastest first.
- **Before pushing:** Show me the working game first and wait for my approval. Then take screenshots of the real game, add them to the README, and tick the checklist.
- **Do not add** anything from "Can wait" until the must-haves are done.

## 6. Progress notes
Add short notes here as you work.

- 2026-11-18: Built `index.html` with all must-haves. The zone layout in the mockup had 30 possible answers, so the game uses a new layout with exactly one answer (checked by brute force). Screenshots of the real game are in `screenshots/`.
- 2026-11-19: Made the game "super beginner": 4x4 board, 2 free balls that can't be removed, and 5 hearts. The puzzle has exactly one answer.
