# Programming: First Program (work in progress)

I have tried to learn some basic coding using the excellent ["Python for everybody"](https://www.py4e.com/) online course and book.

After learning the basic syntax, I went out to look for opportunities to automate a task at my current work. One such task was the production of a portfolio overview. 
This would usually consist of going through more than 1500 word and pdf-files (each year), scan those for a few distinct search terms and enter information about the findings in an excel sheet.
In the following you´ll find the code with some comments and a few thoughts and learnings.

Step 1. Import the libraries
```python
# Prints '2'
print(1+1)
import os 
import re
import docx2txt
import PyPDF2
from PIL import Image
import pytesseract
#import textract
import sys
from pdf2image import convert_from_path
import xlsxwriter
```
