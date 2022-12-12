# About FutureMakers2022:
This repository contains files I worked on during the FutureMakers program by SureStart in summer 2022. 
In the first part of the program, I attended lectures and completed coding homework. 
In the second part (Create-a-thon), my team and I worked on Legal Linguists, a translation tool. We presented this result in a pitch meeting hosted by MIT, and out of 16 competing teams, we won the grand prize. 

# High Level Design:
1. What is Legal Linguists:

Legal Linguists is a translation tool for legal documents. It is designed for people who do not grow up speaking English, such as immigrants.

2. Why Legal Linguists:

Translation is expensive, and can be inaccurate. These problems are more severe for legal documents because they are technical and require professional knowledge. More importantly, mistranslating a legal file lead to negligence or law-breaking. This puts people in jeopardy, especially immigrants who are in a vulnerable situation. By providing accurate and quality-aware translation, we help non-native-English-speakers better navigate through legal problems.

3. How Legal Linguists works:

Legal Linguists processes a legal document in three steps. First, the OCR module processes the input file, a photograph of the legal document, and converts it into text file. This photograph is preferably a scanned document, which can be produced on free software such as CamScanner on a smartphone. Second, the text file is handled by the translation module, which is a neural network trained on legal documents. The result is the content of the legal document translated to the user's preferred choice of language. Finally, the translation is presented to the user, with the addition of highlighting for legal terms as well as terms with low confidence level in translation. This allows the user to understand which words and concepts to look out for, and seek help for words that Legal Linguists cannot handle with confidence.


# Files:
  1. Day_1 to Day_17

These python notebooks are a collection of 115 coding homework problems I completed during the first part of the FutureMakers 2022 program. They are coding and written assignments on AI and machine learning.

  2. Web_Scrapign_Workshop.ipynb

This is code I wrote during a web-scraping workshop in the FutureMakers program. I used BeautifulSoup to extract text data from www.fsis.usda.gov. 

  3. LegalLinguists_OCR_Module.ipynb

This is the OCR (Optical Character Recognition) Module for Legal Linguists. I used the ocrmypdf and pdfplumber modules, following youtube tutorial. At the end, I convert the output of the modules into a list of Strings, so that the Translation Module of our tool can translate the words one by one. 
 
  4. OCR_prototype_01.ipynb

Prototype for the OCR_Module project; I used pdf2image and easyocr. This method is not streamlined because I first need to convert input images into the desired format before running OCR on it.

  5. Requirements.txt
 
A list of commands to install all modules needed to run LegalLinguists_OCR_Module.ipynb.

  6. TEST_DOC_2.pdf
  
A PDF file for testing out the OCR Module found in LegalLinguists_OCR_Module.ipynb

# Setup and How to Run:
(for LegalLinguists_OCR_Module.ipynb)
This is the Setup instructions for the OCR module for Legal Linguists, written in Python 3.8.16. This module converts scanned pdfs into text (so that their content gets translated) to a CSV containing all words from the PDF (the tokenization can be customized)
  1. Install all required modules using commands in Requirements.txt
  
  2. Provide access to your PDF file:
  
  Method A: Obtain a URL for the PDF file you would like OCR-ed. Example: https://bit.ly/2UJgUpO; 
  
  Method B: upload your PDF file to the Collab notebook to access it directly.
  
  3. Run LegalLinguists_OCR_Module.ipynb. 
  
  For methods A and B, follow the comments to change the parameter for .open() method. 
  
  4. Collect the output CSV file, which holds all words extracted from the PDF.
  
  5. View the OCR module's output at the bottom of the Colab notebook.
  For further explanation for the code, please see the comments in the ipynb file.

# Dependency:
(for LegalLinguists_OCR_Module.ipynb)
see Requirements.txt
  
  csv
  
  reader (from csv)



