# A Guide for NVIDIA Roblox Shaders

[Thanks to Toast RBX for creating the original tutorial!](https://www.youtube.com/watch?v=zhSWJnxKIlg)

## Requirements

1. A PC
2. An NVIDIA GPU
3. [NVIDIA Profile Inspector](https://github.com/Orbmu2k/nvidiaProfileInspector)
4. [GeForce Experience \(especially ShadowPlay\)](https://www.nvidia.com/en-us/geforce/geforce-experience/)
5. [Newest NVIDIA **Game Ready** Drivers](https://www.nvidia.com/download/find.aspx)
6. [Bloxstrap](https://github.com/pizzaboxer/bloxstrap)

Install all of those before continuing with this guide.

## Guide

1. Open NVIDIA Profile Inspector
2. Go to the "Other" section and turn "Ansel flags for enabled applications" to `0x00000001 ANSEL_ALLOWLISTED_ALLOWED`, "Ansel - Enabled" to `On`, and "NVIDIA Predefined Ansel Usage" to `0x00000001 ANSEL_ALLOW_ALLOWED`

![image](https://github.com/catb0x/Roblox-Shaders-Guide/assets/77354428/deb9405d-b670-4463-9e2e-15cd67bdf61e)

3. Download this repo, and go to `C:\Program Files\NVIDIA Corporation`
4. a. If you see a folder named `Ansel`, delete all shaders in it and copy the files in the `Effects` folder from this repo to the `Ansel` folder
   
   b. If you don't see it, create a new folder with that name, and copy the files in the `Effects` folder from this repo to the folder you just made
5. Go into GeForce Experience, go to Settings, and enable "in-game overlay"
6. If Bloxstrap version is **under 2.6.0**:

   a. If you are logged into GitHub, [download the official Bloxstrap.exe modification](https://github.com/pizzaboxer/bloxstrap/suites/17761020689/artifacts/1017388973), extract it, and copy-paste the `Bloxstrap.exe` file into the Bloxstrap directory

   b. If you aren't, go to the `BloxstrapEXE` file in the repo and and copy-paste the `Bloxstrap.exe` file into the Bloxstrap directory (SHA256 Hash: `42FFCEFDB485BC6833F2DB4209CB6433BAB0C59DEBB2A1FF77475E06AEBA5BAD`, compare it with the hash of the Bloxstrap.exe from the GitHub link if you want.)

   After that, go to `%LocalAppData%\Bloxstrap` and paste and replace the `Bloxstrap.exe` file, and disable automatic updates in the Behaviour tab.

   If Bloxstrap version is (over) **2.6.0**:

   Change the Roblox executable name to `eurotrucks.exe` **in the Bloxstrap menu**
   
You don't need to do anything from this point, just join Roblox, press <kbd>Alt</kbd> + <kbd>F3</kbd> (to open Game Filter menu) or <kbd>Alt</kbd> + <kbd>Z</kbd> (to open ShadowPlay Menu, click on Game Filter in that menu) to apply any filters you want!

## Troubleshooting

### Error: "A supported game is required to use this feature"

1. **Make sure Bloxstrap is installing Roblox as `eurotrucks2.exe` instead of `RobloxPlayerBeta.exe`**
2. Restart, update Roblox, update your Drivers, reinstall GeForce Experience, or/and reinstall drivers and repeat steps 1 to 5

### Game Filter menu doesn't open

1. Disable and enable the overlay or/and restart. If that doesn't work, update your Drivers, reinstall GeForce Experience, or/and reinstall drivers and repeat steps 1 to 5

### SSR breaks in fullscreen mode

1. Enable fullscreen in the Roblox menu
2. Leave and rejoin
3. Continue using fullscreen or disable fullscreen and enable exclusive fullscreen with <kbd>Alt</kbd> + <kbd>Enter</kbd>

## Presets

### Creating a preset

1. Download the [Ansel Configuration Utility](https://international-gfe.download.nvidia.com/GFE/GFEClient/NVCameraConfiguration/v1.0/NVCameraConfiguration_v1.0.0.6.zip)
2. Open it and enable "Save Preset with Shot"

![image](https://github.com/catb0x/Roblox-Shaders-Guide/assets/77354428/ab38024d-5fc4-437b-871e-8209ebc77957)


4. Launch Roblox
5. Press <kbd>Alt</kbd> + <kbd>F2</kbd> to open the Ansel Photo mode overlay
6. Add the filters you want in the preset and take a photo
7. Exit the overlay and press <kbd>Alt</kbd> + <kbd>Z</kbd> to open the ShadowPlay menu
8. Click on "Gallery", click on the photo you just made, and click "Open File Location"
9. (optional) Rename the `.ini` file to anything
10. Copy the `.ini` file and go to `C:\Program Files\NVIDIA Corporation\Ansel\`
11. a. If you see the `Custom` folder, go into it and paste the `.ini`

    b. If you don't, create it, go into it, and paste the `.ini`

### Using a preset

1. Open Roblox and open the Game Filter menu
2. Select one of the three loadouts, search for the name of the `.ini` file, and press on it

You should now see the preset being used as a filter.
