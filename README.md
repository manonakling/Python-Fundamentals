# Python-Fundamentals
[README.md](https://github.com/user-attachments/files/33976683/README.md)
#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Mon Oct 26 12:03:05 2026

@author: manonkling
"""

# -------------------------------------------------------
# Module 2 Assignment 1
# Program: Celsius to Fahrenheit Temperature Converter
#
# Description:
# This program asks the user to enter a temperature
# in Celsius and converts it to Fahrenheit.
#
# It demonstrates input validation, string manipulation,
# mathematical calculations, and exception handling.
# -------------------------------------------------------

print("Welcome to the Temperature Converter!")

while True:
    user_input = input("Enter a temperature in Celsius: ").strip()

    if user_input == "":
        print("Error: Please enter a temperature.")
        continue

    try:
        Celsius = float(user_input)

        Fahrenheit = (Celsius * 9 / 5) + 32

        print("\nTemperature Conversion Results")
        print("------------------------------")
        print(f"Celsius: {Celsius:.2f}°C")
        print(f"Fahrenheit: {Fahrenheit:.2f}°F")

        message = "temperature conversion successful"

        print(message.upper())
        print(f"Number of words in message: {len(message.split())}")

        break

    except ValueError:
        print("Invalid input! Please enter a number.")

print("\nThank you for using the Temperature Converter!")
