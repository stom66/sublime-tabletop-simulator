# Tabletop Simulator for Sublime Text 3
This plugin implements the [external editor API][api] provided by Tabletop
Simulator to allow use of Sublime Text 3 as the Lua editor.

## Installation
Create the appropriate folder and put the contents of the repository in it.

 -  Windows: `%APPDATA%\Sublime Text 3\Packages\Tabletop Simulator\`
 -  Linux: `~/.config/sublime-text-3/Packages/Tabletop Simulator/`
 -  OS X: `~/Library/Application Support/Sublime Text 3/Packages/Tabletop
    Simulator/`

## Usage
 1. Start the server: `Tools -> Tabletop Simulator -> Start Server`
 2. Launch Tabletop Simulator and load a save
 3. Either open all existing scripts (`Tools -> Tabletop Simulator -> Get
    Scripts`) or open a particular object's script by right-clicking it in
    Tabletop Simulator and choosing `Scripting -> Lua editor`
 4. Send the edited scripts back to Tabletop Simulator: `Tools -> Tabletop
    Simulator -> Send Scripts`

## Notes
 -  The server required to interact with Tabletop Simulator is not started
    by default. To start it, follow step 1 under Usage.

    To start it by default, uncomment line 83 in Tabletop Simulator.py.
    
 -  The changes made by stom to allow editing XML scripts are not done in the best way possible (I'm quite happy to admit this) and could probably benefit from refactoring by someone with a proficiency in Python.

[api]: http://berserk-games.com/knowledgebase/external-editor-api/
