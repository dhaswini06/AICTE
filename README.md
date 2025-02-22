Secure Data Hiding in Images Using Steganography
A Python-based project that combines AES encryption with LSB steganography to securely hide messages within images.

Features
AES-Encrypted Steganography – Ensures double-layer security for hidden messages.
Least Significant Bit (LSB) Encoding – Hides data imperceptibly within an image.
Password-Protected Decryption – Prevents unauthorized access to the embedded data.
Supports PNG Images – Maintains image quality without compression loss.
Cross-Platform Compatibility – Works on Windows.
How It Works
Encryption & Embedding:

The message is encrypted using AES (CBC mode) before being embedded.
Encrypted data is hidden inside the Least Significant Bits (LSB) of the image pixels.
A password-derived key (SHA-256) ensures secure encryption.
Extraction & Decryption:

The program extracts hidden data from the image.
The retrieved encrypted message is decrypted using AES with the correct password.
If the password is incorrect, decryption fails, ensuring data confidentiality.
Installation
METHOD-1
Installation Guide

Step 1️: Install Python

Ensure Python 3.8+ is installed. You can download it from:

Python Official Website: https://www.python.org/downloads/

                          https://pypi.org/project/opencv-python/
Step 2️: Install Jupyter Notebook

Open a terminal or command prompt and run:

pip install jupyter
Step 3️: Install Required Libraries

Run the following command in the terminal or in Jupyter Notebook (using a code cell):

pip install opencv-python cryptography numpy
Step 4️: Launch Jupyter Notebook

After installation, start Jupyter Notebook using:

jupyter notebook
Then, navigate to the project folder and open the Jupyter Notebook (.ipynb) file.

METHOD-2
Prerequisites
Ensure you have Python 3.8+ installed. Then, install the required libraries:

pip install opencv-python cryptography numpy
Usage
Hiding a Secret Message in an Image
python AESSteganography.py
Enter the message and password when prompted.
The encoded image will be saved as Encryptedmsg.png.
Extracting the Hidden Message
python AESSteganography.py
Provide the encrypted image and password to retrieve the original message.
Technologies Used
Python – Core programming language.
OpenCV (cv2) – Image processing & pixel manipulation.
Cryptography (AES-CBC – Encrypts messages securely.
SHA-256 Hashing – Generates a strong key from a password.
NumPy – Efficient array handling for images.
Future Enhancements
Support for JPEG & BMP formats
GUI-based tool for ease of use
AI-based steganalysis resistance
Mobile app integration
