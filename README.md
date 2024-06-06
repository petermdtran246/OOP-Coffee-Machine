# OOP Coffee Machine
## Overview
This project simulates a coffee machine that offers different coffee options, manages resources, processes payments, and updates reports. It includes four main modules:
- `main.py`
- `money_machine.py`
- `coffee_maker.py`
- `menu.py`

## Files and Modules

### main.py
This is the main driver script that runs the coffee machine. It handles user interactions, processes orders, and calls appropriate methods from other modules.

### money_machine.py
This module handles all monetary transactions. It processes coins, calculates payments, and maintains the profit report.

### coffee_maker.py
This module models the coffee machine itself. It tracks resources, ensures there are enough ingredients for the chosen coffee, and makes the coffee.

### menu.py
This module contains the menu with coffee options, their ingredients, and prices.

## Algorithm
The coffee machine operates as follows:

1. **Initialize the machine**:
    - Create instances of `MoneyMachine`, `CoffeeMaker`, and `Menu`.
    - Set the machine's state to `on`.

2. **Main loop**:
    - While the machine is `on`:
        - Display the menu options to the user and prompt for a choice.
        - If the user chooses `off`, turn off the machine.
        - If the user chooses `report`, print the reports for both the money and the coffee machine.
        - If the user chooses a coffee option:
            - Check if there are enough resources to make the coffee.
            - Process the payment.
            - If payment is successful, make the coffee.
