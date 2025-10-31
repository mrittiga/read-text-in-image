# read-text-in-image

# 🖼️ Image Text Reader using PyTesseract (OCR)

This project extracts text from images using **Python** and **Tesseract OCR (Optical Character Recognition)**.  
It works on printed and handwritten text images, returning the detected text as plain text or saving it to a file.

---

## 🚀 Features
- Reads text from images (JPG, PNG, BMP, etc.)
- Supports printed and handwritten text
- Easy integration with Python scripts
- Option to save extracted text to `.txt` file
- Lightweight and open-source

---

## 🧩 Tech Stack
- **Python 3.8+**
- **PyTesseract** (Python wrapper for Google Tesseract OCR)
- **Pillow (PIL)** for image processing

---

## ⚙️ Setup Instructions

### 1️⃣ Install Tesseract OCR Engine
#### 🔹 Windows
1. Download the installer from:
   👉 [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki)
2. Install it and note the installation path (e.g., `C:\Program Files\Tesseract-OCR\tesseract.exe`)

#### 🔹 macOS
```bash
brew install tesseract
````

#### 🔹 Ubuntu / Linux

```bash
sudo apt update
sudo apt install tesseract-ocr
```

---

### 2️⃣ Install Python Dependencies

```bash
pip install pytesseract pillow
```

---

### 3️⃣ Project Structure

```
📁 image-text-reader/
├── images/
│   ├── sample1.jpg
│   ├── sample2.png
├── read_text.py
└── README.md
```

---


### 5️⃣ Run the Script

```bash
python read_text.py
```

🧠 Output will appear in the terminal and a `.txt` file will be created for each image:

```
sample1_output.txt
sample2_output.txt
```

---

## 🧪 Example Output

**Input:**
![sample image](c:/image/1.jpg)

**Output (Console):**

```
Hello World!
This text was extracted using PyTesseract OCR.
```

---

## 📚 Tips

* For better accuracy:

  * Use clear, high-resolution images.
  * Preprocess images (grayscale, thresholding, noise removal).
* You can detect text in different languages:

  ```python
  pytesseract.image_to_string(image, lang='eng+hin')
  ```

  *(Make sure the language data is installed for Tesseract.)*

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---


