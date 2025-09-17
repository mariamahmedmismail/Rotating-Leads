Rotating LEDs Project
📌 Overview

This project demonstrates LED matrix control using an Arduino and C++ programming.
It displays the initials of the project team members on an 8x5 LED matrix by turning LEDs on and off row by row in a timed sequence, creating the appearance of letters scrolling or rotating across the matrix.

🛠 Features

Displays letters A, G, H, I, M and a blank _ character using a binary representation.

Allows row-by-row control of LEDs to display letters sequentially.

Configurable space between letters and delay time for smooth visual effects.

Prints the initials of all team members in sequence with small pauses for readability.

🧠 How It Works

Letter Representation

Each letter is represented as an integer array with 40 binary values (1 = LED ON, 0 = LED OFF).

The project defines arrays for A, G, H, I, M, _ (underscore for space).

Functionality

The printletter() function loops through each row of the letter, writing values to the LED pins and adding a small delay for persistence.

After each letter, it clears the LEDs and waits for a configurable delay to create a space between letters.

Main Loop

The loop() function calls printletter() in a specific sequence to display:
M H _ M I _ G M A (representing the team members' initials).

📂 File Structure
Rotating-LEDs-Project/
│
├── Rotating_LEDs.ino   # Main Arduino sketch (your provided code)
└── README.md           # This file

⚙️ Configuration

You can adjust the following variables in setup() to customize display behavior:

space_between_letters → Controls the gap between letters.

dotTime → Controls how long each row stays lit (affects brightness/speed).


🖥 Tech Stack

Language: C++ (Arduino)

Hardware: Arduino + 8x5 LED Matrix

Concepts Used: Arrays, Pointers, Loops, Digital I/O, Delays
