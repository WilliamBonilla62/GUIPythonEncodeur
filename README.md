# GUIPythonEncodeur
This project is a graphical user interface (GUI) to automate the control of the encoder.

This GUI was developped with Python3 and Qt5.
____
# Table of content
- [1-Installation procedure](#1-Installation-procedure)
 - [1.1-Get the code](#11-Get-the-code)
 - [1.2-Libraries](#12-Libraries)
   - [1.2.1-Needed Libraries](#121-Needed-Libraries)
   - [1.2.2-Install Libraries](#122-Install-Libraries)
  - [1.3-Software](#13-Software)
    - [1.3.1-Needed Software](#131-Needed-Software)
    - [1.3.2-Install Software](#132-Install-Software)
 - [1.4-Modify the Graphical User Interface](#14-Modify-the-Graphical-User-Interface)
    - [1.4.1-Qt Design](#141-Qt-Design)
    - [1.4.2-Translate .UI to .PY](#142-Modify-the-Graphical-User-Interface)
____
# 1-Installation procedure
## 1.1-Get the code

To install the software on raspbian virtual Desktop:
- open terminal with **`Ctrl+Alt+T`**
- go in the local folder where you want to install
```bash
cd /PATH
```
>example of PATH **`/home/pi/Documents`**

- clone the repo [**`GUIPythonEncodeur`**](https://github.com/WilliamBonilla62/GUIPythonEncodeur.git)
```bash
git clone https://github.com/WilliamBonilla62/GUIPythonEncodeur.git --recursive
```
the **`--recursive`** command is important it makes a direct link between the repo and all the submodules inside. If you don't put the command or download the file directly all the submodules will be empty.\
\
Also if you want to be sure to have the last version of the submodule use this command:
```bash
git submodule update --remote
```
## 1.2-Libraries
### 1.2.1-Needed Libraries
- library pyqt5Screenshot from 2020-12-16 22-51-20
### 1.2.2-Install Libraries
#### library phidget installation
Open a terminal write down these two command :
```bash
sudo apt-get install python3-pyqt5
sudo apt-get install python3-pyqt5.qtsql
```
## 1.3-Software
### 1.3.1-Needed Software
- Qt5 assitant
- Qt5 Designer
- Qt5 Linguist
### 1.3.2-Install Software
Open a terminal write down this :
```bash
sudo apt-get install qttools5-dev-tools
```
## 1.4-Modify the Graphical User Interface
### 1.4.1-Qt Design
Open the file with Qt5 Designer **Encoder_Control_GUI.ui** in the submodule **GUI_QT_ONLY** inside the **QT** folder. Do the modification needed and save the file.
### 1.4.2-Translate .UI to .PY
To convert a .ui to a .py you will to run this command:
```bash
pyuic5 -x Encoder_Control_GUI.ui -o Encoder_Control_GUI.py
```
By converting the .ui into a .py you are now able to add code (functions) to the GUI you have designed/modified.
