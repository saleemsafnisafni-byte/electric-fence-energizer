Electric Fence Energizer
Project Overview

The Electric Fence Energizer is an embedded electronics project designed to generate high-voltage pulses to control livestock or secure perimeters. The project uses an ATmega328P microcontroller to drive an inverter circuit for MOSFETs and manage an integrated alarm system.

The device can accept either 12V DC or 220V AC as input and provides an output of 1000V with 100mA current at 2 pulses per second. It is designed to be safe for livestock while providing a reliable electric barrier.

Features

Microcontroller-based design using ATmega328P

MOSFET-based inverter for high-voltage pulse generation

Dual input support: 12V DC or 220V AC

Output: 1000V, 100mA, 2 pulses/sec

Integrated alarm system for monitoring fence activity

Pulse timing controlled via firmware for consistent output

Compact and robust design suitable for outdoor environments

Components Used

Microcontroller: ATmega328P

Power Supply: 12V DC or 220V AC input

Inverter Circuit: MOSFETs for switching high-voltage output

Output: High-voltage transformer/module

Alarm System: Buzzer or indicator LED

Miscellaneous: Resistors, capacitors, PCB, connectors, and protective casing

Circuit Description

Input Section:

Converts AC to DC if using 220V AC input.

Provides regulated 12V DC for the ATmega328P and control circuits.

Microcontroller Control:

ATmega328P generates PWM signals for MOSFET switching.

Controls timing for high-voltage pulse generation (2 pulses/sec).

Monitors the output and triggers the alarm system in case of fault or short.

Inverter Section:

MOSFETs amplify the control signals from ATmega328P.

Drives the high-voltage transformer/module to produce 1000V pulses.

Alarm System:

Monitors fence integrity.

Provides visual/audio alert when fence is touched or shorted.

Working Principle

The ATmega328P microcontroller reads the system inputs and generates pulse-width signals to control the MOSFETs.

MOSFETs switch the transformer primary, producing high-voltage pulses on the output.

Each pulse lasts a few milliseconds, repeated 2 times per second.

The alarm system is triggered if irregular conditions are detected, ensuring safety and monitoring.

Safety Precautions

Output voltage is high (1000V), handle with extreme care.

Do not touch the output terminals when the system is powered.

Ensure the circuit is properly insulated and housed.

Use appropriate fuses and protection circuits to prevent accidents.

Installation & Usage

Connect the input power (12V DC or 220V AC).

Power on the system; the microcontroller will start generating pulses.

Connect the fence wire to the output terminals.

Monitor the alarm system for any irregularities.

Firmware

Developed using Arduino IDE / Atmega328P C code.

Handles pulse generation and alarm monitoring.

Configurable pulse frequency and duration in code.


Demo Video

Watch the project in action :
https://drive.google.com/file/d/1fwy3NhG2aM_A7V3LZK2k0VW2aplA58Xk/view?usp=drive_link, @SafniSaleemsafni
