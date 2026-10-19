Hood Warfare 2 — F6 Mod Menu
An experimental Lua mod for Hood Warfare 2, powered by UE4SS. It adds a native in-game menu with aim assistance, box ESP, visual settings, and local gameplay controls.
Features
- Head-only aim assistance: smooth aiming, sticky target lock, adjustable acquisition angle, distance, and activation controls.
- Box ESP: character outlines, off-screen markers, adjustable range and thickness, and visible-only mode.
- Dead-character filtering: shared by aim assistance and ESP.
- Visual controls: center crosshair, camera FOV, and status HUD toggle.
- Local gameplay controls: walk speed, flight, jump height, gravity, collision, invulnerability, world speed, and AI freeze.
- Position tools: save and return to a position within the current level.
Installation — SteamRIP Folder Layout
For an extracted SteamRIP copy, find the folder containing HW2.exe. Install the mod beside the shipping executable, at:
Hood Warfare 2/
└── HW2/
    └── Binaries/
        └── Win64/
            └── HW2-HoodWarfare2-Win64-Shipping.exe
1. Download a compatible experimental build from the official UE4SS releases. This mod was developed using v3.0.1-1181-g83330635.
2. Extract its dwmapi.dll and ue4ss folder into that Win64 folder.
3. Create this mod directory:
Win64/ue4ss/Mods/HW2CheatMenu/Scripts/
4. Copy these files from this repository into Scripts:
main.lua
MenuView.lua
BoxESP.lua
TargetLife.lua
5. Add this line to ue4ss/Mods/mods.txt, preserving existing entries:
HW2CheatMenu : 1
6. Launch the game normally using HW2.exe.
Controls
Key	Action
F6	Open or close menu
Tab	Switch category
Up / Down	Select or scroll options
Left / Right / Enter	Change or activate an option


Aim assistance uses right mouse by default. Flight controls are WASD, Space to rise, Left Ctrl to descend, and Left Shift to boost.
Known Limitations
This is an experimental project. Regression simulations pass, but full gameplay verification remains incomplete.
- Flight and movement changes require local/server authority; they do not work reliably when joining a remote server.
- ESP can show teammates. Reliable enemy-only filtering is not included in the current revision.
- Custom damage systems may ignore invulnerability.
- Head targeting requires a recognized head socket.
- Game updates may break compatibility.
Uninstall
Close the game and remove the HW2CheatMenu folder and its entry in mods.txt.
