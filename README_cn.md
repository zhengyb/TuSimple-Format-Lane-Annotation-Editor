# TuSimple 2D 车道线标注工具

## 简介

本项目是一个基于 PyQt5 的 TuSimple 2D 车道线标注工具，支持多语言界面，适用于 Ubuntu 和 Windows 系统。

## 使用方式（推荐普通用户）

如果你只是想用工具，并不想修改代码，推荐直接使用打包好的 `.exe` 文件。

### 1. 下载可执行文件

点击右上角的Code，从下拉菜单中下载Zip。

### 2. 运行
解压文件，双击.exe文件运行程序。

## 从源代码运行（开发者）

### 1. 安装 Python 3.10（推荐）

[前往官网下载 Python 3.10](https://www.python.org/downloads/release/python-3100/)

### 2. 克隆项目并进入目录

```bash
git clone https://github.com/WhosFish/TuSimple-Format-Lane-Annotation-Editor.git
cd TuSimple-Format-Lane-Annotation-Editor
git checkout win
```

### 3. 创建虚拟环境并激活（可选）

```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 4. 安装依赖库

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

## 三、用 PyInstaller 打包可执行文件

### 1. 安装PyInstaller

```bash
pip install pyinstaller
```
### 2. 打包命令（包含翻译文件）

```bash
python -m PyInstaller --onefile --windowed --add-data "res\\res_cn.json;res" --add-data "res\\res_en.json;res" lane_label_tool.py
```

## 四、常见问题

TODO

## 五、联系方式

如有问题请提交 issue 或联系作者。
