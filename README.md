# WPM_python_project
Speed Typing Test (Python + Curses)

A terminal-based speed typing test built in Python using the curses library.
The program measures your Words Per Minute (WPM) as you type a random sentence from a text file.

Features

Displays a random line of text from text.txt to type.

Real-time WPM calculation.

Highlights:

✅ Correctly typed characters in green

❌ Incorrect characters in red

Supports backspace to correct mistakes.

Ends automatically when you finish typing the target text.

Press Esc anytime to quit.

##Requirements

Python 3.7+

A terminal that supports curses (Linux/macOS work by default.
On Windows, you may need to install windows-curses
):

pip install windows-curses

Installation

Clone the repository:

git clone <your-repo-url>
cd <repo-folder>


Make sure you have a text.txt file in the same folder containing sample sentences, one per line. Example:

The quick brown fox jumps over the lazy dog.
Coding is fun when you practice every day.
Python makes programming enjoyable.

Usage

Run the program:

python typing_test.py


You’ll see:

Welcome to speed typing test...
Press any key to begin!..


Then a random sentence will appear. Start typing!

Your current WPM will be shown live.

Green = correct, Red = incorrect.

Press Esc anytime to exit.

At the end, you’ll see:

You completed the text! Final WPM: 45

Code Overview

start_screen → Welcome screen.

load_text → Reads a random line from text.txt.

display_text → Prints target vs. typed characters with colors.

wpm_test → Main typing loop; calculates WPM.

main → Handles replay + exit logic.
