# American_British_Converter

Install all the requirements using the below code
    !pip install -r requirements.txt
Both CLI and Jupyter versions of the code are given. To run the CLI version follow
the below mentioned approach.
    python \path_to_file\NLP_Project_Final.py

Introduction

The objective is to convert any words that are minimum in a given document. The words can either be American or British depending on the document.
A document can consist both American and British words. If the document were to be published as a journal or publication, this can issue. This is why the problem has to be solved.
So to solve this issue, One can use either Machine Learning NLP or Text processing or both. For this evaluation, I will be considering it as a Text Processing.

Explanation

First we need to consider that text processing will have an affect on the document. To treat this problem I leveraged docxtext and python-docx library. To count the word we must have a list of British and American words. So, a custom
word list is created. Then both the lists are compared with the document to get the count of British and American words in the document.

Any word that are matched from the lists must also have the original format.
Example: The word Aluminum can exist as aluminum, Aluminum and ALUMINUM.

So, Separate list are then created for each of these versions. Then converted back to a dict format and their consecutive words are kept. After getting the distribution for both American and British words. Based on the distribution the lesser value is then transformed.
Replacement for these words in a document while keeping the format same is an issue that can be solved using the above mentioned library. Words that are present in both paragraph and table can be changed with the help of these library.
