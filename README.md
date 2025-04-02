# Ricks revenge
 Rick's Revenge - for Hypseus
 ...was an April Fools' prank for 1st April 2025.

 ![image](https://raw.githubusercontent.com/Widge-5/ricks-revenge/main/Screenshot.png)
 
 It posed an interesting challenge as I didn't want people to know it was a prank before trying to run the "game", even though suspicions are rife on that particular day of the year, I wanted to make sure the curious didn't ruin the reveal before time.
 
 Hypseus and Singe have certain limitations that make the disguise difficult.
 
 An `M2V` video and accompanying `OGG` audio files are required for Hypseus to run.  Well, I didn't want the video to be that plainly obvious, so the M2V is just a few frames of pure black screen, and I renamed it to, simply `rick.01`. Anyone who tries to view that file will just see lack screen and nothing more.  The `OGG` is optional, so I just omitted that entirely.  I did need audio however, so an `MP3` at low bitrate (to minimise the file size), renamed `rick.02` did the trick.
 
 Singe scripts are usually easily read in any text editor, and if all it did was just play a video then I'm sure there would be some suspicion.  I could have easily compiled the script into bytecode so it wouldn't be so obvious but I'm sure that would have raised suspicion within the context.  So I converted a short video into an array of greyscale values, pixel by pixel, frame by frame.  This method of storing video is very uneconomical, so I kept the resolution and framerate low and decided to abandon colour so that I only needed to store one grey value instead three colour values per pixel.  The array is stored in a singe script file in plain text as `rick.03`.
 The main script then loops through the array and draws each pixel per frame timed to the correct speed.
 So if someone wanted to work it out it wouldn't have been too difficult to read the script and understand, but it would have just been much easier and more fun to play it.
 
 It was a lot of fun to put together, and I think it entertained a few people.
 

# Rick's Revenge - Installation and Usage Guide

## Introduction
This repository contains **Rick's Revenge**, a fan-made game built for use with the Hypseus Singe emulator. This is a **work-in-progress preview** that I'm eager to show people!

## Requirements
- **Hypseus Singe** (Tested with the current release)
- **Singe Files** (All necessary files are included in this repository)

## Installation
### 1. Download Hypseus Singe
- **Windows Users:** Download the latest version of Hypseus Singe from the official [Hypseus GitHub repository](https://github.com/DirtBagXon/hypseus-singe).
- **Raspberry Pi Users:** Install Hypseus from the RetroPie Setup menu.

### 2. Download the Release ZIP
Download the latest release from the [Releases](https://github.com/Widge-5/ricks-revenge/releases/) page. Extract the ZIP file to obtain a folder named `rick` containing all necessary game files.

### 3. Installation for Windows Users
- Place the `rick` folder inside your `singe/` subfolder in your Hypseus installation directory.
- To start the game, double-click the included `rick's revenge.bat` file.

### 4. Installation for Raspberry Pi Users
- Place the `rick` folder inside your `roms/daphne/` directory.
- Rename the folder to `rick.daphne` to ensure Hypseus recognizes it.
- Restart Emulation Station after placing and renaming the folder.
- Select **Rick** from Emulation Station's Daphne menu to launch the game.

## Running the Game
### Windows
Simply double-click the `rick's revenge.bat` file provided within the `rick` folder.

### Raspberry Pi
Launch the game by selecting **Rick** from Emulation Station's Daphne menu after restarting Emulation Station.

## Getting Help
If you need help, feel free to ask on the [Hypseus Discord server](https://discord.gg/aCt2YPae3T).

## Credits
- **Hypseus Singe** by DirtBagXon
- **Rick's Revenge** by Widge

