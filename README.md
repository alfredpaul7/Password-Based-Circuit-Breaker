
# Password-Based Circuit Breaker

This repository contains the code and documentation for a **Password-Based Circuit Breaker** system. The system allows users to open or close a circuit connection by entering a correct password via a keypad. This project is ideal for controlling critical electrical machines or components, adding an extra layer of security.

## Features

- **Password Authentication**: The circuit will only open or close if the correct password is entered.
- **Security**: Prevents unauthorized access to critical machines or electrical systems.
- **Control**: Switch electrical devices (e.g., bulbs, fans) ON or OFF using a password-based system.
- **User Interface**: Easy-to-use keypad and an LCD display to show feedback on password input and system status.

## Technologies and Components Used

- **C++ Programming**: The logic behind password verification and circuit control is implemented in C++.
- **Arduino IDE**: Used for coding and uploading the program to the microcontroller.
- **Microcontroller (Arduino)**: Acts as the brain of the circuit breaker system, processing inputs and controlling the relay.
- **Relay Module**: Switches the circuit on or off based on the microcontroller's instructions.
- **Keypad**: Used for inputting the password.
- **LCD Display**: Provides feedback to the user about the password input and system status.
- **Power Source**: Supplies power to the microcontroller and relay.
- **Output Device**: The device being controlled (e.g., bulb, fan, etc.).

## How It Works

1. **Password Input**: The user enters a password using the keypad.
2. **Password Verification**: The system checks the entered password against the stored password.
   - If the password is correct, the circuit is opened or closed depending on its current state.
   - If the password is incorrect, the circuit remains unchanged and a warning is displayed.
3. **LCD Feedback**: The LCD display shows the status of the system (e.g., "Access Granted" or "Incorrect Password").
4. **Relay Activation**: The relay switches the circuit ON or OFF based on password validation.

## Components Required

- **Arduino Microcontroller** (e.g., Arduino UNO)
- **4x4 Keypad**
- **16x2 LCD Display**
- **Relay Module**
- **Power Source**
- **Output Device** (e.g., light bulb, fan)
- **Connecting Wires**

## Code Overview

- **Setup**: Initializes the microcontroller, LCD, and keypad.
- **Loop**: Continuously checks for keypad input, validates the password, and controls the relay.
- **Password Logic**: The system compares user input with a predefined password and provides feedback through the LCD.
- **Relay Control**: Opens or closes the circuit based on the password input.

## Usage

1. **Connect the Components**: Wire the keypad, LCD display, relay, and output device as per the schematic.
2. **Upload the Code**: Use Arduino IDE to upload the code to the microcontroller.
3. **Power the System**: Connect the power source to the circuit.
4. **Enter Password**: Use the keypad to enter the password and control the connected device.
   - Default password can be modified in the code.

## Example Circuit Diagram

- **Keypad Input**: Input password through the keypad.
- **Microcontroller**: Processes the password and controls the relay.
- **Relay**: Switches the output device ON or OFF.

![Project photo](https://photos.app.goo.gl/CFK34ArqxaqiUwXK7)


