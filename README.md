# Resume-extraction-and-candidate-job-matching
### Resume extraction and candidate job matching using python transformers library DistilBERT.
The python notebook file contains code to solve all the 3 tasks given below.

Objective: Build a PDF extractor to pull relevant details from CVs in PDF format, and match them against the job descriptions from the Hugging Face dataset.

1. PDF Data Extraction
Objective: Extract details from CVs in PDF format.
Dataset: Kaggle Resume Dataset

Instructions:
Download the Kaggle "resume dataset". https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset
Build a PDF extractor using Python, leveraging libraries such as PyPDF2 or PDFMiner.
Extract the key details:
Category (Job role)
Skills
Education (Degree, Institution)

2. Job Description Data Understanding

Objective: Fetch and comprehend job descriptions from the Hugging Face dataset.
Dataset: Job Descriptions from Hugging Face. https://huggingface.co/datasets/jacob-hugging-face/job-descriptions

Instructions:
Use the Hugging Face datasets library to fetch the job descriptions. For this task, consider extracting 10-15 job descriptions.

3. Candidate-Job Matching
Objective: Match extracted CV details against the fetched job descriptions based on skills and education.

Tools Used: Use the Transformers library by Hugging Face. BERT or DistilBERT (can be replaced with better LLMs. This task was performed with minimal GPU power)

### Tasks Performed
- Tokenizing and preprocessing both the job descriptions and the extracted CV details from the PDFs.
- Converting the tokenized text into embeddings using a pretrained model like DistilBERT from Hugging Face.
- For each job description, calculating the cosine similarity between its embedding and the embeddings of the CVs.
- Ranking CVs based on this similarity for each job description.
- Listing the top 5 CVs for each job description based on the highest similarity scores.
