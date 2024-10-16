# -Exercise-7-Read-and-Extract-Text-from-PDF
```
Name: THIRISHA S
Reg No: 212222230160
```
# Aim:
To automate the process of extracting text from a PDF file and saving the extracted content to a text file using UiPath.

# Equipment Required:
UiPath Studio – A tool for automating tasks and workflows.
PDF File – The file from which the text will be extracted.
Text File – The file where the extracted text will be saved.
Computer with the following configuration:
At least 4 GB RAM.
A 2.0 GHz processor.
Running Windows OS.

# Procedure:
# Create a New Project in UiPath Studio:
Open UiPath Studio.
Under the New Project tab, select Process.
Name the project (e.g., Extract PDF Text) and click Create.
This will set up a new project for you to begin automating the task of reading from a PDF.

# Install the PDF Activities Package:
Click on Manage Packages from the top toolbar.
Search for the UiPath.PDF.Activities package and install it.
This package contains tools specifically designed to handle PDF files (like reading text, extracting tables, etc.).

# Define File Paths:
Go to the Variables pane in UiPath Studio to define paths for the PDF file and the output text file:
Create a String variable called pdfFilePath for the PDF file path.

pdfFilePath = "C:\Users\admin\Documents\Sample.pdf"

Create a String variable called textFilePath for the output text file.

textFilePath = "C:\Users\admin\Documents\ExtractedText.txt"

# Use 'Read PDF Text' Activity:
In the Activities panel, search for Read PDF Text and drag it into your sequence.
Set the FileName property of the activity to pdfFilePath (the variable containing the path to your PDF).
Create a new String variable called pdfText to store the extracted text from the PDF file.
Set the Output property of the Read PDF Text activity to pdfText.

# Write the Extracted Text to a File:
Search for the Write Text File activity in the Activities panel and drag it below the Read PDF Text activity.
Set the FileName property of the Write Text File activity to textFilePath.
Set the Text property to pdfText (the variable containing the extracted PDF text).
This activity will write the extracted text from the PDF into the specified text file.

# Save and Run the Workflow:
Press CTRL+S to save your workflow.
Click the Run button in UiPath Studio to execute the workflow.
Once the process completes, the robot will extract the text from the PDF and save it into the designated text file.
# UiPath WorkFlow:
![Screenshot 2024-09-26 201225](https://github.com/user-attachments/assets/f5fbead1-5ef9-465b-828c-8dce1a2ed1fe)
![Screenshot 2024-09-26 201313](https://github.com/user-attachments/assets/d8dcc9e2-adb6-42e1-9eef-68199e3cd534)
![Screenshot 2024-09-26 201536](https://github.com/user-attachments/assets/cc81ace9-e7f5-422f-b638-1acba75a1156)
![Screenshot 2024-09-26 201714](https://github.com/user-attachments/assets/2716f3fa-1021-4c96-9427-dd59e4b310ef)

# Result:
The text from the PDF file is successfully extracted and saved to a text file using UiPath Studio. The process automates the extraction of text from a PDF, which can then be used in further automation tasks, such as data analysis or report generation.

