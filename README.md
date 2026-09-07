🗂️ File Ops Console

A professional local file management application built with Python and Streamlit.

File Ops Console provides a simple, interactive interface for performing common text-file operations from a local environment, including create, read, rename, append, overwrite, and delete actions.

The application combines straightforward file-system functionality with a clean console-style UI, input validation, error handling, and a session-based activity log.

📌 Project Overview

File Ops Console was developed to provide an easy-to-use alternative to performing basic file operations directly from the command line or file explorer.

The application organizes file management into four main operations:

Operation

Functionality

📄 Create

Create a new text file and write content

👁️ Read

Read and preview an existing text file

✏️ Update

Rename, append content, or overwrite a file

🗑️ Delete

Delete an existing file with confirmation

The project uses Python's built-in pathlib module for file-system operations and Streamlit for the interactive user interface.

✨ Key Features

📄 Create File

Create a new text file by entering:

File name

File content

The application checks whether a file with the same name already exists before creating it.

👁️ Read File

Read an existing UTF-8 text file and preview its content inside the application.

Validation and error handling include:

Empty file names

Missing files

Non-file paths

Invalid UTF-8 text

Permission errors

Other operating-system file errors

✏️ Update File

The Update section provides three file-management options.

Rename

Rename an existing file while validating:

Source file existence

Destination file name

Duplicate destination names

Permissions

Append Content

Add new text to the end of an existing file.

When the file already contains data, the application adds a newline before the appended content.

Overwrite File

Replace the current file contents with new content.

🗑️ Delete File

Delete an existing file after an explicit confirmation step to reduce accidental deletion.

📋 Activity Log

The application maintains a session-based activity log containing:

Operation status

Timestamp

Action message

The log records successful, informational, and failed operations.

🖥️ Application Interface

The interface is designed around a clean console-style workflow with:

Sidebar operation navigation

Operation-specific panels

File name and content inputs

File path indicator

Interactive controls

Activity console

Success and error feedback

Responsive Streamlit layout

📸 Application Screenshots

Create File

Create a new file and enter its content directly through the application.



Read File

Read and preview the contents of an existing text file.



Update File

Rename an existing file, append content, or overwrite its contents.



Delete File

Delete an existing file after confirming the operation.



⚙️ How It Works

                    FILE OPS CONSOLE
                           │
              ┌────────────┼────────────┐
              │            │            │
           CREATE         READ        UPDATE
              │            │       ┌────┼────┐
              │            │       │    │    │
              │            │    Rename Append Overwrite
              │            │
              └────────────┼────────────┘
                           │
                         DELETE
                           │
                           ▼
                    ACTIVITY LOG

🛠️ Technology Stack

Python

Streamlit

pathlib

datetime

HTML/CSS

Streamlit Session State

Core Components

Python
├── pathlib
│   ├── Create files
│   ├── Read files
│   ├── Rename files
│   └── Delete files
│
├── datetime
│   └── Activity timestamps
│
└── Streamlit
    ├── User interface
    ├── Navigation
    ├── Inputs
    ├── Buttons
    └── Session state

🧠 Skills Demonstrated

This project demonstrates practical skills in:

Python Programming

Streamlit Application Development

File-System Operations

pathlib

User Input Validation

Exception Handling

Session State Management

Interactive UI Development

HTML/CSS Customization

Activity Logging

Local Application Development

🔍 Error Handling

The application includes validation and error handling for common file-operation scenarios, including:

Empty file names

Existing files during creation

Missing files

Paths that are not files

Duplicate rename targets

Permission errors

Operating-system errors

Invalid UTF-8 text files

Unconfirmed delete operations

Clear messages are added to the activity log when an operation succeeds or fails.

🔒 Local File Operations

File operations are performed using Python's local file-system APIs.

The application uses pathlib.Path to interact with local files and does not require a database for its core functionality.

Because the application works with local file paths, it should be run in an environment where you understand which files and directories it can access.

🚀 Installation & Setup

1. Clone the Repository

git clone https://github.com/YOUR_USERNAME/File-Ops-Console.git

2. Open the Project Folder

cd File-Ops-Console

3. Install Streamlit

pip install streamlit

4. Run the Application

streamlit run FIleApp.py

The application will open in your default web browser.

If you rename FIleApp.py, update the command accordingly.

📁 Project Structure

File-Ops-Console/
│
├── FIleApp.py
├── README.md
│
└── Screenshots/
    ├── Delete file.png
    ├── Create File.png
    ├── Read File.png
    └── Update File.png

🎯 Project Objectives

The project was created to:

Build a practical Python application

Practice Streamlit development

Demonstrate local file-system operations

Implement input validation

Handle common file-operation errors

Provide clear user feedback

Create a foundation for future file-management features

🚀 Future Enhancements

Potential improvements include:

📁 Directory browsing

🔎 File search

📋 File listing and sorting

📊 File metadata and size information

📦 Multiple-file operations

📤 File upload and download

🌳 Folder navigation

📝 Rich text editing

📜 Persistent activity history

⚙️ Configurable working directories

👨‍💻 About the Developer

Muhammad Faisal Jahangeer

Python Developer | Data Analyst | Data Science & AI/ML Enthusiast

I build practical Python applications and data-driven projects with a focus on turning technical concepts into useful, real-world solutions.

Areas of Interest

Python Development

Data Analytics

Data Science

Machine Learning

Artificial Intelligence

Business Intelligence

Data Visualization

Automation

🔗 Connect With Me



⭐ Support

If you find this project useful:

⭐ Star the repository

🍴 Fork the project

💡 Share feedback

🤝 Connect with me

<p align="center">

Python • Streamlit • File Management • Local Automation

</p>
