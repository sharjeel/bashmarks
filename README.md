### This is a fork to add support for aliases in Bashmarks. Bashmarks is a shell script that allows you to save and jump to commonly used directories. Now supports tab completion. 

## Install

1. git clone git://github.com/huyng/bashmarks.git
2. make install
3. source **~/.local/bin/bashmarks.sh** from within your **~.bash\_profile** or **~/.bashrc** file

## Shell Commands

    s <bookmark_name> - Saves the current directory as "bookmark_name"
    a <alias> <cmd>   - Saves alias command
    g <bookmark_name> - Goes (cd) to the directory associated with "bookmark_name"
    p <bookmark_name> - Prints the directory associated with "bookmark_name"
    d <name>          - Deletes the bookmark or alias
    l                 - Lists all available bookmarks
    
## Example Usage

    $ cd /var/www/
    $ s webfolder
    $ cd /usr/local/lib/
    $ s locallib
    $ l
    $ g web<tab>
    $ g webfolder
    $ a ll ls -l
    $ ll 

## Where Bashmarks are stored
    
All of your directory bookmarks and aliases are saved in a file called ".sdirs" in your HOME directory.
