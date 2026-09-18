# Zombie Defense

A Python tower defense game built as my final project for Carnegie Mellon's **15-112: Fundamentals of Programming and Computer Science**. Ranked **Top 8 among 400+ course submissions**.

Defend a wall against increasingly difficult zombies, earn coins for in-game upgrades, and collect gems through a trapping minigame and draggable puzzles.

## Technical highlights

- **Combat and progression:** enemy waves, collision detection, automatic shooting, bombs, upgrades, and two currencies.
- **Graph search:** recursive backtracking on Easy, shortest-path search with pruning on Medium, and breadth-first search with a queue and visited set on Hard.
- **Interactive geometry:** ray casting for point-in-polygon selection, with dragging and snapping for irregular puzzle pieces.
- **Object-oriented design:** six classes model enemies, bullets, soldiers, bonuses, shop items, and puzzle pieces; screen-specific event handlers manage the interface.

## Run locally

Requires Python 3.11–3.14, a desktop display, and an internet connection. Images and audio load from the separate [asset repository](https://github.com/T-ya777/112FinalProjectSource); the game is not self-contained for offline play.

```bash
git clone https://github.com/T-ya777/zombie_defense.git
cd zombie_defense
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python main.py
```

On Windows, use `py` instead of `python3` and activate with `.venv\Scripts\activate`. If installation needs platform-specific setup, follow the [official CMU Graphics instructions](https://academy.cs.cmu.edu/desktop). The CMU Graphics package includes `cmu_cpcs_utils`.

## Controls

- Use the mouse to navigate menus, buy upgrades, and select bonuses.
- Use **Left / Right** arrow keys to move soldiers; shooting is automatic.
- Click the grid to place obstacles in the zombie trapping minigame.
- Drag collected puzzle pieces into place.
- Open the in-game instructions for additional mechanics and settings for audio controls.

## Project layout and notes

`main.py` contains the original game classes, screen handlers, and algorithms. `requirements.txt` lists the runtime dependency. Assets are hosted separately to preserve the original course-project structure.

Verified with Python 3.14.3 and CMU Graphics 2.0.3 on macOS using headless startup and screen initialization checks. Full interactive playthrough and audible playback have not been verified. Desktop fonts may differ if Montserrat is not installed.

Progress is held in memory and resets when the game closes. Original demonstration shortcuts remain enabled and may produce unexpected behavior; normal play uses the controls above. Medium difficulty uses recursive search and may slow down on difficult boards.

## Credits

Created for CMU 15-112 using Python and CMU Graphics. Images were generated with Gemini, music with Suno, and sound effects sourced from Freesound. Individual Freesound creators, source links, and license details still need to be documented. Algorithm references and AI assistance are acknowledged in the source comments.
