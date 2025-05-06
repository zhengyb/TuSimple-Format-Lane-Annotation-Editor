# TuSimple 2D Lane Annotation Tool

## Introduction

This project is a PyQt5-based 2D lane annotation tool following the TuSimple format. It supports multi-language interfaces and works on both Ubuntu and Windows systems.

## Usage (Recommended for General Users)

If you simply want to use the tool and do not plan to modify the code, it's recommended to use the precompiled `.exe` file.

### 1. Download Executable

Click the **Code** button in the upper right corner and select **Download ZIP** from the dropdown menu.

### 2. Run

Extract the ZIP file and double-click the `.exe` file to run the program.

## Running from Source (for Developers)

### 1. Install Python 3.10 (Recommended)

[Go to the official website to download Python 3.10](https://www.python.org/downloads/release/python-3100/)

### 2. Clone the Project and Enter the Directory

```bash
git clone https://github.com/WhosFish/TuSimple-Format-Lane-Annotation-Editor.git
cd TuSimple-Format-Lane-Annotation-Editor
git checkout win
```

### 3. Create and Activate a Virtual Environment (Optional)

```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 4. Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

## 3. Packaging Executable with PyInstaller

### 1. Install PyInstaller

```bash
pip install pyinstaller
```
### 2. Packaging Command (with Translation Files)

On a Windows system,
```bash
python -m PyInstaller --onefile --windowed --add-data "res\\res_cn.json;res" --add-data "res\\res_en.json;res" lane_label_tool.py
```

On a Ubuntu system,
```bash
pyinstaller --noconfirm --onefile --add-data "res:res" lane_label_tool.py
```

## 4. FAQ

TODO

## 5. Contact

If you have any questions, please submit an issue or contact the author.
