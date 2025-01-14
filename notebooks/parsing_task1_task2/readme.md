Collecting workspace information

Here's a readme for the project:

# Conference Paper Classifier

This tool helps classify academic papers into different conferences (CVPR, NIPS, EMNLP, etc.) based on their content.

## Setup

1. Create a `.env` file in the root directory with your OpenAI API key:
```
OPENAI_API_KEY=your_key_here
```

2. Create an 

input-pdfs

 folder in the root directory if it doesn't exist already.

3. Place the PDF papers you want to classify in the 

input-pdfs

 folder. The files should be named as `P001.pdf`, `P002.pdf`, etc.

## Usage

1. Open 

final_notebook.ipynb

 in Jupyter Notebook or Google Colab.

2. Click "Run All" to execute the entire notebook.

3. The results will be saved in 

results.csv

 with the conference classification and reasoning for each paper.

## Notes

- Do not modify the existing Gemini and Pinecone API keys in the notebooks as they are configured for the current setup.
- Make sure your PDFs are research papers in a standard academic format.
- The system processes papers sequentially and maintains rate limits, so classification may take some time depending on the number of papers.

## Requirements

All required packages are listed in 

requirements.txt

 and will be installed automatically when running the notebook.

## Output

The tool generates:
- Extracted text from PDFs in `extracted_full_texts.txt`
- Abstracts in `extracted_full_abstracts.txt`
- Final classifications in 

results.csv