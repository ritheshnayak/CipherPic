# CipherPic
Secure your images with ease using CipherPic, a powerful tool to encrypt and decrypt your sensitive photos.             Protect your data with advanced encryption and ensure only you can access it.
# Video Demo
[![YouTube](https://github.com/user-attachments/assets/f0f939eb-0a27-4fcc-8169-2bc75722cbc1)](https://www.youtube.com/watch?v=BYDeOWHE7bs)
## File Structure

CipherPic By Rithesh  
│  
├── node_modules (Not pushed to GitHub, will be installed via npm)  
├── src  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── index.js ___ _( Main Electron application file )_   
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── encrypt.js ___ _( Encryption logic )_  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── decrypt.js  ___ _( Decryption logic )_  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── gui.js  ___ _( IPC handlers and GUI interactions )_  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── preload.js ___ _( Preload script for Electron )_  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── index.html  ___ _( HTML for the GUI )_  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    ├── style.css  ___ _( CSS styling for the GUI )_  
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    └── background.png  ___ _( Background image for the GUI )_  
│  
├── package.json  ___ _( Project metadata and dependencies )_  
└── package-lock.json ___ _( Dependency tree and versions )_
## Installation Options

You have two options to use CipherPic:

### Option 1: Download the Installer
1. Download the latest installer from the [Releases](https://github.com/ritheshnayak/CipherPic/releases/tag/v1.0.0) page.
2. Run the installer and follow the on-screen instructions.
3. Once installed, launch CipherPic from your applications menu.

### Option 2: Download the Code and Run Manually
If you prefer to run the application from source, follow these steps:  
## Necessary Installation and Prerequisites
1. Ensure your system is set up for html, css, js and node.js
2. Get the code down and organised as per file structure
3. Install Dependencies : run command : `'npm install'`. This will install all required packages as specified in `package.json`. The `node_modules` directory will be created during this process.
## How to Use
1. **Start the Application** :
    ```bash
    npm start
    ```
    A electron `GUI` based application will open.
2. **Encrypt an Image**:
    - Click the "Encrypt" button in the GUI.
    - Select the image file to encrypt.
    - Choose the output file names for the encrypted image and the encryption key.
    - The application will encrypt the image and save the files.

3. **Decrypt an Image**:
    - Click the "Decrypt" button in the GUI.
    - Select the encrypted image file and the key file.
    - Choose the output file name for the decrypted image.
    - The application will decrypt the image and save the file.
## Tools, Technologies, APIs, and Modules Used
- **HTML, CSS** : For the graphical user interface.
- **JavaScript** : Core programming language for both frontend and backend logic. In Frontend handles user interactions in `index.html` via script tags. In backend used to Implement the core encryption/decryption logic in `encrypt.js` and `decrypt.js`, and manages IPC communication in `gui.js`.
- **Electron** : Framework to create the desktop application.
- **Node.js** :  JavaScript runtime for backend operations.  
                - Module System : Organizes the application into separate modules (index.js, encrypt.js, decrypt.js, etc.).  
                - File System Operations : Reads and writes image and key files using the fs module.  
                - Package Management : Manages dependencies like jimp and cli-alerts.  
- **Jimp** : Image processing library.
- **cli-alerts** : For displaying alerts in the terminal. Informs if encryption successful or failed.


### Key Changes:
1. Added a new section titled **Installation Options**.
2. Provided two clear options:
   - **Option 1**: Download the installer for a straightforward installation process.
   - **Option 2**: Download the code and run it manually for users who prefer working with the source code.
3. Included detailed instructions for both options to ensure clarity and ease of use.

This structure ensures that users of all technical backgrounds can choose the method that best suits their needs.


