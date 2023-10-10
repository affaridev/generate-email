# generate email script

# Requirements
```
MacOS
bash
Terminal skills
```

# Install bash
Lets see if bash is installed.  Type this into your Terminal app.  If it shows you a version in the output, then you have bash installed.
```
echo $BASH_VERSION
```

If bash isn't installed, you should be able to install it with brew.  But you'll need to first install brew.  Here are the details on that, if this 1 command doesn't work.
https://brew.sh
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Install bash
```
brew install bash
```

Using Finder (file manager) app, copy the directory containing the email script into your Downloads folder.
Use the Terminal to find that script with this command:
```
cd ~/Downloads/[NAME_OF_THE_DIRECTORY]
```

# Edit the script files
You'll need a code editor to edit script files since using a basic text editor could introduce unwanted formatting into the code.  I would recommend using Sublime, but any code editor will do.
https://www.sublimetext.com
This is a free version, so it will ask you to upgrade once in a while.  You can just click cancel and continue using Sublime.

