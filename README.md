
# BizCardX-Extracting_Business_Card_Data_with_OCR
!(r'C:\pythan\DATA SCEINCE\BizcardX\download.jpg')


## project overview
```bash
 BizCardX is a user-friendly tool for extracting information from business cards. 
The tool uses OCR technology to recognize text on business cards and extracts the data into a SQL database after classification using regular expressions.
Users can access the extracted information using a GUI built using streamlit. The BizCardX application is a simple and intuitive user interface that guides users through the process of uploading the business card image and extracting its information.
The extracted information would be displayed in a clean and organized manner, and users would be able to easily add it to the database with the click of a button. 
Further the data stored in database can be easily Read, updated and deleted by user as per the requirement.
 ```
## Key Technologies and Skills
```bash
* Python
* Pandas
* easy OCR
* MYSQL
* Streamlit
```
## Programming hints
```http
Write the program to below content
1)Install the required packages: pip install -r requirements.txt
2)upload the business card
3)Extract the data with easy OCR and store the data to MYSQL
4)Run the Streamlit app: streamlit run app.py
5)Access the app in your browser at http://localhost:8501
```

## What is EasyOCR?
```bash
EasyOCR, as the name suggests, is a Python package that allows computer vision developers to effortlessly perform Optical Character Recognition.It is a Python library for Optical Character Recognition (OCR) that allows you to easily extract text from images and scanned documents. In my project I am using easyOCR to extract text from business cards.

When it comes to OCR, EasyOCR is by far the most straightforward way to apply Optical Character Recognition:

* The EasyOCR package can be installed with a single pip command.
* The dependencies on the EasyOCR package are minimal, making it easy to configure your OCR development environment.
* Once EasyOCR is installed, only one import statement is required to import the package into your project.
* From there, all you need is two lines of code to perform OCR — one to initialize the Reader class and then another to OCR the image via the readtext function.

## program work flow
```bash
To get started with BizCardX Data Extraction, follow the steps below:

* Install the required libraries using the pip install command. Streamlit, mysql.connector, pandas, easyocr.

* pip install [Name of the library]
Execute the “BizCardX_main.py” using the streamlit run command.

* streamlit run BizCardX_main.py
A webpage is displayed in browser, I have created the app with three menu options namely HOME, UPLOAD & EXTRACT, MODIFY where user has the option to upload the respective Business Card whose information has to be extracted, stored, modified or deleted if needed.

* Once user uploads a business card, the text present in the card is extracted by easyocr library.

* The extracted text is sent to get_data() function(user defined- I have coded this function) for respective text classification as company name, card holder name, designation, mobile number, email address, website URL, area, city, state, and pin code using loops and some regular expression.

* The classified data is displayed on screen which can be further edited by user based on requirement.

* On Clicking Upload to Database Button the data gets stored in the MySQL Database. (Note: Provide respective host, user, password, database name in create_database, sql_table_creation and connect_database for establishing connection.)

* Further with the help of MODIFY menu the uploaded data’s in SQL Database can be accessed for Read, Update and Delete Operations.
```
