Smart Note Organizer
Overview
This application acts as your personal academic editor. It takes messy text files, PDFs, and images (like photos of diagrams or slides) and uses Artificial Intelligence to reorganize them into a professional Study Guide.

The program automatically categorizes your notes, creates tables for comparative data, and exports everything into a clean Microsoft Word document (.docx).

Prerequisites
To use this program, you must have:

A Google Account (Gmail).

Python installed on your computer.

How to Install Python
Go to python.org/downloads.

Download the latest version for Windows.

Run the installer.

CRITICAL STEP: On the first screen of the installer, check the box that says "Add python.exe to PATH". If you skip this, the program will not run.

Click Install Now.

Installation Instructions
Step 1: Download the Application
Click the green Code button on this GitHub page.

Select Download ZIP.

Go to your Downloads folder.

Right-click the ZIP file and select Extract All... then click Extract.

You will now have a normal folder containing the program files.

Step 2: Install Dependencies
This step installs the necessary tools for reading PDFs and creating Word documents. You only need to do this once.

Open the folder where you extracted the files.

Click into the address bar at the very top of the window (where the folder path is displayed).

Type cmd and press Enter. A black command window will appear.

Type the following command exactly and press Enter:

pip install -r requirements.txt

Wait for the installation to complete (the text will stop scrolling).

Step 3: Get Your Free AI Key
This program uses Google's AI to read your notes. You need a "Key" (like a password) to use it.

Go to this website: aistudio.google.com/app/apikey

Sign in with your Google/Gmail account.

Click the blue button that says Create API key.

If asked, select Create API key in new project.

A box will pop up with a long string of random letters and numbers. Click the Copy button next to it.

Step 4: Configure the App
Now you need to put that key into the program settings.

Go back to your application folder.

Find the file named config.json.

Right-click on config.json and select Open with > Notepad.

You will see text that looks like this: "GEMINI_API_KEY": "YOUR_API_KEY_HERE".

Highlight the text YOUR_API_KEY_HERE.

Paste your new key (Right-click > Paste).

Make sure the key is still inside the quotation marks "".

Click File > Save.

Close Notepad.

How to Run the Program
Open the application folder.

Click the address bar at the top, type cmd, and press Enter.

Type the following command and press Enter:

python main.py

The application window will open.

Usage Guide
Add Files: Click the "Add Files" button to select your text notes, PDF documents, or images.

Instructions: (Optional) In the text box, type specific instructions for the AI (e.g., "Focus on vocabulary" or "Create a timeline").

Categorize & Compile: Click the button to start processing. The status bar will indicate progress.

Export: Once the notes appear in the right-hand window, click "Export DOCX" to save them as a Word document.

Troubleshooting
"Python is not recognized...": This error means you did not check the "Add to PATH" box during installation (Prerequisites section). Please uninstall Python and reinstall it, ensuring that box is checked.

"No module named...": This means Step 2 (Install Dependencies) did not finish correctly. Please try running that step again.

The program closes immediately: This usually means the config.json file has a mistake. Make sure you did not accidentally delete one of the quotation marks " when pasting your key.
