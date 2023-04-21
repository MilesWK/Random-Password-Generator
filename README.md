# Random-Password-Generator-Python
This is a program that will create a 3 word (one uppercase), 2 number, and 1 symbol password in Python! All program in this repository is under a MIT License. 

# Setup Instructions
**Step 1:**
Download the folder called "Project Files." This will have the two text documents required for this program

**Step 2:**
Create a new python file in the "Project Files" folder. This will make it so you don't need to call the files by their full directory when accesing them.

# The Program
**Step 3:**
Setup the variables and import the modules:
```python
import random
Numbers = ["1","2","3","4","5","6","7","8","9","0"]
Words = [] 
Symbols = []
```
**Step 4:**
Put all the symbols and words into two lists:
```python
Words_File = open("words.txt","r") # Open the words.txt file and make it readable ("r")
Symbols_File = open("symbols.txt","r") # Open the symbols.txt file and make it readable ("r")

# This script will find all the words in the Words_File variable and put them into the Words list:

for line Words_File:
  Words.append(line)

# This script will find all the words in the Symbols_File variable and put them into the Symbols list

for line Symbols_File:
  Words.append(line) 
```
Now we have all the words in Words.txt in a list and all the symbols in Symbols.txt in another list.

**Step 5:**
Create the code that prints the random password:

This program will create the random password with 3 words (one uppercase), 2 numbers, and 1 symbol:
```python
while True: 
  Password = str(upper(Random.choice(Words))) + str(Random.choice(Words)) + str(Random.choice(Words))  + str(Random.choice(Numbers)) + str(Random.choice(Numbers)) + str(Random.choice(Symbols)))
  print("Your random password is ' + Password)
  input('Press ↵ to get a new password or press "Ctrl + C" to quit the program.')
```
Put all the code together to get this final program:
```python
import random
Numbers = ["1","2","3","4","5","6","7","8","9","0"]
Words = [] 
Symbols = []
Words_File = open("words.txt","r") # Open the words.txt file and make it readable ("r")
Symbols_File = open("symbols.txt","r") # Open the symbols.txt file and make it readable ("r")

# This script will find all the words in the Words_File variable and put them into the Words list:

for line Words_File:
  Words.append(line)

# This script will find all the words in the Symbols_File variable and put them into the Symbols list

for line Symbols_File:
  Words.append(line) 
while True: 
  Password = str(Random.choice(Words).upper()) + str(Random.choice(Words)) + str(Random.choice(Words))  + str(Random.choice(Numbers)) + str(Random.choice(Numbers)) + str(Random.choice(Symbols)))
  print("Your random password is ' + Password)
  input('Press ↵ to get a new password or press "Ctrl + C" to quit the program.')
```
Save and run the program. You should get this in the console:
```cmd
Your random password is HAPPYmangopeach12!
Press ↵ to get a new password or press "Ctrl + C" to quit the program.
```
Of course, you most likely won't HAPPYmangopeach12! as your password, but you get the idea!
# Support
If you have any issues with this program, contact me at [https://replit.com/@MilesWK/MilesWK-V3](https://replit.com/@MilesWK/MilesWK-V3?v=1)
