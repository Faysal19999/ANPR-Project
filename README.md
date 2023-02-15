# ANPR Project

A Group project centered around creating an interactive GUI to scan Licence plates 
## Dependencies
* Python 3.7+
* OpenCV
* Numpy
* PyQt5
* imutils
* setuptools 40.8.0
* pywin32
* Google Tesseract OCR 5.0.0 alpha


## Installation ( Dependencies ) 

To install all Python library requirements, in the command-line run:
```bash
pip install -r requirements.txt
```

## Installation Tesserract
### Windows
Download and install Tesseract 5.0.0 alpha from [link](https://github.com/UB-Mannheim/tesseract/wiki "here")

### Linux

```
sudo apt install tesseract-ocr
sudo apt install libtesseract-dev
```

## Running the script
### 3 Simple ways to run the program.

1. The first way is to launch *scanner.py* through command line, type in:
```
python scanner.py [image.jpg/png]
```
2. The second way is to launch *eval.py*, type in:
```
python eval.py
```

This is used to evaluate the performance of the system. It goes through every image in the dataset, saves the results into the *finalplates* directory and outputs the evaluated performance.

The third way is to use the GUI, type in:
```
python gui.py
```
This will launch a fully functional GUI.

**Ensure you have installed all the dependencies first and have completed the config, otherwise this system will not work properly.**

## Configuration

### Using the GUI

1. Launch gui.py.

2. This will automatically create a configuration file

3. In the settings group, you will need to locate the tesseract.exe file.

4. Then you are given an option to save the images. Check it if you wish to do so.

5. You are also given the choice of showing processing steps. Check it if you wish to do so.

### Using command-line

1. Launch the program using *scanner.py* or *eval.py* first.

2. Open *config.json*

3. Enter the file url of *tesseract.exe* into the *tesseract_url* variable. If you cannot find *tesseract.exe*, ensure it is installed first.

4. If you wish to view the steps the program has taken to get the result, set *show_steps* to *true*, otherwise leave it as *false*.

5. If you wish to save the resultant images, set *save_images* to *true*, otherwise leave it as *false*.

6. Launch the program again and you should get the results.

## Dataset
A dataset has been provided in *example_dataset* folder.

### Using VirtualEnv
It is recommended to use a python virtual environment for this project, as it installs quite a few additional pip packages.
You can find documentation for VirtualEnv [link](https://virtualenv.pypa.io/en/latest"here")


