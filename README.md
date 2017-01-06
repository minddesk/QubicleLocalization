# QubicleLocalization
All language files and templates for the localization  of the Qubicle Voxel Editor.

If you like to help translating Qubicle into other languages:

1. First of all: you rock, I appreciate your help! Oh, and there are also rewards (see below)
2. Please have a look at the guidelines for some very few text formation rules
3. If you are not familiar with GitHub you can also send your translation file directly to me

## The Language File Structure

All ini files are regular Windows ini files, which work like this:

There are section headers like *[MENU_FILE]* and loads of lines with key/value pairs like *FILE = File*.
I use sections only for organization puposes, and to give you an idea where to find a word. All sections starting with MENU are menu entries, so everything found under [MENU_FILE] are menu entries of the File menu. All sections starting with DIALOG are words found in pop up dialogs.
Please note that keys only appear once in the ini files. E.g. the key WIDTH is used many times in Qubicle but has to be declared only one time. So, not all words found in a dialog are necessarily declared in its section, it might be declared elsewhere.

To make the tranlation process easier, keys are descriptive. So, most of the time you will see something like this: WIDTH = Width. In the German translation that line would be WIDTH = Breite. 

**IMPORTANT** Never, ever change a key, because it will lead to unwanted results in Qubicle. 

## How To Proceed

Download the ini files

## Text Formatting Guidelines

There's only one rule: all words have to start with a capital:

* *Create Empty Matrix* is correct
* *Create empty Matrix* is wrong

The only exception to this rule: all messages found in the section **[MESSAGES]** have to be written normally:

* *Are you sure you want to continue?* is correct
* *Are You Sure You Want To Continue?* is wrong
