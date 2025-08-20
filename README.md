# 🚉 Automatic Tatkal Ticket Booking using Selenium & OCR  

## 📌 Project Overview  
This project automates the **Tatkal ticket booking process** on the IRCTC platform using **Selenium WebDriver** for browser automation and **Tesseract OCR** for CAPTCHA recognition.  
It reduces the time taken to fill forms manually and increases the chances of securing a Tatkal ticket during the highly competitive booking window.  

---

## 🔑 Key Features  
- **Automated Login** – Uses saved credentials to log in quickly.  
- **Train Search & Selection** – Automatically enters journey details (source, destination, date, class).  
- **Passenger Autofill** – Pre-fills passenger details and contact information from a config file.  
- **Captcha Recognition (ML Model)** – Uses **Tesseract OCR** with preprocessing (OpenCV + Pillow) to solve captchas.  
- **One-Click Booking** – End-to-end flow from login to booking confirmation with minimal user interaction.  

---

## 🛠️ Tech Stack  
- **Python**  
- **Selenium WebDriver** (automation)  
- **Tesseract OCR (via pytesseract)** (captcha recognition)  
- **OpenCV & Pillow** (image preprocessing)  

---

## ⚡ Why Tesseract OCR?  
IRCTC captchas are text-based but slightly noisy.  
- Preprocessing (thresholding, binarization, noise removal) improves recognition accuracy.  
- Tesseract OCR is lightweight, open-source, and easily integrates with Python.  

---

## 🚀 Workflow  
1. Launch Selenium WebDriver → Open IRCTC login page.  
2. Autofill credentials → Capture CAPTCHA image.  
3. Preprocess CAPTCHA → Run **Tesseract OCR** → Extract text.  
4. Submit login form → Autofill passenger & train details.  
5. Confirm booking → Complete payment manually (automation limited by RBI guidelines).  

---

## 🔮 Future Improvements  
- Replace Tesseract with **Deep Learning-based CAPTCHA Solvers (CNNs, CRNNs)** for higher accuracy.  
- Add **proxy rotation** and **headless browser mode** for stealthier automation.  
- Build a **GUI wrapper** for non-technical users.  

---


---

## ⚠️ Disclaimer  
This project is for **educational purposes only**. Automating IRCTC booking may violate their terms of service.  
Use responsibly and at your own risk.  

---

