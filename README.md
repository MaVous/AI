Interactive Autonomous Learning AI with python (python2.7)
======================
This is an AI made in python.  
Since it is an autonomous learning type, you learn the words by yourself and combine the words you have learned to speak various things.

You can have them read the text as a candidate morpheme in advance, or you can have them learn from nothing based only on the sentence you entered.
 
use
------
### Interact with AI ###
Let's talk to the AI!  

Prepare an empty file called ''save/alice.txt''. Of course, this must be writable.  
Then move to the ''AI/'' folder and execute it like ''python Alice_AI.py''.  
'' save/alice.txt '' After loading '', ''Alice is logged in'', you will see something like '', so please enter something after ''You: ''.

There is no particular command for exiting, so please exit with ''Ctrl + C ''.

### Interact with AI ###
Next, let's make AI and AI talk!

Prepare two empty files: ''save/alice_2.txt'' and ''save/bob_2.txt''. Of course, it must be writable.
In the same way as before, execute python ai2ai.py '' in the ''AI/'' folder.
''Alice has logged in'' ''Bob has logged in'' If you get a message, the AIs will automatically talk to you!
 
### Read the file in advance ###
You can also have the file read in advance. In that case, it is necessary to decompose the file in which the sentence is written into morphemes.  
First of all, let's prepare a file (some of which I pulled from Aozora Bunko are in the ''text/ '' folder).

Run this as ''python Cutmorph.py [filename]'' next.  
Then ''save/m_[file name].txt'' (''~.txt.txt'' if it was originally a text file) will look like this.

After that, if you rename it like ''alice.txt'' or ''bob_2.txt'' as shown above and run the AI, it will automatically create your own conversation from the original sentence! It might be interesting to have your favorite characters imitate AI.

### Using Twitter Logs ###
If you want to use twitter logs to make the AI speak, it is faster to bring the logs from [twilog] (http://twilog.org/).  
You can download a CSV file with an appropriate character encoding from the twilog management page. Right now, everything is being developed in UTF-8, so please drop it in UTF-8.

Once the log file is ready, execute it as ''python text/non_number.py [log file]''. Unnecessary numbers are omitted from the log file and appear in the form of ''[log file].txt''.

After that, if you let the AI read this as ''python Cutmorph.py [[log file].txt]'' as above, it will be able to talk to you through the Twitter log.

Modification of the program
------- 

### Change the file to be loaded ###
The setting of the file to be read first is at the bottom if it is '' ./Alice_AI.py''

```python
if __name__ == "__main__":
    alice = AliceEngine("save/alice.txt") # ← here
    while True:
        input = raw_input("You：").decode('utf-8')
        if input == '': continue
        alice.mainloop(input)
```

''./ai2ai.py'', the

```python
AI.append(Alice_AI. AliceEngine("save/alice_2.txt",u"Alice")) # ← Here
AI.append(Alice_AI. AliceEngine("save/bob_2.txt",u"Bob")) # ← Here
```

Please change the file name appropriately.

-------
Have a fun AI life!  
Note that this program uses python 2.7.3. Please note that there are some parts that do not work in the python3.x series (in that case, please folk and modify it appropriately!). ）。

`` save/alice.txt ``
``AI/`` `` python Alice_AI.py ``  
`` save/alice.txt ```` AAliceさんがログインしました `` `` Yoou: ``

` Ctrl + C

`` save/alice_2.txt ``  `` save/bob_2.txt `` 
 ppython ai2ai.py
 python Cutmorph.py   

python text/non_number.py
python Cutmorph.py 

プロググラムの改変
------- 

### 読み込むファイルを変更する ###
最初に読み込ませるファイルの設定は`` ./Alice_AII.py ``であああれれれば一番下、

```python
if __name__ == "__main__":
    alice = AliceEngine("save/alice.txt") # ← ココです
    while True:
        input = raw_input("You：").decode('utf-8')
        if input == '': continue
        alice.mainloop(input)
```

``./ai2ai.py ``

```python
AI.append(Alice_AI.AliceEngine("save/alice_2.txt",u"Alice"))  # ← ココです
AI.append(Alice_AI.AliceEngine("save/bob_2.txt",u"Bob"))      # ← ココです
``` 

```python
if __name__ == "__main__":
    alice = AliceEngine("save/alice.txt") # ← ココです
    while True:
        input = raw_input("You：").decode('utf-8')
        if input == '': continue
        alice.mainloop(input)
```

``./ai2ai.py``であれば真ん中辺りの

```python
AI.append(Alice_AI.AliceEngine("save/alice_2.txt",u"Alice"))  # ← ココです
AI.append(Alice_AI.AliceEngine("save/bob_2.txt",u"Bob"))      # ← ココです
```

のファイル名を適当に変更して下さい。


Interactive Autonomous Learning AI with python (python2.7)
======================
This is an AI made in python.  
Since it is an autonomous learning type, you learn the words by yourself and combine the words you have learned to speak various things.

You can have them read the text as a candidate morpheme in advance, or you can have them learn from nothing based only on the sentence you entered.
 
use
------
### Interact with AI ###
Let's talk to the AI!  

Prepare an empty file called ''save/alice.txt''. Of course, this must be writable.  
Then move to the ''AI/'' folder and execute it like ''python Alice_AI.py''.  
'' save/alice.txt '' After loading '', ''Alice is logged in'', you will see something like '', so please enter something after ''You: ''.

There is no particular command for exiting, so please exit with ''Ctrl + C ''.

### Interact with AI ###
Next, let's make AI and AI talk!

Prepare two empty files: ''save/alice_2.txt'' and ''save/bob_2.txt''. Of course, it must be writable.
In the same way as before, execute python ai2ai.py '' in the ''AI/'' folder.
''Alice has logged in'' ''Bob has logged in'' If you get a message, the AIs will automatically talk to you!
 
### Read the file in advance ###
You can also have the file read in advance. In that case, it is necessary to decompose the file in which the sentence is written into morphemes.  
First of all, let's prepare a file (some of which I pulled from Aozora Bunko are in the ''text/ '' folder).

Run this as ''python Cutmorph.py [filename]'' next.  
Then ''save/m_[file name].txt'' (''~.txt.txt'' if it was originally a text file) will look like this.

After that, if you rename it like ''alice.txt'' or ''bob_2.txt'' as shown above and run the AI, it will automatically create your own conversation from the original sentence! It might be interesting to have your favorite characters imitate AI.

### Using Twitter Logs ###
If you want to use twitter logs to make the AI speak, it is faster to bring the logs from [twilog] (http://twilog.org/).  
You can download a CSV file with an appropriate character encoding from the twilog management page. Right now, everything is being developed in UTF-8, so please drop it in UTF-8.

Once the log file is ready, execute it as ''python text/non_number.py [log file]''. Unnecessary numbers are omitted from the log file and appear in the form of ''[log file].txt''.

After that, if you let the AI read this as ''python Cutmorph.py [[log file].txt]'' as above, it will be able to talk to you through the Twitter log.

Modification of the program
------- 

### Change the file to be loaded ###
The setting of the file to be read first is at the bottom if it is '' ./Alice_AI.py''

```python
if __name__ == "__main__":
    alice = AliceEngine("save/alice.txt") # ← here
    while True:
        input = raw_input("You：").decode('utf-8')
        if input == '': continue
        alice.mainloop(input)
```

''./ai2ai.py'', the

```python
AI.append(Alice_AI. AliceEngine("save/alice_2.txt",u"Alice")) # ← Here
AI.append(Alice_AI. AliceEngine("save/bob_2.txt",u"Bob")) # ← Here
```

Please change the file name appropriately.

-------
Have a fun AI life!  
Note that this program uses python 2.7.3. Please note that there are some parts that do not work in the python3.x series (in that case, please folk and modify it appropriately!). ）。
