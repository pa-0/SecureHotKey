# Secure Hot Key

## Overview
- This app was created for a particular bank's online system for automatic password input (to achieve fast access by the bank's cashier).
- You can assign the content, e.g., passwords, to the `F8`/`F9` function keys -- just press the hotkey to input the content automatically.
- Supports Internet Explorer password input for online banking, non-program events, and driver-level keyboard control.

## Function
- `F8`/`F9` hotkeys
- Automatic carriage returns
- Support for all input fields (games, IE password controls, etc.)

## System Requirements:
- Windows (x86/x64) (tested under Windows7 64-bit Professional)
- Visual Studio 2015

## Installation Steps
- Download Interception
- Download and run “command line installer”
- To run successfully, `interception.dll` must reside in the same folder as the app
- install-interception /install
- Reboot

# Build steps
- Copy the library/XXX/interception.dll of the interception link library to the same directory as the application execution, XXX: for the corresponding platform (x64/x86), please select by system version.
- Compile using Visual Studio

## Known Issues
- The shortcut is implemented by standard registration methods, and some software will be invalid without using the `SetWindowsHookEx` method and will directly ignore the Hooks of other applications when working)
- In order for Interception to function correctly, the physical keyboard must be manually triggered <ins><strong>at least once</strong></ins> in advance to send the keyboard message correctly, and it only needs to be triggered once

## License
- Secure Hotkey: MIT License 
- Interception carries with it a dual Commercial (Paid) / Personal (Free) License
