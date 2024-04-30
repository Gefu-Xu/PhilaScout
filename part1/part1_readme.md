## Purpose of this project phase (part 1):
The first part of the project focuses on pre-processing the raw dataset and preparing a vector database (ChromaDB) for similarity search.

## Steps included:

### Step1: Download and prepare the stamp catalog
Download a stamp catalog and prepare a demonstration pdf featuring stamps issued in 2012 to begin the project.

### Step2: Define utility functions
Implement utility functions to 'print progress', 'display stamps', and 'calculate API costs'.

### Step3: Extract stamp images from pdf
Extract all stamp images from the demonstration pdf and store them in the '/img' folder.

### Step4: Generate descriptions for stamp images using OpenAI's multi-modal model
Utilize OpenAI's multi-modal model to generate descriptions for each stamp image.

### Step5: Convert stamp image descriptions to OpenAI embeddings and store in ChromaDB
Further transform stamp image descriptions into OpenAI embeddings and store them in ChromaDB for future retrieval.

### Step6: Perform test queries using text or images
Conduct tests to assess the effectiveness of similarity searches in ChromaDB using either text or images.

### Step7: Backup generated artifacts
Backup all generated artifacts for next steps.

## Related files

### Main Jupyter notebook:
- `part1.ipynb` - The main Jupyter Notebook for Part 1.

### Google Colab folder structure:
- `/content/` 
  - `Mystics_2024_US_Stamp_Catalog.pdf` - The original dataset downloaded from the internet.
  - `2012.pdf` - A small demonstration dataset containing stamps issued in the year 2012.
  - `debug.pdf` - Builds on `2012.pdf` by highlighting the Scott number and detect_radius in the pdf file.
  - `stamp.csv` - A csv file to track all stamp data, which includes stamp_id, img_file_location, and image_description.
  - `/chroma_db/` - The vector database storing the embeddings of stamp image descriptions.
  - `/img/` - The folder to store all stamp images.
    - `p0_4603_0.jpg`
    - `p0_4608-12_1.jpg`
    - ...
  - `/test/` - The folder to store test images, which are either from the `/img` folder or from the internet.
    - `test1_1.png`
    - `test1_2.png`
    - ...

