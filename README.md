# 🗂️ File Ops Console

A lightweight, professional **local file management application** built
with **Python and Streamlit**.

File Ops Console provides a simple web-based interface for performing
common file operations directly from your local environment ---
including **creating, reading, renaming, appending, overwriting, and
deleting files**.

The application is designed with a clean console-style interface, clear
operation feedback, and an activity log that records file actions during
the current session.

------------------------------------------------------------------------

## 📌 Project Overview

File management is often performed through command-line tools or
operating-system file explorers. This project provides an alternative
approach by wrapping common file operations inside an easy-to-use
Streamlit interface.

The application is focused on four core operations:

-   **Create** --- Create a new text file and write content to it.
-   **Read** --- Read and preview the contents of an existing text file.
-   **Update** --- Rename a file, append content, or overwrite existing
    content.
-   **Delete** --- Permanently delete a file after explicit
    confirmation.

The application uses Python's built-in `pathlib` library for file-system
operations and Streamlit for the user interface.

------------------------------------------------------------------------

# ✨ Key Features

### 📄 Create Files

Create a new file by providing:

-   File name
-   File content

The application checks whether the file already exists before creating
it.

### 👁️ Read Files

Read an existing UTF-8 text file and display its contents directly
inside the application.

The application also handles common conditions such as:

-   Missing files
-   Invalid file paths
-   Non-file paths
-   UTF-8 decoding errors
-   Permission errors

### ✏️ Update Files

The update section provides three operations:

#### Rename

Rename an existing file while checking for:

-   Empty file names
-   Missing files
-   Existing destination names
-   Permission errors

#### Append Content

Add new content to the end of an existing file.

A newline is automatically added when the existing file already contains
data.

#### Overwrite File

Replace the existing contents of a file with new content.

### 🗑️ Delete Files

Delete an existing file with an explicit confirmation checkbox to help
prevent accidental deletion.

### 📋 Activity Log

The application maintains a session-based activity log showing:

-   Operation status
-   Timestamp
-   Action message

Successful, informational, and failed operations are visually
distinguished in the interface.

------------------------------------------------------------------------

# 🖥️ Application Interface

The application uses a clean desktop-style interface with:

-   Sidebar navigation
-   Operation-specific panels
-   File path indicator
-   Dark input fields
-   Activity console
-   Clear success and error feedback
-   Responsive Streamlit layout

------------------------------------------------------------------------

# 📸 Application Screenshots

## Create File

![Create File](Screenshots/Create%20File.png)

Create a new file and write content directly through the interface.

------------------------------------------------------------------------

## Read File

![Read File](Screenshots/Read%20File.png)

Read and preview the contents of an existing text file.

------------------------------------------------------------------------

## Update File

![Update File](Screenshots/Update%20File.png)

Rename files, append content, or overwrite existing file contents.

------------------------------------------------------------------------

## Delete File

![Delete File](Screenshots/Delete%20file.png)

Delete an existing file after confirming that the operation cannot be
undone.

------------------------------------------------------------------------

# 🛠️ Technology Stack

-   **Python**
-   **Streamlit**
-   **pathlib**
-   **datetime**
-   **HTML/CSS**
-   **Python Session State**

### Core Python Components

The application uses:

``` text
Streamlit
    ├── User Interface
    ├── Navigation
    ├── Forms & Inputs
    └── Session State

pathlib
    ├── File Creation
    ├── File Reading
    ├── File Renaming
    └── File Deletion

datetime
    └── Activity Log Timestamps
```

------------------------------------------------------------------------

# ⚙️ How It Works

``` text
                File Ops Console
                       │
          ┌────────────┼────────────┐
          │            │            │
        Create        Read        Update
          │            │            │
          │            │       ┌────┼────┐
          │            │       │    │    │
          │            │    Rename Append Overwrite
          │            │
          └────────────┼────────────┘
                       │
                     Delete
                       │
                       ▼
                Activity Log
```

------------------------------------------------------------------------

# 🚀 Installation & Setup

## 1. Clone the Repository

``` bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

## 2. Navigate to the Project

``` bash
cd YOUR_REPOSITORY
```

## 3. Install Dependencies

``` bash
pip install streamlit
```

## 4. Run the Application

``` bash
streamlit run FIleApp.py
```

The application will open in your default browser.

> If you rename the Python file, update the `streamlit run` command
> accordingly.

------------------------------------------------------------------------

# 📁 Project Structure

``` text
File-Ops-Console/
│
├── FIleApp.py
├── README.md
│
└── Screenshots/
    ├── Create File.png
    ├── Read File.png
    ├── Update File.png
    └── Delete file.png
```

------------------------------------------------------------------------

# 🧠 Skills Demonstrated

This project demonstrates practical experience with:

-   Python Programming
-   Streamlit Application Development
-   File System Operations
-   Object-Oriented File Handling Concepts
-   `pathlib`
-   Session State Management
-   Exception Handling
-   User Input Validation
-   Interactive UI Development
-   HTML/CSS Customization
-   Activity Logging
-   Local Application Development

------------------------------------------------------------------------

# 🔍 Error Handling

The application includes validation and error handling for common
file-operation scenarios.

Examples include:

-   Empty file names
-   Files that already exist
-   Files that do not exist
-   Paths that are not files
-   Permission errors
-   Operating-system file errors
-   Invalid UTF-8 text files
-   Delete operations without confirmation

This helps provide clear feedback instead of allowing common
file-operation failures to terminate the application.

------------------------------------------------------------------------

# 🔒 Local File Operations

File operations are performed through Python's local file-system APIs.

The application uses `pathlib.Path` to interact with files and does not
require a database for its core functionality.

Because the application operates on local paths, it should be run in an
environment where you understand which files and directories the
application can access.

------------------------------------------------------------------------

# 🎯 Project Goals

The primary goals of File Ops Console are to:

-   Build a practical Python application
-   Demonstrate local file-system operations
-   Practice Streamlit interface development
-   Implement robust input validation
-   Handle common file-operation errors
-   Provide clear user feedback
-   Create a reusable foundation for future file-management features

------------------------------------------------------------------------

# 🚀 Future Improvements

Possible future enhancements include:

-   📁 Directory browsing
-   🔎 File search
-   📊 File metadata and size information
-   📋 File listing and sorting
-   📦 Multiple-file operations
-   📤 File upload and download
-   🔐 Improved access controls
-   📝 Rich text editing
-   🌳 Folder navigation
-   📜 Persistent activity history
-   ⚙️ Configurable working directories

------------------------------------------------------------------------

# 👨‍💻 About the Developer

**Muhammad Faisal Jahangeer**

**Python Developer \| Data Analyst \| Data Science & AI/ML Enthusiast**

I enjoy building practical Python applications and data-driven projects
that solve real-world problems.

My areas of interest include:

-   Python Development
-   Data Analytics
-   Data Science
-   Machine Learning
-   Artificial Intelligence
-   Business Intelligence
-   Data Visualization
-   Automation

------------------------------------------------------------------------

# 🔗 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Muhammad%20Faisal%20Jahangeer-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-faisal-jahangeer-4b38393a8/)

------------------------------------------------------------------------

# ⭐ Support

If you find this project useful:

-   ⭐ Star the repository
-   🍴 Fork the project
-   💡 Share suggestions
-   🤝 Connect with me

------------------------------------------------------------------------

```{=html}
<p align="center">
```
**Python • Streamlit • File Management • Local Automation**

```{=html}
</p>
```
