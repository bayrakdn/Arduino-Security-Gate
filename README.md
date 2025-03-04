Arduino Security Gate Project

Overview

This project is an Arduino-based security gate system that uses a keypad to enter a password and a servo motor to unlock the gate. It also includes LED indicators to show the locked and unlocked status.

Components Used

Arduino board

4x4 Keypad

Servo motor

LEDs (Red and Green)

Resistors

Connecting wires

Circuit Connections

Keypad:

Row Pins: 8, 7, 6, 9

Column Pins: 5, 4, 3, 2

Servo Motor:

Signal Pin: 11

LEDs:

Red (Locked): Pin 12

Green (Unlocked): Pin 13

How It Works

The user enters a 3-digit password using the keypad.

If the entered password matches the predefined password (555), the servo motor rotates to unlock the gate.

If the password is incorrect or the user presses * or #, the system resets.

A red LED indicates a locked state, and a green LED indicates an unlocked state.

Code Explanation

The code defines a password (555) and checks user input from the keypad.

If the input matches the password, the servo motor moves to unlock the gate.

If an incorrect key is pressed, the system resets.

The LockedPosition() function handles LED status and servo motor movement.

How to Use

Power the Arduino board.

Enter the password (555) using the keypad.

If the password is correct, the servo motor moves to unlock the gate, and the green LED lights up.

If an incorrect key is pressed or * or # is pressed, the system resets, and the red LED stays on.

Possible Improvements

Implement a function to change the password dynamically.

Add an LCD display for better user interaction.

Include a buzzer for incorrect password attempts.

Use EEPROM to store the password permanently.

License

This project is open-source and free to use for educational purposes.
