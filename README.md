CHIP-8 Emulator
This repository contains a CHIP-8 emulator written in Rust. The CHIP-8 is a simple, interpreted programming language used in the 1970s for programming video games on early microcomputers. This emulator allows you to run and play classic CHIP-8 games on modern hardware.

Features
CHIP-8 Instruction Set Support: Fully implements the CHIP-8 instruction set, including various opcodes for drawing graphics, handling input, and controlling game logic.
Graphics Rendering: Renders the CHIP-8 graphics on a 64x32 pixel monochrome display.
Keyboard Input: Maps the CHIP-8 hex-based keypad to your keyboard for user input.
Timers: Implements the delay and sound timers for accurate game emulation.
Prerequisites
To build and run this project, you'll need to have the following installed:

Rust (latest stable version)
Cargo
SDL2 (for graphics and input handling)
Installing SDL2
To install SDL2 on your system, follow the instructions for your platform:

Windows: Use the vcpkg package manager to install SDL2.
macOS: Install using Homebrew:
bash
Copy code
brew install sdl2
Linux: Install using your package manager (e.g., apt-get, yum, pacman):
bash
Copy code
sudo apt-get install libsdl2-dev
Getting Started
Clone the repository
bash
Copy code
git clone https://github.com/basit-shafiqq/chip-8-emulator.git
cd chip-8-emulator
Build the project
bash
Copy code
cargo build --release
Run the emulator
bash
Copy code
cargo run --release /path/to/your/chip8/rom.ch8
Replace /path/to/your/chip8/rom.ch8 with the path to a CHIP-8 ROM file you want to load.

Controls
The CHIP-8 system uses a 16-key hexadecimal keypad, which is mapped to your keyboard as follows:

CHIP-8 Key	Keyboard Key
1	1
2	2
3	3
C	4
4	Q
5	W
6	E
D	R
7	A
8	S
9	D
E	F
A	Z
0	X
B	C
F	V
Project Structure
src/main.rs: The main entry point of the emulator where initialization and game loop occur.
src/cpu.rs: Contains the implementation of the CHIP-8 CPU, including opcode handling.
src/display.rs: Handles the rendering of the CHIP-8 display using SDL2.
src/keyboard.rs: Manages keyboard input and maps it to CHIP-8 keys.
src/timer.rs: Implements the delay and sound timers for accurate emulation.
ROMs
This emulator does not include any CHIP-8 ROMs. You can find public domain CHIP-8 ROMs online to test the emulator.

Contributing
Contributions are welcome! If you have any improvements, bug fixes, or suggestions, feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

Feel free to adjust or expand on this README based on your project specifics!






