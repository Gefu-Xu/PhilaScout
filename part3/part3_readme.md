## Purpose of this project phase (part 3):
The third part of the project focuses on integrating all components from previous parts to perform final user text and image queries.

## Steps included:

### Step1: Upload the artifacts created in part 1 & 2
Upload the artifacts created previously.

### Step2: Define utility functions
Define utility functions 'print progress', 'display stamps', and 'calculate API costs', which are the same as in Part 1

### Step3: Convert stamp image descriptions to OpenAI embeddings and store them in ChromaDB
As in Step 5 of Part 1, transform all stamp image descriptions into OpenAI embeddings and store them in ChromaDB for retrieval.

### Step4: Reuse functions from Part 1 to generate descriptions for user query images
Reuse functions from Part 1 to generate descriptions for stamp images from user queries.

### Step5: Reuse functions from Part 2 to extract stamp value info from text files
Reuse functions from Part 2 to extract stamp value information from unstructured documents.

### Step6: Integrate all components into functions that support user image or text queries
Integrate functions to support two scenarios:
- Scenario 1: User types in a stamp description
- Scenario 2: User uploads a stamp image

## Related files

### Main Jupyter notebook:
- `part3.ipynb` - The main Jupyter Notebook for Part 3.

### Google Colab folder structure:
- `/content/` 
  - `stamp.csv` - A csv file to track all stamp data, which includes stamp_id, img_file_location, and image_description.
  - `/chroma_db/` - The vector database storing the embeddings of stamp image descriptions.
  - `/img/` - The folder to store all stamp images.
    - `p0_4603_0.jpg`
    - `p0_4608-12_1.jpg`
    - ...
  - `/txt/` - The folder to store text files that contain stamp value information
    - `p0.txt` - The text file converted from the index0 page of the demostration pdf
    - `p1.txt`
    - ...
  - `/tmp/` - The folder to store user uploaded test images
    - `test1_1.png`
    - `test1_2.png`
    - ...

### User's local PC/Mac folder:
  - `/test/` - The folder to store test images, which are either from the `/img` folder or from the internet.
    - `test1_1.png`
    - `test1_2.png`
    - ...