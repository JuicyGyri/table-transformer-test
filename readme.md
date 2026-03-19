# **🌟 Table Extraction Tool: OCR & Computer Vision for Structured Data**
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/Sudhanshu1304/table-transformer)
[![Stars](https://img.shields.io/github/stars/Sudhanshu1304/table-transformer.svg)](https://github.com/Sudhanshu1304/table-transformer/stargazers)
[![Watchers](https://img.shields.io/github/watchers/Sudhanshu1304/table-transformer.svg)](https://github.com/Sudhanshu1304/table-transformer/watchers)

## Overview

Table Transformer is an advanced open-source tool that leverages state-of-the-art OCR and computer vision techniques to extract structured tabular data from images. It is ideal for enhancing LLM preprocessing, powering data analysis pipelines, and automating your data extraction tasks.

## Features
- 📊 **Automatic Table Detection**: Effortlessly detect tables in images.
- 📝 **OCR-based Document Processing**: Extract text with high accuracy.
- 🧠 **Integrated Models**: Seamlessly combine OCR and table detection models.
- 💾 **Flexible Export Options**: Export data as DataFrame, HTML, CSV, and more.

---

## **Tool Overview**

<div align="center">

<!-- First Row -->
<img src="images/image1.png" alt="Image upload" width="45%" style="margin: 10px;">
<img src="images/image2.png" alt="Table detection & extraction" width="45%" style="margin: 10px;">

<!-- Second Row -->
<img src="images/image3.png" alt="Table in HTML format" width="45%" style="margin: 10px;">
<img src="images/image4.png" alt="Table exported as CSV" width="45%" style="margin: 10px;">

</div>

---

## **Open-Source Tools Used**
- **[PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)**: For text extraction.
- **[Hugging Face Table Detection](https://huggingface.co/foduucom/table-detection-and-extraction)**: For table structure detection.

---

## **Installation**

### **Prerequisites**
- [Python 3.8+](https://www.python.org/downloads/)
- [Conda](https://docs.conda.io/en/latest/miniconda.html) (Miniconda recommended)
- [Git](https://git-scm.com/downloads)

### **Setup**

1. **Clone the Repository**

   Clone **this** repository to your local machine:

   ```bash
   git clone https://github.com/JuicyGyri/table-transformer-test.git
   cd table-transformer-test
   ```

2. **Create and Activate Conda Environment**

   Create a new conda environment and activate it:

   ```bash
   conda create --name myenv python=3.12.7
   conda activate myenv
   ```

3. **Install Dependencies**

   **Option A – Install from `requirements.txt` (recommended):**

   ```bash
   pip install -r requirements.txt
   ```

   **Option B – Install packages individually:**

   Install PaddlePaddle:

   ```bash
   python -m pip install paddlepaddle==3.0.0rc1 -i https://www.paddlepaddle.org.cn/packages/stable/cpu/
   ```

   Install PaddleOCR and remaining packages:

   ```bash
   pip install paddleocr
   pip install ultralytics pandas streamlit
   ```

### **Project Structure**
```
project/
├── src/
│   ├── streamlit_app.py       # Streamlit application
│   ├── table_creator/
│   │   └── processing.py      # Core processing logic
│   ├── models/
│   │   └── text.py            # table detection and text recognition
│
├── requirements.txt           # Dependencies
├── README.md                  # Project documentation
└── .gitignore                 # Git ignore configuration
```

### **Usage**
Run the Streamlit app to interact with the tool:

```bash
streamlit run src/streamlit_app.py
```

---

## **Using This Tool in VS Code — Step by Step**

Follow these steps to set up and run the tool directly inside Visual Studio Code.

### **Step 1 — Install the Python Extension**

1. Open VS Code.
2. Click the **Extensions** icon in the left sidebar (or press `Ctrl+Shift+X` / `Cmd+Shift+X` on Mac).
3. Search for **Python** (published by Microsoft) and click **Install**.

> This extension enables Python IntelliSense, debugging, and interpreter selection inside VS Code.

---

### **Step 2 — Open the Project Folder**

1. In VS Code, go to **File → Open Folder…** (or press `Ctrl+K Ctrl+O` / `Cmd+K Cmd+O` on Mac).
2. Navigate to the `table-transformer-test` folder you cloned in the installation step and click **Select Folder**.

You should now see the project files in the VS Code Explorer panel on the left.

---

### **Step 3 — Select the Conda Python Interpreter**

1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) to open the Command Palette.
2. Type **Python: Select Interpreter** and press `Enter`.
3. Choose the interpreter that corresponds to your `myenv` conda environment — it will look something like:
   ```
   Python 3.12.7 ('myenv': conda)
   ```

> If `myenv` does not appear, make sure you created it with `conda create --name myenv python=3.12.7` and that Conda is on your system PATH.

---

### **Step 4 — Open the Integrated Terminal**

1. In VS Code, go to **Terminal → New Terminal** (or press `` Ctrl+` ``).
2. A terminal panel will open at the bottom of the editor.
3. Activate your conda environment:
   ```bash
   conda activate myenv
   ```

---

### **Step 5 — Run the Streamlit App**

In the integrated terminal, run:

```bash
streamlit run src/streamlit_app.py
```

VS Code's terminal will display output similar to:

```
  You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  Network URL: http://192.168.x.x:8501
```

VS Code may also prompt you to **Open in Browser** — click it to open the app directly.

---

### **Step 6 — Use the App**

Once the app opens in your browser:

| Step | Action |
|------|--------|
| 1 | Click **Browse files** (or drag-and-drop) to upload a PNG, JPG, or JPEG image that contains a table. |
| 2 | Wait for the tool to detect and highlight the table with a green bounding box. |
| 3 | Switch between the **Raw Data** and **Enhanced Data ⭐** tabs to inspect the extracted table. |
| 4 | Copy the generated **HTML table** snippet from the code block shown under each tab. |
| 5 | Click **Download Raw Data** or **Download Enhanced Data ⭐** to save the results as a CSV file. |

To stop the app, go back to the VS Code terminal and press `Ctrl+C`.

### **Contributions**
Contributions are welcome! Please fork the repository and submit a pull request with your improvements or new features.

### **License**
This project is licensed under the MIT License.

---

## **Connect with Us**
Stay updated and connect for any queries or contributions:

- **GitHub**: [Sudhanshu1304](https://github.com/Sudhanshu1304)
- **LinkedIn**: [Sudhanshu Pandey](https://www.linkedin.com/in/sudhanshu-pandey-847448193/)
- **Medium**: [@sudhanshu.dpandey](https://medium.com/@sudhanshu.dpandey)

---

## **Support**
If you find this tool useful, please consider giving it a ⭐ on GitHub. Your support is greatly appreciated!

Happy Extracting!
