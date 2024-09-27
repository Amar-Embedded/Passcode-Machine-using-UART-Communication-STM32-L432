# Passcode-Machine-using-UART-Communication-STM32-L432

Overview
This project implements a passcode verification system using UART communication with the STM32 L432KC microcontroller. When the user enters the correct passcode, a green LED blinks, and the message "Correct Passcode" is displayed in the terminal on PuTTY. Additionally, a hint feature is included to guide the user in case they forget the passcode.

Objective

To simulate a basic passcode machine where user input is verified over UART, and feedback is provided through both an LED and a serial terminal.
Implement UART communication to handle input and output between the STM32 microcontroller and a PC terminal (PuTTY).
Add a hint option to help users with passcode recovery.

Hardware Used

Microcontroller: STM32 L432KC Nucleo-32 board.
LED: A green LED connected to a GPIO pin for passcode success indication and a red LED for wrong passcode indication.
UART Communication: Used for sending and receiving data from the terminal (PuTTY).
Terminal Software: PuTTY for user interaction.

How it Works

User Input via UART: The user inputs the passcode through a serial terminal (PuTTY) connected to the STM32 microcontroller via UART.
Passcode Verification: The input passcode is checked against the predefined correct passcode stored in the microcontroller's memory.
Green LED Feedback: If the entered passcode is correct, the green LED blinks to indicate success, and the message "Correct Passcode" is displayed on the PuTTY terminal.
Hint Option: If the user forgets the passcode, they can request a hint by entering a special command, and the hint is displayed on PuTTY.
Error Handling: If the passcode is incorrect, the terminal displays "Incorrect Passcode," and RED LED will glow.
