# Grimace-App-for-Mouse-Facial-Expression-Assessment
Grimace App for Mouse Facial Expression Assessment
Python application for blinded annotation of mouse photos using facial grimace action units. Exports raw results and per-animal means to Excel.

Requirements
Python 3.9+.

Packages: customtkinter, pillow, pandas, openpyxl. See requirements.txt.​

Installation
Install Python 3.9+.

Install dependencies:

Windows/macOS: Use your Python environment manager (for example, pip install -r requirements.txt).

Prepare a folder named fotos with your image files (png/jpg/jpeg) in the same directory as the script.

Usage
Run grimace_app.py.

Click the score buttons (0–2) for each action unit.

Click “Next Photo” to record and proceed.

When finished, the app saves:

resultado_scores.xlsx with two sheets:

Raw_Results: photo-level scores and metadata.

Means: per-animal mean of Photo_Mean.

The app attempts to open the Excel file automatically on Windows.

Notes
Filenames are parsed with the pattern: Group Animal - Day (PhotoNum), e.g., Control 12 - 3 (1). Adjust the regex in parse_photo_info if your format differs.
