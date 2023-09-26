# SAFE SPACE
## Installation Instruction
To get the code..

1. Cloning the repository:
  ```bash
  https://github.com/Paul-Ngigi/safe-space.git
  ```
2. Move to the folder and install requirements
  ```bash
  cd safe-space
  python -m venv virtual
  linux - source virtual/bin/activate  | windows - virtual/Scripts/activate.ps1
  pip install -r requirements.txt
  ```

3. Fix ModuleNotFoundError: No module named 'flask._compat'  
  Click on Ctrl + the path to the virtual file. Change this line of code
  ```
  Where:

from ._compat import text_type on original flask-script file

to :

from flask_script._compat import text_type
```

3. Running the application
  ```bash
  python manage.py server
  ```
Open the application on your browser `http://127.0.0.1:5000`.
