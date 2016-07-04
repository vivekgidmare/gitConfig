# gitConfig
Git config on mac

##Go to home directory

    $ mv Downloads/git-completion.bash git-completion.bash
    $ mv Downloads/git-prompt.sh git-prompt.sh
    $ mv Downloads/bash_profile .bash_profile


Note : if bash profile is already added then copy+paste the content instead of moving whole file which may result into deletion of original one.

Sublime path to open it from terminal

    $ /Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl 

To add this path and to create shortcut for sublime 

    $ mv .bash_profile bash_profile
 
Open bash_profile in texteditor and add following line

    $ alias subl="/Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl"

After saving file do 

    $ mv bash_profile .bash_profile

## Config git

    $ git config --global core.editor "subl -n -w"
    $ git config --global push.default upstream
    $ git config --global merg.conflictstyle diff3

After this close termianl app and relaunch finder  (Hold alt-> right click on finder icon->relaunch)

Test sublime by following command

    $ subl .bash_profile
