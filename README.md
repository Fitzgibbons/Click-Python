# Click-Python
Automation Service for macOS that allows one click execution of python files through the context menu.

## Usage:
This workflow should be put in the Services directory found under [User_Name]/Library/Services. Once present here it will appear when a file is right clicked in Finder. This only works for files ending in ".py". The name of the workflow is what will appear in the context menu, and macOS tends to delay any changes from appearing, so make sure the name you want is there before you move the file into Services

Note: This version uses the command line argument "python", which is usually used for python2, but you can change that command to whatever python interpreter you would like. For example the standard command line argument for python3 is "python3", so you could change the 5th to last line to:
```
tell application "Terminal" to do script ("python3 " & pythonFile) in front window
```
