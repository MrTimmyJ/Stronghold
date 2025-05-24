# Stronghold
GameDev.tv Game Jam: Last Stand

[Play now on itch.io](https://sourcecodesorcerer.itch.io/stronghold)

Author: Timothy Johnson <br>
Date: May 24, 2024 to June 3, 2024

Defend the central catalyst at all costs! Build towers, survive waves of enemies, and stop the onslaught in this grid-based tower defense shooter.
Made in Godot for the GameDev.TV Game Jam.

## Overview

&nbsp;&nbsp;&nbsp;&nbsp;Stronghold is a 2D top-down tower defense game built in Godot for the GameDev.TV Game Jam.
Your mission: defend the catalyst at the center of the map from endless waves of monsters.
Move your hero using tile-based grid movement and shoot enemies with your blaster. Between waves, construct defensive towers to hold off the incoming threat!

🧩 Features

    🧱 Grid-based player movement (like classic tactics games)

    💥 Blaster weapon to shoot enemies

    🏰 Build towers to automatically attack nearby enemies

    🧠 Enemy waves with scaling difficulty

    🎯 Central catalyst must be protected – game over if it's destroyed

    🛠️ Godot's scene system used for modular towers, enemies, and map design

🎮 Gameplay

You play as the guardian of the catalyst. Move in cardinal directions using grid-based controls and fend off waves of enemies.
After each wave, you get time to build towers in empty spaces around the map. Survive as long as you can.

### Controls:

| Key   | Action |
| ----- | ------ |
| ↑ / W | Move Up     |
| ↓ / S | Move Down   |
| ← / A | Turn Left   |
| → / D | Turn Right  |
| Space | Fire blaster|
| E     | Interact    |
| Esc   | Quit        |

📁 Code Structure

. <br>
├── main.tscn &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Main scene with game loop and HUD <br>
├── player.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Player movement, swimming, and oil laser code <br>
├── oil_area.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Pollution cleanup zone logic <br>
├── laser_beam.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Oil blaster laser behavior <br>
├── ui/ &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Oxygen + cleanup progress bars <br>
├── levels/ &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Tilemaps and level scenes <br>
├── res/ &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Sprites, audio, and background assets <br>
│   ├── knight.png <br>
│   ├── oil_splash.png <br>
│   ├── background_layers/ <br>
│   └── pollution_zones/ <br>

.<br>
├── Game.tscn &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Main game scene<br>
├── Player.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Player movement and shooting<br>
├── Enemy.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Enemy behavior and targeting<br>
├── Tower.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Tower attack logic<br>
├── Catalyst.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Central base health and status<br>
├── WaveManager.gd &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Spawns and escalates enemy waves<br>
├── res/ &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; Sprites, sounds, and maps<br>
│   ├── player.png<br>
│   ├── tower.png<br>
│   ├── enemy.png<br>
│   └── catalyst.png<br>
└── UI/ &nbsp;&nbsp;&nbsp;---&nbsp;&nbsp;&nbsp; UI for health, wave count, build mode, etc.<br>


⚙️ How It Works

Player System

    Player moves in grid-based directions (one tile at a time)

    Shoots in facing direction using Space

Tower Building

    Player enters build mode

    Can place towers on empty tiles if resources are available

    Towers auto-attack enemies in range

Wave System

    Each wave spawns from map edges

    Enemies pathfind toward the catalyst

    Game ends when the catalyst reaches 0 HP

Enemies

    Simple pathfinding toward the catalyst

    Attacks the catalyst or towers if in the way
    
🖼️ Screenshots / Visuals

![strongholdbanner](https://github.com/user-attachments/assets/8d8ad7a8-f5dc-44a3-a117-e865000be223)

🧰 Technologies Used

    🎮 Godot Engine

    🧱 TileMap and Grid Movement System

    ⚙️ Scene-based modular entity design

    🎵 Godot AudioStreamPlayer for sound effects

🚀 Getting Started

    To run this project:

    1. Clone this repository

        git clone https://github.com/MrTimmyJ/stronghold-defense.git
        cd stronghold-defense

    2. Open the project in Godot

       Launch the Godot editor and open the project folder.

    3. Run the game
    
       Click "Play Scene" to start the game.

🌱 Future Improvements

    🧱 More tower types (e.g., slow, AOE, laser beam)

    💣 Exploding enemies and mini-bosses

    🏆 Endless wave mode with online leaderboards

    ⚒️ Upgrade system for towers and player

    🗺️ Multiple maps and difficulty levels

🪪 License

This open-source project is available under the [MIT License](https://opensource.org/license/mit).

