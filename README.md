# generate email script

# Requirements
```
MacOS
bash
Terminal skills
```

# bash
Lets see if bash is installed.  Type this into your Terminal app.  If it shows you a version in the output, then you have bash installed.
```
echo $BASH_VERSION
```

If bash isn't installed, you should be able to install it with brew.  But you'll need to first install brew.  
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
If you have any problems, refer to the brew website for help.
https://brew.sh


Install bash
```
brew install bash
```

Using Finder (file manager) app, copy the directory containing the email script into your Downloads folder.
If the directory name IS 'affari_buildingmd-email-sig' then use the Terminal to find that script with this command:
```
cd ~/Downloads/affari_buildingmd-email-sig/
```
If affari_buildingmd-email-sig is NOT the name of that directory, then you will need to use this command and replace [NAME_OF_THE_DIRECTORY] with the directory name.
```
cd ~/Downloads/[NAME_OF_THE_DIRECTORY]
```


# Edit file
You'll need a code editor to edit script files since using a basic text editor could introduce unwanted formatting into the code.  I would recommend using Sublime, but any code editor will do.
https://www.sublimetext.com
This is a free version, so it will ask you to upgrade once in a while.  You can just click cancel and continue using Sublime.  

Now that you have a code editor installed, right click the file called 'people_list_to_generate.txt' and open that with your code editor.  At the top of this file is a placeholder line, showing the exact format of each employee you will add below.  So copy that first line as many times as you need for each employee.  You will notice that each field is separated by a ';'.  
```
_TEST USER;Company + Job Title;123-456-7890;Email Address;
```
Now replace each line with a different persons information.  Once that is done, save the file and go back to the Terminal app.  Paste this command into the Terminal
```
bash _do_all_sigs.bash
```
If all went well, you should have several HTML files in the directory called 'sigs'

## Troubleshooting
If you get an error while running the bash command, send us the error, and the version of bash that you do have installed with:
```
echo $BASH_VERSION
```
If you have an issue where the last person on the list doesn't get generated, open up the 'people_list_to_generate.txt' file with your code editor, and make sure there is an empty line at the end of the file.

------------

## If this is all too much trouble and you would rather just edit some html files, then feel free to do that with the code editor.  Just duplicate the template.html file and search for these placeholders to edit them.
```
NAME_PLACEHOLDER
EMAIL_PLACEHOLDER
O_NUM_PH
COMPANY_JOBTITLE
```
