# MidiLang
An esoteric programming language based on midi sequences.
<br>Also the first language whose code can be actually heard.

## How to use
Download every file and open the `MidiLangCompiler.exe` executable, you should see a new console window open.
<br>Before being able to compile your *amazing* midi files, you'll need to calibrate your note offset.
<br>Since most DAWs don't map their piano roll notes to the standard layout (C4 = 60), the program needs to calculate the offset. Simply follow the instructions written in the console.
<br>If you don't see the "NOTE OFFSET CALIBRATION" text, you're good to compile your programs and brag about how good of a *hacker* you are.
<br>(You can change the offset in the automatically generated `calibration` file)
<br>PS: if you select another file after compiling one, type `r` to compile the new one. I don't know why, but that's the only way it works.

## Instructions
In this language, instructions correspond to notes, placeable in a piano roll.
<br>Here are all the notes you can use:
- `C4`: move pointer to next cell
- `D4`: move pointer to previous cell
- `E4`: add 1 to current cell
- `F4`: subtract 1 to current cell
- `G4`: write cell content to console
- `A4`: read user input
- `B4`: start loop, repeats any instruction inside until cell is 0
- `C5`: end loop
- `C#5`: move cell content to next cell
- `D5`: converts next note to ascii character
- `D#5`: move cell content to previous cell
- `E5`: add two previous cells
- `F5`: subtract two previous cells
<br>PS: note length, BPM, time signature, rhythm and swing do not affect the program's execution: only the order does

## Help
If you type "help" in the console, a file opens displaying the Note-To-Character map, useful when using the `D5` instruction.

## That's it
Have fun!
