# QubicleLocalization
All language files and templates for the localization  of the Qubicle Voxel Editor.

You like to help translating Qubicle into other languages? Awesome, you rock, I appreciate your help! Please follow the guidelines below, it's easy but will require some time. There are a total of 1000 lines that need to be translated. It's a lot of work, that's why I want to reward you for your help as described in the last section.

THANK YOU!
Tim

PLEASE NOTE:
* Of course you can do this with the free Demo found on Steam: http://store.steampowered.com/app/454550
* **Windows is required for the following workflow.**
* **Only languages that can be displayed with ISO-8859-1 are currently supported**. E.g. Chinese and Russian are currently not supported. For a list of supported languages visit https://en.wikipedia.org/wiki/ISO/IEC_8859-1 There's still some magic required to support other alphabets, but I will try to find a solution. If you like to provide an unsupported language, that would help me to find that solution. Thanks!

## How To Create A New Translation

1. Update to Qubicle 3.1 or higher
2. Download *custom_ui_translation.ini* and *custom_help_translation.ini* and copy them to documents/Qubicle 3.0/
3. Start Qubicle, select *Custom* from the *Language* menu and quit Qubicle again
4. Translate values in the custom ini files
5. Start Qubicle to test the changes you made
6. Send the files along with the language code (e.g. en for english) to support[at]minddesk[dot]com

## How To Correct Parts Of An Existing Translation

1. Update to Qubicle 3.1 or higher
2. To fix the German version, download *de_ui.ini* and *de_help.ini* 
3. Make your changes
4. If you like to test what you have done, copy the files to documents/Qubicle 3.0/, rename them to *custom_ui_translation.ini* and *custom_help_translation.ini* and proceed as described above
5. If you are familiar with Git make a pull request. Otherwise send the corrected files to support[at]minddesk[dot]com. Please describe what changes you made

## The Language File Structure

There are two separate files, one for the ui and one for the quick help found in the status bar. All ini files are regular Windows ini files, which work like this:

There are section headers like *[MENU_FILE]* and loads of lines with key/value pairs like *FILE = File*.
I use sections only for organization puposes, and to give you an idea where to find a word. All sections starting with MENU are menu entries, so everything found under [MENU_FILE] are menu entries of the File menu. All sections starting with DIALOG are words found in pop up dialogs.
Please note that keys only appear once in the ini files. E.g. the key WIDTH is used many times in Qubicle but has to be declared only once. So, not all words found in a dialog are necessarily declared in its section, it might be declared before.

To make the tranlation process easier, keys are descriptive. So, most of the time you will see something like this: WIDTH = Width. In the German translation that line would be WIDTH = Breite. 

**IMPORTANT** Don't change a key, only its value. If Qubicle does not find a certain key it will revert the language to english

## Text Formating Guidelines

There's only one rule: in the ui.ini files all words have to start with a capital:

* *Create Empty Matrix* is correct
* *Create empty Matrix* is wrong

The only exception to this rule: all messages found in the section **[MESSAGES]** have to be written normally:

* *Are you sure you want to continue?* is correct
* *Are You Sure You Want To Continue?* is wrong

There are no real rules for the help.ini files. As a best practice I tried to not address the user directly. So you won't find a *you* or *your* in the files. 

## Rewards

Rewards will be sent out when the translation is released.

#### Submit a new translation of both ui.ini and help.ini:

* Get a free Qubicle Indie Edition license key
* Get mentioned on Qubicle's start screen in the *Thank You* section
* Get mentioned in the Help > About dialog

#### Submit a new tranlation for either ui.ini or help.ini

* Get a free Qubicle Basic Edition license key + a DLC of your choice
* Get mentioned in the Help > About dialog

#### Correct parts of an existing language file

* Get mentioned in the Help > About dialog
