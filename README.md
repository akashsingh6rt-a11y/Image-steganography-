# Image-steganography-
Image steganography using LSB(Least significant bit) technique
# Image Steganography using LSB

A Python Tkinter-based GUI tool to hide **text or files inside images** using the **Least Significant Bit (LSB)** steganography technique. The project also allows sending the encrypted image and password via Gmail SMTP.

---

## 📌 Features
- Hide **text** inside PNG/JPG images
- Hide **files** inside images (any format)
- Auto-generate password for decryption
- Sends encrypted image + password via email
- Extract hidden text or files from stego images
- Clean and modern Tkinter UI
- Debug console built into the app
- HTML Project Info page auto-generated

---

## 🛠️ Technologies Used
- Python 3
- Tkinter
- PIL (Pillow)
- EmailMessage + smtplib
- base64
- threading
- webbrowser

---

## 📁 Project Structure
```
Image-Steganography-LSB/
│
├── main.py                 # Main application file (your code)
├── requirements.txt        # Python dependencies
├── .gitignore              # Ignore unnecessary files
├── README.md               # Documentation
├── project_info.html       # Auto-generated HTML file
├── encrypted_image.png     # Output (ignored by git)
├── stego_password.txt      # Auto-generated (ignored)
└── DecryptedFiles/         # Extracted files directory
```

## ✅ Installation Instructions

### 1. Install Python Dependencies
```
pip install -r requirements.txt
```

### 2. Run the Application
```
python main.py
```

---

## 📌 Usage Guide

### 🔐 **Encrypting Data**
1. Click **Encrypt**
2. Select an image (PNG/JPG)
3. Choose **Text** or **File** mode
4. Enter your Gmail + App Password
5. Enter receiver's Gmail
6. Click **Encrypt**
7. Tool will:
   - Hide text/file in image
   - Generate unique password
   - Email encrypted image + password

---

### 🔓 **Decrypting Data**
1. Click **Decrypt**
2. Select the encrypted image
3. Enter the password you received
4. Tool extracts:
   - Hidden **text**, OR
   - **File** saved in `/DecryptedFiles/`

---

## 📧 Gmail SMTP Setup (Important!)
Google now requires **App Password** instead of real password.

Follow these steps:
1. Go to Google Account → Security
2. Enable **2-Step Verification**
3. Go to **App Passwords**
4. Create password for "App"
5. Use that password in this app

---

## 🧪 requirements.txt
```
tk
pillow
```

(If tkinter gives error, install via OS package manager)


