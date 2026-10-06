# 🚀 Fly Away

A hyper-casual 2D side-scrolling space game built in **Unity** with **C#**.

Guide your astronaut through open space with the mouse or your finger. Stay inside the endless boundary lines, dodge asteroids and UFOs, and score as high as you can before your lives run out.

<p align="center">
  <img src="ScreenShot/Main%20Menu.png" width="600">
</p>

## 🎮 Gameplay Video

- [Watch on PC](https://drive.google.com/file/d/1X7UKYSgf5LBtztLGRZiCEiIObZw9U5hd/view?usp=drive_link)
- [Watch on Mobile](https://drive.google.com/file/d/1dyQIuD5MGBcrtMfoFG7NGFO6bZmctoiY/view?usp=drive_link)

## ▶️ Play the Game

- **Download:** [Latest release](https://github.com/sriram-game-dev/Fly-Away/releases) (Windows build)

## ✨ Features

- Mouse / touch controlled player kept inside the camera view
- Endless scrolling space background
- Random asteroids and UFOs spawning at intervals
- Boundary lines at the top and bottom of the screen that change shape
- Score increases each time you avoid an enemy
- 3-lives system with on-screen life icons
- Game speed increases over time using `Time.timeScale`
- Animated player, asteroids and UFOs using Unity's Animator
- Main menu (Play, Settings, Quit) and Game Over screen with Restart and Home buttons

## 🕹️ Controls

| Platform | Control |
|----------|---------|
| PC | Move the mouse |
| Android phone / tablet | Touch and drag (landscape mode) |

## 🧩 How It Works

| Script | Purpose |
|--------|---------|
| `PlayerController.cs` | Moves the player to the pointer position, keeps it inside the camera bounds, and reduces a life on collision with an `Enemy` or `Border` tag |
| `BaseEnemy.cs` | Moves enemies toward the player, awards score when avoided, and speeds up as the game progresses |
| `GameManager.cs` | Spawns random enemy prefabs with `InvokeRepeating`, tracks score and lives, handles Game Over and restart |
| `RepeatBackground.cs` | Loops the background using a `repeatWidth` value |
| `MainMenu.cs` | Loads the game scene with `SceneManager` and quits the application |

## 🛠️ Built With

- **Engine:** Unity
- **Language:** C#
- **UI:** TextMeshPro
- **Target platforms:** PC, Android phone and tablet (landscape)

## 📂 Repository Contents

```
Fly-Away/
├── Demo Gamplay video/
├── Project Document/
├── ScreenShot/
└── README.md
```

## 📄 Design Document

The full game design document is here: [Fly_Away_Design_Document.pdf](Project%20Document/Fly_Away_Design_Document.pdf)

## 🗺️ Roadmap

- [ ] Power-up objects for bonus points
- [ ] High score board
- [ ] Sound effects

## 👤 Author

**S. Sriram**
- GitHub: [@sriram-game-dev](https://github.com/sriram-game-dev)
- Portfolio: [sriram-game-dev.github.io/profile](https://sriram-game-dev.github.io/profile/)
