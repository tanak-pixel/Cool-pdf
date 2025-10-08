PDFTris — Tetris Inside a PDF
Created by Tanak Solanki
Overview
PDFTris embeds a playable Tetris game directly in a PDF using form fields and embedded JavaScript. The Python script gengrid.py generates the PDF with the grid, controls, and logic bundled in.

Features
Colored tetrominoes per piece type
Smooth gameplay in modern PDF readers (PDFium/PDF.js)
Progressive speed increase as you clear lines
Pause (P) and quick drop (Space)
On-page buttons for Start, Left, Right, Down, Rotate
Output
Build produces cool.pdf in the project root.
Recommended viewers: Chrome (PDFium) or Firefox (PDF.js).
Controls
W: Rotate
A: Move left
D: Move right
S: Soft drop
Space: Quick multi-step drop
P: Pause / resume
Prerequisites
Python 3.8+
No third-party Python packages required
Build and Run
Open a terminal in the project folder:
cd C:\Users\Dell\OneDrive\Desktop\Programs\Cool-pdf\Cool-pdf>
Generate the PDF:
python gengrid.py
Open cool.pdf in Chrome or Firefox and play.
How It Works (Brief)
The grid is a matrix of PDF button widgets acting as pixels.
Embedded JavaScript manages piece generation, rotation, movement, collision, line clears, scoring, and drawing by toggling visibility and setting fill colors on the widgets.
Notes
Some PDF viewers (including older or non-standard ones) may not execute the embedded JavaScript or show colors properly. Use Chrome or Firefox for best results.
Credits
Original idea: “Tetris in a PDF” (see background at https://th0mas.nl/2025/01/12/tetris-in-a-pdf/).
Enhancements and colorized gameplay:Tanak Solanki .
License
Provided as-is for educational and demonstration purposes.
