---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Set up Atom for Python on Mac
Atom is an open source text editor developed by engineers at GitHub. A great text editor is at the core of writing and documenting good code. In this How-To guide you will learn how to set up Atom on a Mac to make coding in Python easy and streamlined.

## Prerequisites

To install Atom and begin customizing it for a Python on environment, you'll need the following:
- Internet connection

## What will be covered?

1. Installing Atom
2. Installing packages
3. Customizing Atom's default settings

## What packages will we install?

| Package | Function |
|  ------ | -------  |
| Script package| Runs programming languages within Atom|
|Autocomplete package | Explain this |
| Mini Map package | Explain this |
| Python-autopep8 package | Explain this |
| Python Linter-flake 8 | Checks for errors in the code base |



## Install Atom

Go to http://atom.io/ and follow the installation instructions.

## Disable default welcome windows
Two welcome windows appear every time Atom is opened.


To disable this feature, uncheck the `Show welcome guide when opening Atom` box.
> Result: The default welcome window will now not appear each time Atom is opened.

<img alt="video" src="/assets/remove-welcome-page.gif" width="500" height="375">

## Install packages
Installing packages are the heart of customizing and configuring Atom.

Install packages by following these steps:

1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type the package name into the search bar.

> Result: You are now familiar with the process for installing packages.

<img alt="video" src="images/install-package-v4.gif" width="500" height="375">

## Install Script package
The Script package allows you to run a variety of programming languages within Atom.

1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type `Script` name into the search bar.

4. Exit *Settings* windows after installing.

> Result: You can now run Python within Atom.

<img alt="video" src="images/install-Script.gif" width="500" height="375">

## Change Python version to run scripts

Script will use the default Python version on your Mac, which is Python 2. If you've downloaded Python 3, you can use Python 3 to run your scripts.
To download Python 3, go here: (https://www.python.org/)

1. Click `Atom` > `Preferences` > `Packages`.

2. Type `Script` into the search bar.
4. Click `Settings`.
5. Click `View Code`.
1. Click `Scripts` > `lib` > `Grammars` > `python.coffee`.
1. Under *Selection Based* and *File Based* type a '3' after *python*.
1. Save the file by pressing <kbd>cmd-s</kbd> or `File` > `Save`.
1. Close Atom and the reopen it.

> Result: You're now using Python 3 to run scripts in Atom

<img alt="video" src="images/change-to-python3.gif" width="500" height="375">

 > Result: You can see the Python version in the console output.

<img alt="video" src="images/change-to-python3-result.gif" width="500" height="375">


For a more in depth video on this process: [Change Python 2 to Python 3 in Atom](https://discuss.atom.io/t/how-can-i-switch-python-version-for-script/24036/14)

## Change hotkeys

There are many ways to run a Python script, but the easiest way is to use hot keys.

The default hotkey is <kbd>cmd-i</kbd>. I think <kbd>cmd-l</kbd> is a little easier.

1. Click `Atom` > `Preferences` > `Packages`.

2. Type `Script` into the search bar.
4. Click `Settings`.
5. Click `View Code`.
1. Click `Scripts` > `keymaps` > `scripts.cson`.
1. Change the letter after `cmd` to your preference.
1. Click `File` > `Save`.
1. Close Atom and then restart it.

> Result: Your new hotkey will run your script.

<img alt="video" src="images/change-hotkeys.gif" width="500" height="375">


Here is a list of all the ways to run scripts in Atom

| Command                    | macOS                               | Linux/Windows               | Notes                                                                         |
|:---------------------------|:------------------------------------|:----------------------------|:------------------------------------------------------------------------------|
| Script: Run                | <kbd>cmd-i</kbd>                    | <kbd>shift-ctrl-b</kbd>     | If text is selected a "Selection Based" is used instead of a "File Based" run |
| Script: Run by Line Number | <kbd>shift-cmd-j</kbd>              | <kbd>shift-ctrl-j</kbd>     | If text is selected the line number will be the last                          |
| Script: Run Options        | <kbd>shift-cmd-i</kbd>              | <kbd>shift-ctrl-alt-o</kbd> | Runs the selection or whole file with the given options                       |
| Script: Run with profile   | <kbd>shift-cmd-k</kbd>              | <kbd>shift-ctrl-alt-b</kbd> | Runs the selection or whole file with the specified profile                   |
| Script: Close View         | <kbd>esc</kbd> or <kbd>ctrl-w</kbd> | <kbd>esc</kbd>              | Closes the script view window                                                 |
| Script: Kill Process       | <kbd>ctrl-c</kbd>                   | <kbd>ctrl-q</kbd>           | Kills the current script process


## Change console font output size and color

Changing the console font output size and color makes it easier to view your console results.

1. Click `Atom` > `Preference`.

1. Click `Themes`.
1. Click `Your stylesheet`.
1. Scroll to the bottom and paste this code in.
```
.script-view .line {
  font-size: 16px;
}
.script-view .panel-body pre {
  color: white
}

.script-view .-linked-path {
  color: red
}
```
1. Click `File` > `Save`.

1. If you want to change the color or font size, change the values next to `font-size` and `color`.

> Result: Your console output font size and color have changed.

<img alt="video" src="images/change-console-output.gif" width="500" height="375">

## Install file icon package

Having recognizable icons associated with files makes scanning a large repository easy.

1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type `File icon` name into the search bar and press `Return`.
1. Click `Install`.

> Result: Icons are not associated with your file extensions.

<img alt="video" src="images/file-icons.gif" width="500" height="375">




## Install minimap package

Minimap provides a zoomed-out view of your file in the upper-right of Atom's screen. This is nice when working with long files in order to move between parts of the code quickly.


1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type `minimap` name into the search bar and press `Return`.

1. Click `Install`.

1. Choose between *Jedi* and *Kite* (I'll choose Jedi since there's no signup.)
> Result: Minimap is now installed, making it easy to navigate long files.

<img alt="video" src="images/minimap.gif" width="500" height="375">

## Install autocomplete package

Autocomplete offers a variety of function and method suggestions when writing code. These suggestions can increase your coding speed.


1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type `autocomplete python` into the search bar and press `Return`.

1. Click `Install`.

1. You'll be prompted to choose between *Jedi* and *Kite* (I'll choose Jedi since there's no signup.)

> Result: Autocomplete is now installed, which can help increase your coding speed.

<img alt="video" src="images/autocomplete.gif" width="500" height="375">

## Install the predawn theme

Themes determine both the look of user interface looks and  color of the coding syntax. You can change your themes based on the UI or the syntax. We'll change the syntax theme to predawn, a slightly muted color scheme. Explore themes to find one you enjoy.

The predawn theme can be installed by doing the following:

1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Themes` next to the search bar.

3. Type `predawn` into the search bar and press `Return`.

1. Click `Install` for predawn-syntax.

1. Click `Themes` on the left navigation bar.

1. Click `Syntax Theme` drop down and choose `Predawn`.

> Result: Your syntax colors have changed and are now based on the predawn stylesheet.

<img alt="video" src="images/predawn.gif" width="500" height="375">

## Install Python-autopep8 packages

The Python autopep8 package formats your Python code according to the Pep 8 standards.

You can learn about Pep 8 here: https://www.python.org/dev/peps/pep-0008/

1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type `pep8` into the search bar and press `Return`.
2. Choose `python autopep8`

1. Click `Install`.

2. Click `Settings` and scroll to the bottom.
2. Copy the line `pip install autopep8`.
3. Open a terminal window.
    - [Learn to open a terminal window](https://www.youtube.com/watch?v=zw7Nd67_aFw)

2. Copy and paste the pip install line `pip install autopep8`. If the error `pip command not found` appears, type `pip3 install autopep8`.

3. Exit terminal window after the installation.
2. Click the box `Format On Save` in the settings pane. This formats your files to the Pep 8 standards every time you save.  

> Result: Your Python files will be formatted according to the Pep 8 standards every time you save.

<img alt="video" src="images/pep8.gif" width="500" height="375">

## Install linter-flake8

Linter-flake8 shows errors in your base, which helps debugging before you run your code.

1. Click  `Atom` > `Preferences` > `Install`.

2. Click `Package` next to the search bar.

3. Type `linter flake 8` into the search bar and press `Return`.
2. Choose `linter-flake8`

1. Click `Install`.

1. Click `Yes` on the pop-up menus as they appear to install dependencies.

2. Click `Settings` and scroll to the bottom.

2. Copy the line `pip install flake8`.

3. Open a terminal window.
    - [Learn to open a terminal window](https://www.youtube.com/watch?v=zw7Nd67_aFw)

2. Copy and paste the pip install line `pip install flake8`. If the error `pip command not found` appears, type `pip3 install autopep8`.

3. Exit terminal window after the installation.

> Result: You can now see the error messages by clicking the orange '!' in the bottom-left.

<img alt="video" src="images/linter-flake8.gif" width="500" height="375">

## Customize Atom's default settings

There are a number of editor settings that can be changed.

We'll make the following changes to the editor.

| Setting | Functionality |
| ------- | ------------- |
| Font size | Changes font size |
| Scroll past end | Allows scrolling past the end of the document |
| Show indent guide | Shows which indents line up in code blocks|
| Tab length | Sets default tab spacing |


1. Go to `Preferences` > `Editor`
2. Scroll down and make the following changes:
    - Change `Font Size` to `16`.
    - Click the box `Scroll Past End`.
    - Click the box `Show Indent Guide`.
    - Change `Tab Length` to `4`.


> Result: Your editor will be changed according to those values.

<img alt="video" src="images/editor-1.gif" width="500" height="375">

## Push to GitHub from inside Atom

If you use GitHub to host your code, Atom makes it easy to make commits, push, and pull.

1. Click `View` > `Toggle GitHub Tab`

1. Click the `1 file` icon in the bottom-right corner. You can now see the familiar window stage, commit, and push and pull.

> Result: You can now use GitHub within Atom

<img alt="video" src="images/github.gif" width="500" height="375">


> End
