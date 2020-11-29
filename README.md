# YahtzeeCoCo

The classic five dice game written in Extended Color BASIC to run on a TRS-80 Color Computer (emulator on Windows) using only a keyboard.

## Getting Started

If you had a Color Computer back in the day and ventured into writing your own games, this will feel familiar.  Either way you will likely need to reference the [Getting Started With Extended Color BASIC](https://colorcomputerarchive.com/repo/Documents/Manuals/Hardware/Getting%20Started%20With%20Extended%20Color%20Basic%20(Tandy).pdf) user manual along the way.

### Prerequisites

Install the latest Virtual Color Computer 3 Emulator from the [VCCE](https://github.com/VCCE/VCC/releases) repository. Version 2.1.0b and beyond allow you to paste code into the console as though you typed it.

### Installing

The default configuration for the emulator works well, although you will likely want to change the keyboard mapping to Natural matching modern keyboard layouts.

## Running a test

Caps Lock should be on while typing in the CoCo emulator window (an SN – syntax error will display if not), but if you turn it off (Shift-Caps to avoid characters sent) **before** pasting, lowercase letters are persisted with a black background.

### Pasting in the code

To examine and modify the logic, copy the entire contents of the .bas text file and select Edit > Paste BASIC Code (with NEW) > Yes. This will scroll through all the lines for a while and then just pause at the end with no prompt. Be aware that pasting large amounts of text cannot be canceled, even with a hard reset, so be patient or restart the entire emulator.

### Loading from tape

An alternative, somewhat faster, way to load the program is to select Configuration > Config > Tape > Browse > *select the .cas file in the Tape directory* > type CLOAD (Enter) in the terminal > Play in the Vcc Options popup. A single character (usually F) will toggle in the upper left of the emulator while loading as the Counter increments on the config screen. Once OK returns a cursor, type LIST 0-100 (if you exclude the line range, prepare to wait for the entire codebase) to verify the program is ready.

## Deployment

Once the code is loaded, type RUN to view the splash screen.  The ready to roll prompt is expecting a Y or YES response. From there gameplay proceeds with responses primarily consisting of menu number choices. Zero or just Enter indicates a non-response and on the scorecard page requires selecting which item to “scratch off” with no points.

## Built With

* [TRS-80 Color Computer (CoCo)]( http://www.trs-80.com/wordpress/trs-80-computer-line/coco/) - Original hardware used to write the program one line at a time
* [Extended Color BASIC]( https://en.wikipedia.org/wiki/Extended_Color_BASIC) - Interpreter for the Radio Shack/Tandy TRS-80 Color Computer

### Additional documentation

There is an emulator help file link installed in the "C:\ProgramData\Microsoft\Windows\Start Menu\Programs\VCC 2.1.0b Coco 3\Coco Manuals\Welcome to VCC 210b.pdf.lnk" directory. Refer to this for Windows specific implementation.
