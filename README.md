# 🚀 Fly Away

A hyper-casual 2D side-scrolling space game built in **Unity** with **C#**.

Guide your astronaut through open space with the mouse or your finger. Stay inside the endless boundary lines, dodge asteroids and UFOs, and score as high as you can before your lives run out.

![Gameplay](Screenshots/gameplay.png)

## 🎮 Gameplay Video

- [Watch on PC](ADD-PC-VIDEO-LINK-HERE)
- [Watch on Mobile](ADD-MOBILE-VIDEO-LINK-HERE)

## ▶️ Play the Game

- **Download:** [Latest release](../../releases) (Windows build)
- **Play in browser:** ADD-ITCH.IO-OR-GITHUB-PAGES-LINK-HERE

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

- **Engine:** Unity (version: check `ProjectSettings/ProjectVersion.txt`)
- **Language:** C#
- **UI:** TextMeshPro
- **Target platforms:** PC, Android phone and tablet (landscape)

## 📂 Project Structure

```
Fly-Away/
├── Assets/
│   ├── Scripts/
│   ├── Prefabs/
│   ├── Scenes/
│   ├── Animation/
│   └── Sprites/
├── Packages/
├── ProjectSettings/
├── Docs/
│   └── Fly_Away_Design_Document.pdf
└── README.md
```

## 🚀 Run the Project in Unity

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/Fly-Away.git
   ```
2. Open **Unity Hub** → **Add** → select the cloned folder.
3. Open it with the Unity version listed in `ProjectSettings/ProjectVersion.txt`.
4. Open the `MainMenu` scene and press **Play**.

## 📄 Design Document

The full game design document is here: [Fly_Away_Design_Document.pdf](Docs/Fly_Away_Design_Document.pdf)

## 🗺️ Roadmap

- [ ] Power-up objects for bonus points
- [ ] High score board
- [ ] Sound effects

## 👤 Author

**S. Sriram**
- GitHub: [@YOUR-USERNAME](https://github.com/YOUR-USERNAME)
- Contact / portfolio: ADD-LINK-HERE
