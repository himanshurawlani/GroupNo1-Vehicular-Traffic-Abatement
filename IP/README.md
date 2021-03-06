## Setup
```
$ virtualenv venv        #ensure virtulenv is installed else install it using pip
$ venv/Scripts/activate  #getting into virtual environment
(venv) $ pip install -r requirements.txt
```

## Virtual Environment
A `virtual environment` ensures no other python package not in our project interferes with the code. We can even keep track of all required packages in this way.
 - Always activate the virtual environment on opening the terminal in this folder, to see `(venv)` prefixed to the prompt
```
 $ venv/Scripts/activate  #getting into virtual environment
```
 - To leave the virtual environment type the following
```
(venv) $ deactivate
```

## Python Packages
In case of adding a new package using `pip install` it should be reflected in `requirements.txt` file. Do it using
```
(venv) $ pip freeze > requirments.txt
```
Ensure at all times that packages are installed being inside the virtual environment.

## Filter out traffic and roads from the SS images
```
(venv) $ python main.py
```

## JSON
 - JSON dataset are stored inside `json` folder which is ignored inside `.gitignore` to never commit it to GitHub
 - Images are picked up from the `ss gen/images` folder and the same hierarchy of folders is maintained on the output JSON files as well