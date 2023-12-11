# Biz-Card-Data-Extraction-with-OCR
**Imports:**
pandas, streamlit, easyocr, mysql.connector, PIL, cv2, os, matplotlib.pyplot, re: Importing necessary libraries for data manipulation, Streamlit app creation, OCR (using EasyOCR), image processing, database connectivity, and regular expressions.

**Page Configuration and Background Image:**
Setting up the Streamlit page configuration with a custom icon and a background image.
Option Menu Creation:
Creating an option menu using streamlit_option_menu to navigate between Home, Upload & Extract, and Modify sections.

**Initializing EasyOCR Reader:**
Creating an EasyOCR reader object to perform optical character recognition.

**Connecting to MySQL Database:**
Establishing a connection to a MySQL database and creating a table named card_data if it doesn't exist already. The table schema includes fields for various card details along with an image field to store card images.
Home Menu:
Displays information about the application and its purpose in the Home section.

**Upload & Extract Menu:**
Allows users to upload business card images.
Uses EasyOCR to extract text data from the uploaded image.
Processes the extracted text to identify specific card details like company name, card holder, designation, contact info, etc.
Displays the extracted data in a table format and provides an option to upload the extracted data to the connected MySQL database.

**Modify Menu:**
Provides options to alter or delete the extracted data in the database.
Allows selecting a specific card to update or delete its information.
For alteration, it displays the existing information and allows modifying it before updating in the database.
For deletion, it confirms the deletion of the selected card's information from the database.

**Overall Functionality:**
Handles image upload, OCR text extraction, text processing, database operations, and user interface management using Streamlit components.
This code integrates various functionalities like image processing, text extraction, database handling, and user interface development to create a complete application for business card data extraction and management.
