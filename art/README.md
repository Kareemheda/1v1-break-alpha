# Character art

One folder per character: `swordsman`, `archer`, `mage`, `paladin`, `demon`, `vampire`, `cavalryman`, `gunner`.

Name each frame `<action>-<number>.png`, numbered from 1 with no gaps:

| Action | Files |
|---|---|
| Standing | `standing-1.png`, `standing-2.png`, ... |
| Attacking | `attacking-1.png`, ... |
| Blocking | `blocking-1.png`, ... |
| Hurt | `hurt-1.png`, ... |

- Canvas 120 x 144 pixels, transparent, the character facing **right**, feet on row 140 (see `design/pixel-fable/art-brief.md`).
- The game plays whatever frames are in the folder, in number order. Adding or replacing frames needs no code change and no build: just reload the game.
- One frame for an action: the game moves it in code (a bob while standing, a lunge to attack, a step back to block, a jolt back when hurt).
- No frame for an action: the standing frames are used. No standing frame: a labelled placeholder is drawn.
