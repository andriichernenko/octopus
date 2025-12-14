# Octopus for Xcode

Octopus for Xcode is a [source editor extension](https://developer.apple.com/documentation/xcodekit#overview) that adds a several convenience features.

## Features

### Expand/Shrink selection

- Expand selection selects the nearest scope that contains the current selection. 
- Shrink selection goes back to the previous selection. 

https://github.com/user-attachments/assets/d0897aab-ff24-46f3-b248-2d829018a207

### Select next/previous/all occurrences

**Select next/previous** command finds the next/previous instance of the the selected text in the current file and adds a selection for it. Unlike a similar feature built into Xcode, it allows you to backtrack if you end up selecting too many occurrences. 

**Select all occurrences** selects all occurrences at once.

https://github.com/user-attachments/assets/02d3d19e-f9fb-41fb-b192-2ea70f3a1611

### Format with SwiftFormat

This feature provides better Xcode integration with [nicklockwood/SwiftFormat](https://github.com/nicklockwood/SwiftFormat).

It combines the **benefits of an Xcode extension**, like:
- formatting instantly by pressing a shortcut,
- keeping the undo history for the formatted file,
- formatting only selected code

with the benefits of **formatting via command line**: 
- automatically using the correct project-specific and folder-specific configs,
- taking `.swift-version` into account.

## Requirements
- Xcode 16+
- Swift code (Objective-C and other languages are not supported).

Octopus may work in Xcode versions as old as 8, but it has not been tested with anything older than Xcode 16.

## Privacy policy
Octopus for Xcode doesn't collect or send any information, even analytics. Nothing ever leaves your computer.

## Getting started
1. Download _Octopus.zip_ from [the Releases page](https://github.com/andriichernenko/octopus/releases).
2. Unzip the file, move _Octopus.app_ to the _Applications_ folder.
3. Launch _Octopus.app_. This will automatically add a login item.
4. On launch, Octopus will request accessibility permissions. Press the _Open System Settings_ button:

   <img width="573" alt="accessibility permission dialog" src="https://github.com/user-attachments/assets/8fbcf70f-ea2f-4e93-a96b-dbe7f8657d0d" />

   Alternatively, go to _Settings > Privacy & Security > Accessibility_

   Enable the toggle for Octopus:

   <img width="835" alt="accessibility permission page" src="https://github.com/user-attachments/assets/022a75dc-5e19-4e6b-9aca-b733dfb47d3d" />

5. Open _Settings > General > Login Settings & Extensions_. Scroll down to the _App Background Activity_ section and make sure the item for Octopus is enabled:

   <img width="835" alt="login item app background activity" src="https://github.com/user-attachments/assets/8226915c-de86-4d50-86a7-c6870ffb0ce0" />

   While on the same page, scroll down to the _Extensions_ section and select _By Category_. Then find the _Xcode Source Editor_ item and press the "i" button next to it:

   <img width="835" alt="login item extensions" src="https://github.com/user-attachments/assets/39e9d2e7-a98b-4630-adec-607749b86d94" />

   In the dialog that opens, make sure the Octopus extension is enabled:

   <img width="835" alt="source editor-extension" src="https://github.com/user-attachments/assets/d0d264f4-9855-4594-9689-d81822e5d2cb" />

6. Start Xcode. When you open a project, you should see the Octopus submenu in the Editor menu:

   <img width="573" src="https://github.com/user-attachments/assets/4d94d8af-c700-4830-ad0e-37338fca8e57" />

7. (Optional) Assign shortcuts for Octopus commands in Xcode settings (no shortcuts are assigned by default).

## Installing updates

1. Download the new version of Octopus from [the Releases page](https://github.com/andriichernenko/octopus/releases).
2. Quit Xcode and the Octopus app using the menu bar item.
3. Replace _Octopus.app_ in the _Applications_ folder with the new version.
4. Start Xcode and Octopus.
