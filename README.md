# Test for MkDocs

## 1. Installation

### 1.1. Installing Python and pip
#### Download Python:
https://www.python.org/downloads/

#### Installing pip:
If you already have Python installed, pip is most likely already installed too. However you may need to upgrade it to the latest version:
```
pip install --upgrade pip
```
If you need to install pip, [download the get-pip.py script](https://bootstrap.pypa.io/get-pip.py). *(Right click > "save as..." to download the .py file).* Then, run the script:

**Linux/MacOS:**

ℹ️ *Debian-based Linux distributions may need to use `python3` (or whatever version of Python you have installed) instead of just `python`. Optionally, you can install the `python-is-python3` package so you can use `python` as an alias of `python3`.*
```
python get-pip.py
```
**Windows:**

ℹ️ *`python` works too on Windows*
```
py get-pip.py
```

### 1.2. Installing MkDocs using pip:

First, it's recommended to install and contain Python packages per project using a virtual environment (venv).

Start by creating a new virtual environment (locate yourself in the root directory of the project before executing the command):
```
python -m venv .mynewvenv
```

ℹ️ *`.mynewvenv` being the name of your virtual environment, you can name it whatever you want. I personally like making the directory hidden too.*

Now activate it by running:

```
# Linux/macOS
source .mynewvenv/bin/activate

# Windows (Command Prompt)
.\.mynewvenv\Scripts\activate.bat

# Windows (Powershell)
.\.mynewvenv\Scripts\Activate.ps1
```
You should now be inside the virtual enviroment. You can exit the virtual environment at any time by running:
```
deactivate
```
And enter it again executing the previous command.

Lastly, install MkDocs and the [Material](https://squidfunk.github.io/mkdocs-material/) theme using pip. The dependencies are listed in `requirements.txt`, so you just need to run:
```
pip install -r requirements.txt
```

Alternatively, you can install them individually:
```
pip install mkdocs
pip install mkdocs-material
```
