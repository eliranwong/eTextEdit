# eTextEdit
Extensible Text Editor; built with prompt toolkit

Originally a simple text editor created by Jonathan Slenders
Source: https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/full-screen/text-editor.py

Modified and Enhanced by Eliran Wong:
* added file and clipboard utilities
* added regex search & replace feature
* added key bindings
* added handling of unasaved changes
* added dark theme and lexer style
* support stdin, e.g. echo "Hello world!" | python3 eTextEdit.py
* support file argument, e.g. python3 eTextEdit.py <filename>
* support plugins (forthcoming)

eTextEdit repository:
https://github.com/eliranwong/eTextEdit

# Screenshots

<img src="github.com/eliranwong/eTextEdit/assets/25262722/c7a564ce-2e3c-4913-8210-52e259545044"/>

<img src="https://github.com/eliranwong/eTextEdit/assets/25262722/7703f138-e56e-4c6f-84fc-4abe768f161a"/>

# Download

> pip install --upgrade etextedit

# Usage

To launch eTextEdit:

> etextedit

To open a text file, e.g. test.txt:

> etextedit test.txt

To pipe in a text string, e.g. "Hello World!":

> echo "Hello World!" | etextedit

To append a file, e.g. test.txt, with a text string, e.g. "Hello World!":

> echo "Hello World!" | etextedit test.txt

# Key Bindings

escape + m: toggle menu

control + k: help

control + q: quit

control + a: select all

escape + a: deselect all

control + c: copy

control + v: paste

control + x: cut

control + z: undo

control + i: insert spaces

control + f: find

escape + f: clear i-search highlights

control + r: find & replace

control + l: go to line

control + d: delete

control + n: new file

control + o: open file

control + s: save file

control + w: save as file

## Navigation

escape + a: go to beginning of document

escape + z: go to end of document

escape + b: go to beginning of current line

escape + e: go to end of current line
