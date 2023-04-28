# Random Password Generator in Python
This program will create a random password containing 3 words (one uppercase) 2 numbers, and 1 symbol. Got it? Let's go!!!

# Setup
**Setup Step 1:** Download the "Project Files" folder.

**Setup Step 2:** Use pip to download the "termcolor" package and the "colorama" packages:

**In your computer's console:**
```console
pip install termcolor
pip install colorama
```

**Setup Step 3:** Create a python program __IN THE PROJECT FILES FOLDER__.

We are done with setup: now it is time to program!!!
# The program!
**Step 1:** create the variables and import the modules
```python
# Importing the modules
import random
from colorama import init
from termcolor import colored

# Setting the variables
Words_File = open("words.txt","r")
Symbols_File = open("symbols.txt","r")
Words = []
Symbols = []
```
**Step 2:** Find all the words in "words.txt" and put them into a list:
```python
for line in Words_File:
  Words.append(line.strip())
```
