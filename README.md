# Hop Hazard

A single-file arcade Frogger. No build step, no dependencies, no server —
`index.html` is the whole game.

**Play it:** https://caughtsmart.github.io/frogger/

## How to play

Get a frog from the bottom of the screen into each of the five bays at the top.

- **Road** — five lanes of cars and trucks. Touch one and you lose a frog.
- **River** — you can't swim. Ride the logs and turtles across.
- **Diving turtles** — some turtle groups submerge on a cycle. They fade out
  before they go under, which is your warning. They're solid while fading;
  once they're gone, so are you.
- **The power timer** — the strip above the board is your clock. A hand
  creeps toward the plug, and its distance to the socket is the time you have
  left. Its fingers curl into a fist over the last few seconds. At zero it
  yanks the plug, the screen dies like an old CRT, and you lose a frog.
- **Levelling up** — fill all five bays and everything speeds up 22%, capped
  at 3× by level 10. The turtles dive more often too.

Three frogs, 32 seconds each.

## Controls

| Input | Action |
| --- | --- |
| Arrow keys / WASD | Hop |
| Swipe the board | Hop in that direction |
| Tap the board | Hop forward |
| On-screen D-pad | Hop (touch devices) |
| `P` | Pause (it also pauses if the window loses focus) |
| Speaker icon | Mute |

## Scoring

- 10 per new row reached
- 50 plus a time bonus per bay filled
- 1000 per level cleared

High scores are saved in your own browser, so each person who opens the page
keeps their own table.

## Running it locally

Open `index.html` in any browser — double-clicking works.

Note that iOS will not run the game from a file sent through a messaging app:
tapping an HTML attachment opens Apple's QuickLook preview, which renders the
page but does not execute JavaScript, so the board stays blank and the Start
button does nothing. Use the hosted link above on a phone.

The only external resource is the arcade font from Google Fonts. Offline it
falls back to a monospace stack and plays identically.
