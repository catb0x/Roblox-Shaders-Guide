# A Guide for NVIDIA Roblox Shaders

[Thanks to Toast RBX for creating the original tutorial!](https://www.youtube.com/watch?v=zhSWJnxKIlg)

## Requirements

1. A PC
2. An NVIDIA GPU
3. [NVIDIA Profile Inspector](https://github.com/Orbmu2k/nvidiaProfileInspector)
4. [GeForce Experience \(especially ShadowPlay\)](https://www.nvidia.com/en-us/geforce/geforce-experience/)
5. Newest NVIDIA **Game Ready** Drivers
6. [Bloxstrap](https://github.com/pizzaboxer/bloxstrap)

Install all of those before continuing with this guide.

## Guide

1. Open NVIDIA Profile Inspector
2. Go to the "Other" section and turn "Ansel flags for enabled applications" to `0x00000001 ANSEL_ALLOWLISTED_ALLOWED`

![image](https://github.com/catb0x/Roblox-Shaders-Guide/assets/77354428/2a2a0399-e76b-4556-b963-24edb7c024ed)

3. Download this repo, and go to `C:\Program Files\NVIDIA Corporation`
4. a. If you see a folder named `Ansel`, delete all shaders in it and copy the files in the `Effects` folder from this repo to the `Ansel` folder
   
   b. If you don't see it, create a new folder with that name, and copy the files in the `Effects` folder from this repo to the folder you just made
5. Go into GeForce Experience, go to Settings, and enable "in-game overlay"

### SKIP 6 IF BLOXSTRAP IS HIGHER THAN VERSION 2.5.4

6. Go to the `BloxstrapEXE` file in the repo and replace `Bloxstrap.exe` in `%LocalAppData%\Bloxstrap` with the `Bloxstrap.exe` in the `BloxstrapEXE` folder (updates should be auto-disabled but make sure it's disabled in the Bloxstrap menu)
   
   **If Bloxstrap added the function of changing the Roblox executable name, change it to `eurotrucks2.exe`**
   
You don't need to do anything from this point, just join Roblox, press <kbd>Alt</kbd> + <kbd>F3</kbd> (to open Game Filter menu) or <kbd>Alt</kbd> + <kbd>Z</kbd> (to open ShadowPlay Menu, click on Game Filter in that menu) to apply any filters you want!

## Troubleshooting

### Error: "A supported game is required to use this feature"

1. **Make sure Bloxstrap is installing Roblox as `eurotrucks2.exe` instead of `RobloxPlayerBeta.exe`**
2. Disable and enable the overlay, restart, update Roblox, update your Drivers, and if it still breaks, reinstall GeForce Experience and repeat steps 1 to 5
   
