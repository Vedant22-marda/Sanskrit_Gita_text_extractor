# Astavakra Gita Verse Extractor



This Python script extracts verses and their corresponding numbers from a DOCX file (`Sanskrit_text_file.docx`). The extracted data is then saved into a JSON file (`verses.json`) on your Desktop.



## Prerequisites



- Python 3.x installed on your system.

- The `python-docx` library installed. You can install it using pip:

  ```bash

  pip install python-docx

The input DOCX file named Sanskrit_text_file.docx should be in the same directory as the Python script (or the path in the script should be updated).

How to Run

Save the Python script as Sanskrit_text_code.ipynb.

Ensure the Sanskrit_text_file.docx is in the same directory as the script, or modify the input_file variable in the script with the correct path if it's elsewhere.

Run the script using a Jupyter Notebook environment or by converting it to a Python script and running it:Bash



jupyter notebook Sanskrit_text_code.ipynb# OR after converting to .py:# python Sanskirt_text_code.py

The extracted verses will be saved in a file named verses.json on your Desktop.

Output Format

The verses.json file contains a JSON array of verse objects, where each object has the following structure:



JSON



[

{

"verse": "First line of the verse\nSecond line of the verse",

"index": "Verse number (e.g., 1.5)"

},

{

"verse": "...",

"index": "..."

},

// ... more verses

]

Edge Cases Considered

The script relies on the presence of the pattern // Avg_X.Y at the end of a two-line verse to identify and extract verses along with their index.

It assumes that each verse consists of exactly two lines preceding this pattern. Lines that do not fit this pattern will be skipped.

The script includes basic error handling for reading the DOCX file. If the file is not found or there's an error reading it, the script might not function correctly.

Repository Contents

This repository contains:



Sanskrit_text_code.ipynb: The Python script (likely a Jupyter Notebook) used for extracting the verses.

verses.json: The JSON file containing the extracted verses and their indices.

README.md: This file, providing information about the project.

https://github.com/Vedant22-marda/Sanskrit_Gita_text_extractor