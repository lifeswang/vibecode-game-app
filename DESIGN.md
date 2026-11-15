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
   - **Lose:** You have 3 hearts. At 0 hearts, the puzzle restarts.
   - **Start screen:** Before playing, you can type a name (optional, empty means "Guest") and tap "Start game".
   - **Score:** Fastest time wins. A timer runs while you play.
   - **High scores:** After you win, you see your time and a list of the 5 fastest times. Scores are saved in the browser, so they only show on that device.
5. **Visual concept:** Three screens: a start screen (logo, name box, "Start game", "High scores" link), the game board, and a win screen with the time and a high score list. The board is a 6x6 grid with soft, bright colors, one color per zone. Every piece is the same simple red and white Poké Ball. Placing a ball makes it pop in. A wrong move makes the square shake and a heart disappears.
6. **MLP:** See the checklist below.

## 3. Build checklist (MLP)

Work top to bottom. Only start "Can wait" items if the must-haves are done.

### Must have
- [ ] One 6x6 puzzle with a single correct answer
- [ ] Three-tap cycle (✕, ball, empty)
- [ ] Rule checking for rows, columns, zones and touching
- [ ] 3 hearts, and the puzzle restarts at 0
- [ ] "You win" screen and "Try again" button
- [ ] One simple Poké Ball picture
- [ ] Start screen with optional name box and "Start game" button
- [ ] Timer while playing
- [ ] Save scores in the browser and show the 5 fastest times

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

## 5. Progress notes
Add short notes here as you work.

- (date) ...
