# What are we doing here???

In the first lessson we will

- get ready to collaborate. We will do so using GIT.
- Install everything needed
- Create a tiny first program

I will not tell you how to do most of your tasks.

- because I'm lazy
- because there are already tons and tons of tutorials how to do those things.
- and finally because I would like to see how little hand-holding you can handle. Programming is 5% coding 90% googling and 5% figuring out what to name your variables. Better get used to it right from the start:-P

(But seriously message me with any troubles if Google/chatGpt fails)

## GIT

You know Github. But do you know git?

Git is a technology that allows us to share data. (Usually coding projects)

[Download git](https://git-scm.com/downloads), install it and add your github credentials(name/password) to it so that you can edit this repo.

Adding the credentials is a part of installation process I hope. If not, google or hit me up;-)


### Git bootcamp

A **repository** (or repo for short) is one "project" that is shared using git.
This repository is called Rychlokurz.

You can **clone** this **repository** - ie. download it from Github (**origin**) into your computer.

After you do that, you can:

- **pull** changes from the **origin**. (ie. Update your repo so that it matches the newest version on github)
- **push** changes to the **origin**. (ie. upload your work to github.)
- create a **branch** (We won't do that in this lesson but it is a important concept we might explore in the future;-)

The "changes" I mentioned above are called **commits**. They basically hold information about what changed from the previous commit (mostly just creating/editing/deleting files).

That should be enough for this lesson. Git is a bit more complex than that but this is all we need to know for now.

All of the magic of git is stored in .git folder. (You might not see it as Windows hides folders starting with a dot by default)

### Tortoise GIT

Git itself is controlled through command line.

For instance, to clone this repo you would open cmd, navigate to the folder you want to clone the repo to and enter
```
git clone https://github.com/0rbit3r/Rychlokurz.git
```

But with Tortoise git installed you get to control git through GUI/context menu (right click menu).

To clone the repo using Tortoise you can simply go to the folder you want, right click, click clone and paste the url.

Tortoise is not necessary but I recommend [downloading](https://tortoisegit.org/) it as using cmd might not feel comfortable for you (yet:-P).

## Vscode

Vscode is your future text editor, IDE, lover and favourite power tool. It can be used for pretty much anything. (Provided you have the right extentions installed.)

[Download](https://code.visualstudio.com/) it, install it and open this Repo in it (either by **File>Open folder** or drag the Rychlokurz folder onto the vscode icon) This will allow the vscode to treat the folder as a project (and more importantly a git repo).

Once opened, go to extentions and install these:

- Markdown all in one
- Python

## Markdown

Markdown is what this file is written in. (extention **.md**).
It's easy to style and that's why it's widely used in Repositories. (I even use it for note-taking.)

You can open the .md file in vscode. If you have **Markdown All in one** extention installed, you can press **ctrl+shift+p** (This openes vscodes universal action prompt) and search for **Markdown: open preview to the side** to see both the raw file and the rendered result prettily side by side.

This markdown code...

```
# Second-level header

**Some bold text** with some *italic* info here and there... blah blah blah... this is still the first paragraph.

To add a paragraph, you can put two new lines.

- to make a list you use dashes
- don't forget to new lines before and after the list
  - lists can also be inside of other lists!
    - crazy right?

- [ ] This is a special list that is rendered with checkboxes
- [x] This task is finished!
```
...
renders like this:

# Second-level header

**Some bold text** with some *italic* info here and there... blah blah blah... this is still the first paragraph.

To add a paragraph, you can put two new lines.

- to make a list you use dashes
- don't forget to new lines before and after the list
  - lists can also be inside of other lists!
    - crazy right?
    - Just put an extra tab before the dash

- [ ] This is a special list that is rendered with checkboxes
- [x] This task is finished!

## Python

[Download Python 3](https://www.python.org/downloads/)

Python is a programming language you might have heard of. In context of this lesson, I will only tell you this:

Much like git, you can run python in command line. If you navigate to the 01_Repository folder and run `python3 HelloWorld.py` the file will execute and work.

But it's easier to use vscode (or any other IDE) and just press F5 to run the opened file. That's what the Python extention is for (among many many other things).

Go on and try to run the **HelloWord.py** in vscode. You should see `Hello world!` in console if it works. 

Then modify the **PersonalHello.py**.

I recommend watching a python "hello world" tutorial. (Any one you like)

## TODO

- [x] Install and configure the necessary software
  - [x] Visual studio Code with extentions
    - [x] Python (vscode extention)
    - [x] Markdown All in one (vscode extention)
  - [x] Python 3
  - [x] Git
    - [x] Add Github credentials to Git settings
    - [x] Send your Github name to me so I can give you edit rights
  - [ ] Tortoise Git (Optional but allows us to use git iwthout command line)

---

- [x] Clone this repository
- [x] Create a new markdown file **I_did_it.md** inside **01_Repository**, commit the changes and push them to the origin.

----

- [x] Run **HelloWorld.py**
- [x] Finish **PersonalHello.py** (and commit + push to origin)