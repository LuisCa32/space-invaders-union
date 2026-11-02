# Space Invaders Union

[![Space Invaders Union: aliens on a picket line holding protest signs while their union rep announces a deal](og-image.png)](https://luisca32.github.io/space-invaders-union/)

**[▶ Play it in your browser](https://luisca32.github.io/space-invaders-union/)**. It's free, works on phones and desktops, and a run takes about a minute.

Classic Space Invaders, except the aliens have organized. Partway through every wave they go
on strike: they stop shooting, form a picket line, and hold up tiny protest signs ("FAIR WAGES
FOR INVADERS", "WE WANT DENTAL", "NO MORE LASERS WITHOUT BREAKS").

- **Hold your fire** and the union rep negotiates a deal. The aliens go back to work.
- **Shoot a striker** and you get a **UNION VIOLATION**. The rest of the wave gets angrier and
  faster. Three violations in one strike and they walk out in a **wildcat rage**.

Clear all three waves and HR hands you your **Labor Relations Score**, from
*A+ Beloved Overlord* down to *F Galactic Labor Criminal*.

## Controls

| | Phone / tablet | Desktop |
|---|---|---|
| Move | Drag anywhere in the bottom third of the screen | ← / → or A / D |
| Fire | Hold the **FIRE** button | Hold Space |
| Pause | ⏸ button (top right) | P or Esc |
| Mute | 🔈 button (top right) | M |

The game pauses on its own when you switch tabs or apps.

## How it plays

- 3 waves (Morning Shift, Overtime, Graveyard Shift), each bigger and faster than the last.
- The strike starts at a random point once 40–60% of the wave's aliens are left.
- You have 3 lives. You lose if the aliens shoot you 3 times or reach the ground.
- Labor Relations Score = 60 + 15 for each strike you let finish − 10 for each union
  violation, kept between 0 and 100.

## Run it locally

The whole game is a single `index.html` with no dependencies or build step. The graphics are
drawn in code on a `<canvas>`, and the sounds come from the Web Audio API.

```bash
git clone https://github.com/LuisCa32/space-invaders-union.git
cd space-invaders-union
python3 -m http.server 8000
```

Then open <http://localhost:8000>. You can also open `index.html` directly in a browser.
