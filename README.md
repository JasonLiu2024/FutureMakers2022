# About FutureMakers2022:
This repository contains files I worked on during the FutureMakers program by SureStart in summer 2022. 
In the first part of the program, I attended lectures and completed coding homework. 
In the second part (Create-a-thon), my team and I worked on Legal Linguists, a translation tool. We presented this result in a pitch meeting hosted by MIT, and out of 16 competing teams, we won the grand prize. 

# Files:
  1. Day_1 to Day_17

These python notebooks are coding homework I completed during the first part of the FutureMakers 2022 program. They are coding and written problems on AI and machine learning.

  2. Web_Scrapign_Workshop.ipynb

This is code I wrote during a web-scraping workshop in the FutureMakers program. I used BeautifulSoup to extract text data from www.fsis.usda.gov. 

  3. LegalLinguists_OCR_Module.ipynb

This is the OCR (Optical Character Recognition) Module for Legal Linguists. I used the ocrmypdf and pdfplumber modules, following youtube tutorial. At the end, I convert the output of the modules into a list of Strings, so that the Translation Module of our tool can translate the words one by one. 
 
  4. OCR_prototype_01.ipynb

Prototype for the OCR_Module project; I used pdf2image and easyocr. This method is not streamlined because I first need to convert input images into the desired format before running OCR on it.

  5. Dependency.txt
 
A list of commands to install all modules needed to run LegalLinguists_OCR_Module.ipynb.

  6. TEST_DOC_2.pdf
  
A PDF file for testing out the OCR Module found in LegalLinguists_OCR_Module.ipynb

# Setup and How to Run:
(for LegalLinguists_OCR_Module.ipynb)
This is the Setup instructions for the OCR module for Legal Linguists, written in Python 3.8.16. This module converts scanned pdfs into text (so that their content gets translated) to a CSV containing all words from the PDF (the tokenization can be customized)
  1. Install all required modules using commands in Dependency.txt
  2. Provide access to your PDF file:
  
  Method A: Obtain a URL for the PDF file you would like OCR-ed. Example: https://bit.ly/2UJgUpO; 
  
  Method B: upload your PDF file to the Collab notebook to access it directly.
  
  3. Run LegalLinguists_OCR_Module.ipynb. 
  
  For methods A and B, follow the comments to change the parameter for .open() method. 
  
  4. Collect the output CSV file, which holds all words extracted from the PDF.
  
  5. View the OCR module's output at the bottom of the Collab notebook.
  For further explanation for the code, please see the comments in the ipynb file.

# Dependency:
(for LegalLinguists_OCR_Module.ipynb)
The OCR module has the following dependencies:
  
  ocrmypdf
  
  pdfplumber
  
  os
  
  requests
  
  pdfplumber
  
  re
  
  pandas
  
  numpy
  
  collections
  
  csv
  
  reader (from csv)



