## Purpose of this project phase (part 2):
The second part of the project focuses on preparing text files for stamp value information queries.

## Steps included:

### Step1: Upload the demonstration dataset
Upload the demonstration pdf created in Part 1.

### Step2: Define utility functions
Define utility functions 'print progress' and 'calculate API costs', which are the same as in Part 1.

### Step3: Convert the demonstration pdf into text files
Convert the demonstration pdf into multiple text files, creating one text file for each page. Converted text files contain stamp value information and are stored in the '/txt' folder.

### Step4: Extract stamp value info from text files using OpenAI's LLM model
Utilize OpenAI's LLM model to extract stamp value info from the text files based on user queries.

### Step5: Perform queries to test stamp value info extraction
Conduct tests to assess the effectiveness of the stamp value info extraction.

### Step6: Backup generated artifacts
Backup all generated artifacts for next steps.

## Related files

### Main Jupyter notebook:
- `part2.ipynb` - The main Jupyter Notebook for Part 2.

### Google Colab folder structure:
- `/content/` 
  - `2012.pdf` - A small demonstration dataset containing stamps issued in the year 2012.
  - `/txt/` - The folder to store text files that contain stamp value information
    - `p0.txt` - The text file converted from the index0 page of the demostration pdf
    - `p1.txt`
    - ...