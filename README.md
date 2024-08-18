# Personalized-Letter-Generator
This Python script automates the process of personalizing letters by replacing a placeholder in a template letter with names from a list. It reads the names from a text file and the letter template from another file, then generates a personalized letter for each name, saving them as separate .docx files.

# Project Structure
├── input
│   ├── Names
│   │   └── invited_names.txt
│   └── letters
│       └── starting_letter.txt
├── output
│   └── ReadyToSend
│       └── letter_for_[name].docx
└── letter_generator.py
input/Names/invited_names.txt: A text file containing a list of names, each on a new line.
input/letters/starting_letter.txt: The template letter with a placeholder [name] where the names will be inserted.
output/ReadyToSend/: Directory where the personalized .docx files will be saved
# How It Works
1)Read the Names: The script reads all the names from the invited_names.txt file.
2)Read the Template Letter: The template letter is loaded from starting_letter.txt.
3)Generate Personalized Letters: For each name in the list, the script replaces the [name] placeholder in the template letter with the actual name.
4)Save the Letters: Each personalized letter is saved in the output/ReadyToSend/ directory with the format letter_for_[name].docx.
# How to Run the Script
Ensure File Structure: Make sure the files invited_names.txt and starting_letter.txt are placed in the correct directories as shown in the project structure.

Execute the Script: Run the script letter_generator.py using Python:
python letter_generator.py
Check the Output: The personalized letters will be saved in the output/ReadyToSend/ directory.
# Example
# If invited_names.txt contains:
Alice
Bob
Charlie
# And starting_letter.txt contains:
Dear [name],

You are invited to our annual event.

Sincerely,
Event Organizer
# the script will generate:

letter_for_Alice.docx
letter_for_Bob.docx
letter_for_Charlie.docx
Each file will have the [name] replaced with the respective name.
# Requirements
Python 3.x
# License
This project is licensed under the MIT License. See the LICENSE file for details.
