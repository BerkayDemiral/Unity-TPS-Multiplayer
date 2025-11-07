# 🚀 Unity & Netcode TPS Multiplayer

> A portfolio-focused, technical showcase of a multiplayer TPS (Third-Person Shooter) game built with **Unity** and **Netcode for GameObjects**. This project serves as a strong foundation, demonstrating the core systems required for a production-ready online game.

---

## 🚧 Project Status

This project is a **completed technical prototype** developed as a portfolio piece. The primary goal is to showcase proficiency in **network programming**, **gameplay systems integration**, and **Unity engine capabilities**.

The project's current state demonstrates that the targeted core systems are complete and present a working demo.

---

## 🛠️ Implemented Features

### 🎮 Gameplay Mechanics
* **Core TPS Controller:** Movement, animation (blendtrees), and camera control.
* **Advanced Aim Down Sights (ADS):** Dynamic aiming using rig constraints and camera zoom.
* **Weapon System:** Recoil management, bullet trajectory, and muzzle flash effects.
* **Weapon Switching:** Ability to switch between weapons in the player's inventory.
* **Reloading:** Reload animations managed with a blendtree.
* **Physics-Based Ragdoll:** Physics-driven reactions for character death or heavy impacts.
* **UI Systems:** Dynamic crosshair for aiming, a lobby interface, and a full inventory management interface.

### 🌐 Online Systems (Networking)
* **Netcode Integration:** The core multiplayer foundation of the project.
* **Authentication:** Basic player authentication and session management.
* **Lobby & Matchmaking:** Allowing players to join sessions and find games.
* **Character Selection:** Player selection and basic customization in the lobby.
* **Networked Inventory:** A host-authoritative, fully synchronized inventory and item management system.
* **Networked Equipment System:** Synchronizing the character's equipped items (weapons, etc.) across the network.
* **Character Synchronization:** Synchronization of movement, animations, and character physics over the network.
* **Networked Interactions:** Synchronizing weapon handling, shooting, and inputs across all clients.
* **Networked Item Pickup:** Picking up items from the world with UI prompts and network sync.

---

## 💻 Tech Stack
* **Game Engine:** Unity
* **Programming Language:** C#
* **Networking:** Unity Netcode for GameObjects
* **Backend:** Standalone C# Console Application (Master Server)
* **Database:** Sqlite

---

## 📁 Setup and Running

This project consists of two separate parts: The **Backend Server (C#)** and the **Game Client (Unity)**.
To test the project, the *server must be running first*, followed by the game.

### Step 1: Start the Server (Backend)

1.  Navigate to the `[Server Manager]/` directory in the project files.
2.  Open `Realtime Networking Server.sln` with Visual Studio.
3.  Run the project using the "Start" (▶) button in Visual Studio.
4.  A terminal/console window will open and display a message like "Server started...". **Do not close this window.**

### Step 2: Start the Game (Unity Client)

1.  While the backend server is running, open the main game project (Unity).
2.  Open the `Lobby` (or main menu) scene in the Unity editor and press 'Play'.
3.  The game will automatically connect to the running server, and the login screen will appear.

---

## 💡 Potential Improvements (Future Vision)

Potential next steps that could be built upon this project's foundation include:

* **Dedicated Server Support:** Migrating the architecture from host-dependency to a dedicated server structure.
* **Persistence:** Connecting the inventory and player profiles to a database (e.g., Firebase, PlayFab).
* **Expanded Game Loop:** Adding game modes with win conditions, such as Team Deathmatch (TDM).
* **Content Polish:** Polishing the game with new weapons, maps, and sound effects.

---

## 👤 Developer

**Berkay Demiral**  
GitHub: [@BerkayDemiral](https://github.com/BerkayDemiral)

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## 🗒️ Note

This project serves as an excellent reference for **Unity network architecture**. The systems (especially authentication, lobby, and the networked inventory) are designed to be decoupled and can be studied or adapted for other multiplayer projects.

---

## 🎓 Project Origin & Acknowledgments

This project is a complete implementation of the comprehensive multiplayer tutorial series created by **Developers Hub** ([@developershub_org](https://www.youtube.com/@developershub_org)).

**Tutorial Playlist:** [YouTube](https://youtube.com/playlist?list=PLfLOlXy59QoqaRLD_eSSCb8tSiloOnpt4)

The primary goal of this repository was to study and successfully implement a complex, full-stack multiplayer game. All architecture and code for both the Unity client and the C# Server Manager are based on the methods and assets provided in this tutorial.
