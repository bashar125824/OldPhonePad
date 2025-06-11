# Old Phone Pad Solution

This repository contains a C# implementation of the Old Phone Pad coding challenge.

## Problem Description

The challenge involves converting input from an old phone keypad into the correct output string. The keypad has:
- Numbers 0-9 with associated letters
- A backspace key (*)
- A send button (#)

Pressing a button multiple times cycles through its letters. A space indicates a pause between same-button presses.

## Solution Features

- Handles multi-tap input for each button
- Processes spaces as pauses between same-button characters
- Implements backspace functionality (*)
- Properly handles the send command (#)
- Includes comprehensive unit tests
- Follows clean code principles

## Usage

```csharp
// Using the instance method
var converter = new OldPhonePadConverter();
string result = converter.Convert("4433555 555666#"); // Returns "HELLO"

// Using the static method (matches challenge requirements)
string result = OldPhonePadConverter.OldPhonePad("227*#"); // Returns "B"
