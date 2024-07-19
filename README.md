PDF Table Extraction and Processing
> Introduction:
* This repository contains a. ipynb file designed to extract tables from a PDF file, convert the data into JSON format, and process the JSON data to extract specific information. 
* This is particularly useful for automating the extraction of tabular data from PDFs, making it easier to analyze and manipulate.
> Dependencies:
To run the code in this notebook, ensure you have the following installed on your system-
Python 3.x: The code is written in Python, so you will need a Python environment to execute it.
Jupyter Notebook/colab/Visual Studio Code: This is necessary to open and run the. ipynb file or .py file.
tabula-py: A Python wrapper for tabula-java, which is used for reading tables from PDF files.
You can install the necessary library using pip with the following command:
pip install tabula-py
> Tutorial
* Begin by cloning the repository to your local machine using Git:
git clone https://github.com/yourusername/your-repo-name.git
* cd your-repo-name
* Once the repository is cloned, open the code: 
jupyter notebook extract_code. ipynb. You can use any of the platforms given in the requirements to open the code and to run it. 
* There are two formats available - .py and. ipynb. You can use any of the formats according to your choice. 
* Setting the PDF File Path : 
Before running the notebook, you need to specify the path to the PDF file from which you want to extract tables.
* Edit the pdf_path variable in the notebook to point to your PDF file: Copy code, pdf_path = '/path/to/your/pdf/file.pdf' 
Here, I used a sample pdf.
* Running the Notebook,
Execute the cells in the notebook sequentially to perform the following tasks:
* Install and import necessary libraries: Ensure tabula-py is installed and import required libraries.
* Read the PDF file: Use tabula.read_pdf() to read tables from the specified PDF file.
* Convert tables to JSON: Convert the extracted tables into JSON format for easier manipulation.
* Process the JSON data: Extract specific rows and columns from the tables and process them as needed.
* Notebook Overview-
The notebook is structured to guide you through each step of the process:
* Installation and Importing Libraries: The first cell installs the tabula-py library if it is not already installed and imports all necessary libraries for the project.
* Reading the PDF: The code reads tables from the specified PDF file using the tabula.read_pdf() function, which returns a list of DataFrame objects, each representing a table detected in the PDF.
* Converting to JSON: The extracted tables are converted to JSON format using the to_json() method of DataFrame objects. This allows for easier data manipulation and extraction.
* Processing JSON Data: Specific rows and columns from the JSON data are processed to extract relevant information. This involves converting rows into lists of tuples and extracting values based on predefined keys.

