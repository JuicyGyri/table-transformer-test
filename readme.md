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
- Python 3.8+
- Conda
- [Git](https://git-scm.com/downloads) (to clone the repository)

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
