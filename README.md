# Poké Ball Grid

A small puzzle game where you place one Poké Ball in every row, column and color zone, and no two balls can touch.

It's inspired by Meow Doku, a cat puzzle game, but with Poké Balls instead of cats. This is a class project, built in about 1.5 hours.

## How to play
- Tap a square to cycle through three states: ✕ (a reminder to yourself), Poké Ball, then empty.
- Put exactly one ball in every row, every column and every color zone.
- Balls can't touch, even diagonally.
- A wrong ball costs one heart and disappears. You have 3 hearts, and the puzzle restarts at 0.
- You win when every row, column and zone has one ball.
- Enter a name (or leave it empty) on the start screen. Your time is saved, and everyone's time goes on a list, fastest first, so you can see who won.

## How to run
Open `index.html` in a browser (double-click it). There is nothing to install.

## Screenshots
| Start | Playing (one mistake) |
|---|---|
| ![Start screen](screenshots/start.png) | ![Playing](screenshots/playing.png) |

| Win | High scores |
|---|---|
| ![Win screen](screenshots/win.png) | ![High scores](screenshots/scores.png) |

The high score names in these screenshots are demo data.

## Design
The original plan is in [DESIGN.md](DESIGN.md), with a design mockup in `design/design-mockup.png`.

## Status
The first playable version is built (one 6x6 puzzle, hearts, timer, and a saved high score list for all players).

## More info
See [DESIGN.md](DESIGN.md) for the full design, the build checklist and progress notes.
