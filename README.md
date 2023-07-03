# Random Password Generator in Python
This program will create a random password containing 3 words (one uppercase), 2 numbers, and 1 symbol. Got it? Let's go!!!

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
from random import choice
from colorama import init
from termcolor import colored

init() #Makes termcolor work on windows

# Setting the variables
Words_File = open("words.txt","r")
Symbols_File = open("symbols.txt","r")
Words = []
Symbols = []
Numbers =  ["1","2","3","4","5","6","7","8","9","0"]
```
**Step 2:** Find all the words in "words.txt" and put them into a list:
```python
#Putting all the words in words.txt into a list
for line in Words_File:
  Words.append(line.strip())
```
**Step 3:** Find all the symbols in "symbols.txt" and put them into a list:
```python
#Putting all the symbols in symbols.txt into a list
for line in Symbols_File:
  Symbols.append(line.strip())
```

**Step 4:** Create a random password using the lists we created:
```python
#Creating the password
Password = choice(Words).upper() + choice(Words) + choice(Words) + choice(Numbers) + choice(Numbers) + choice(Symbols)
print(colored("Your random password is ","blue") + colored(Password, "aqua"))
```

Here is all the code put together:
```python
# Importing the modules
from random import choice
from colorama import init
from termcolor import colored

init() #Makes termcolor work on windows

# Setting the variables
Words_File = open("words.txt","r")
Symbols_File = open("symbols.txt","r")
Words = []
Symbols = []
Numbers =  ["1","2","3","4","5","6","7","8","9","0"]

#Putting all the words in words.txt into a list
for line in Words_File:
  Words.append(line.strip())

#Putting all the symbols in symbols.txt into a list
for line in Symbols_File:
  Symbols.append(line.strip())

Password = choice(Words).upper() + choice(Words) + choice(Words) + choice(Numbers) + choice(Numbers) + choice(Symbols)
print(colored("Your random password is ","blue") + colored(Password, "aqua"))
```
See the project files for symbols.txt and words.txt.

To run this program in a Command Prompt/Terminal, enter this line of code to make sure the terminal doesn't close as soon as the program is done:
```python
input("Press enter to close")
```
or add a while True around the print like this:
```python
while True:
  print(colored("Your random password is ","blue") + colored(Password, "aqua"))
  input("Press enter to generate a new password")
```

Have fun with this program. Please note this program is under a MIT licence. 

