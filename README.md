Text File to Dictionary Converter
A simple client-side web tool that converts structured .txt vocabulary files into a JavaScript-style dictionary (array of word–translation pairs). The tool runs entirely in the browser — no backend, no uploads, and no dependencies.
________________________________________
Features
•	Upload a .txt file with vocabulary entries
•	Automatically parses entries in the format:
word [pronunciation] translation
•	Outputs a JavaScript-friendly array format:
•	["word", "translation"]
•	Toggle output order:
o	["word", "translation"]
o	["translation", "word"]
•	Copy results to clipboard with one click
•	Fully offline and privacy-friendly
________________________________________
Demo Use Case
This tool is ideal for:
•	Preparing dictionaries for language-learning apps
•	Generating datasets for AI / NLP projects
•	Converting textbook vocabulary lists into structured data
________________________________________
Expected Input Format
Each line (or entry) in the .txt file should follow this pattern:
word or phrase [pronunciation] translation
Example Input
take off [teɪk ɒf] взлетать; снимать
break down [breɪk daʊn] ломаться; выходить из строя
________________________________________
Output Format
By default:
[
  ["take off", "взлетать, снимать"],
  ["break down", "ломаться, выходить из строя"]
]
With “Switch output order” enabled:
[
  ["взлетать, снимать", "take off"],
  ["ломаться, выходить из строя", "break down"]
]
________________________________________
How to Use
1.	Download or clone this repository
2.	Open index.html in any modern browser
3.	Upload a .txt file
4.	(Optional) Toggle output order
5.	Copy the generated result to your clipboard
________________________________________
Technical Overview
•	HTML + CSS for layout and styling
•	Vanilla JavaScript
•	Uses:
o	FileReader for local file processing
o	Regular expressions for parsing
o	Clipboard API for copying results
•	No frameworks or external libraries
________________________________________
Limitations
•	Designed primarily for Latin-based source words
•	Assumes consistent formatting in the input file
•	Does not validate pronunciation content (ignored during output)
________________________________________
Privacy
All processing is done locally in your browser.
No files are uploaded or transmitted anywhere.
________________________________________
License
MIT License — free to use, modify, and distribute.

