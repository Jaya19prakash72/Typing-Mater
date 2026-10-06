TYPING MASTER - LOCAL HOST PROJECT
====================================

This project is based on the uploaded Typing Master HTML application.

REQUIREMENTS
------------
- Windows 8.1 / Windows 10 / Windows 11
- Python 3.x
- VS Code (recommended)
- A modern browser such as Chrome or Edge

No external Python packages are required.

RUN METHOD 1: PYTHON LOCAL SERVER
---------------------------------
1. Extract this ZIP.
2. Open the extracted folder in VS Code.
3. Open Terminal in VS Code.
4. Run:

   py --version

   If that works, run:

   py -m http.server 8000

   If "py" does not work, try:

   python --version
   python -m http.server 8000

5. Open your browser and visit:

   http://localhost:8000

6. Click index.html if the directory page appears.

STOP SERVER
-----------
Press CTRL + C in the VS Code terminal.

RUN METHOD 2: VS CODE LIVE SERVER
----------------------------------
1. Open the project folder in VS Code.
2. Install the "Live Server" extension.
3. Right-click index.html.
4. Select "Open with Live Server".

IMPORTANT DATA NOTE
-------------------
The application currently stores users, passwords, score history,
unlocked levels, login state, and dark-mode preference in browser
localStorage. This means the data is stored only in that browser on
that computer. It is NOT a real server-side database/authentication
system.

CURRENT FEATURES FROM THE UPLOADED FILE
---------------------------------------
- Login / create account
- Password check for existing local accounts
- 5 progressive typing levels
- Level locking/unlocking
- 60-second test timer
- WPM calculation
- Accuracy calculation
- Error count
- Character-by-character correct/wrong highlighting
- Score history
- Dark mode
- Responsive/mobile layout
- Automatic completion when the sentence is fully typed

FILES
-----
index.html       Main application
README.txt       Localhost setup instructions
assets/          Reserved for future images/assets

TROUBLESHOOTING
---------------
If "python is not recognized":
- Check Python installation.
- In VS Code terminal run: py --version
- Then use: py -m http.server 8000

If port 8000 is busy:
- Use another port, for example:
  py -m http.server 8080
- Then open:
  http://localhost:8080

If old data causes login/testing problems:
- Open browser Developer Tools -> Application -> Local Storage
- Clear the local storage for localhost.
