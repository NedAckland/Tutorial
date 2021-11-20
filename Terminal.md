
# Mac Terminal

_can be a pain to learn but once you do it makes life much easier - me_


Folder -> Directory

### The Main Commands

|Command|What is?|How to use|
|:---:|:---|:---|
| cd | change directory | cd _Downloads/movies_ 
| ls | list items in current directory | ls
| mkdir| make directory | mkdir _nameOfNewDirectory_
| touch| create file | touch _newFileName_
| sudo | run command as root/admin | sudo _command_
| pwd | print working directory | pwd
| code  | open vscode | code _filename/fullstop_  .  will open vscode project in current directory 


----

## How to traverse the terminal

When you open your terminal you are inside your user directory(folder) by default. 

Type **pwd** then press enter. you will see something similar to this:

_/Users/you_

Type **ls** and press enter. you will see all the directories(folders) & files inside your user directory

As an example create a direactory called _test_.

To do this type **mkdir test** and press enter.

If you once again type **ls** and press enter you should see the _test_ directory you created in the list.

To enter this new directory, type **cd test** and press enter.

**pwd** should now show this:

_/Users/you/test_

**ls** will display nothing because this is a new directory you have just created.

To create a file in this directory. Type **touch newfile.js** and press enter.

**ls** will now display _newfile.js_ 

typing **cd** with no target directry will take you back to the user directory where you started.

you can travel down multiply directories by adding them to the cd command like this: **cd Downloads/movies/new**.
## challenge 

- create a folder called _lessons_ **mkdir lessons**
- move into _lessons_  **cd lessons**
- create another directory called _lesson_1_ **mkdir lesson_1**
- move into _lesson_1_  **cd lesson_1**
- create a file called fundamentals.js  **touch fundamental.js**
- open vscode from the terminal  **code .**


_there is a faster way of doing this challenge but we should cover the basics first_