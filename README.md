# RC-3D-printer-over-Telegram-automated
At the Robotics Club of Tishreen University, we faced challenges with managing the scheduling of our 3D printing system. To address this issue, I developed a Python-based system that automates and organizes the entire process.

## System Workflow:
##### 1) File Submission: Members send their .gcode files through a designated Telegram group.
##### 2) File Management: The system automatically downloads the .gcode files from the group and schedules them in an Excel file.
##### 3) GUI Interaction: Members can interact with a user-friendly graphical interface (GUI) either in person or through a private Telegram chat. They are presented with options to:
##### Print the file
##### Not print the file and delete
##### Schedule the print for later
##### 4) Automated Printing: Once the member makes a selection, the system sends the .gcode to the 3D printer via a serial port. The file is copied onto the printer's built-in SD card, and the print begins automatically, without the need for further human interaction.
## Features:
##### 1) Easy to Use: The system is designed with simplicity in mind, making it accessible for all members.
##### 2) Time-Efficient: It automates the printing process, reducing manual involvement and saving time.
##### 3) Organized Scheduling: Files are managed and organized efficiently, ensuring smooth scheduling of print jobs.
##### 4) Data Security: The system includes safe data encryption for file management and communication.
#### This system streamlines our 3D printing workflow, enhancing productivity and ensuring reliable and organized print management for the club.

## install:
### 1) first you need to install the following libraries:
   ```bash
   pip install telebot
   pip install openpyxl
   pip install pandas
   pip install colorama
   pip install tqdm
   pip install asyncio
   pip install random string
   pip install serial
   ```
### 2) Get Telegram-API Credentials:

To get Telegram-API credentials for integrating with Python, you'll need to follow a few steps:

a) Create a Google Cloud Project: Go to the [Google Cloud Console](https://cloud.google.com/) and create a new project.

b) Enable the Google Sheets API: Within the project, go to the "APIs & Services" section and enable the Google Sheets API and Google Drive API. This allows your project to interact with Google Sheets.

c) Create a Service Account: In the "APIs & Services" section, create a service account. This account will act on your behalf when accessing the Google Sheets data. Generate a key in JSON format during this step and download it.
