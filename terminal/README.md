# Terminal Directory

This directory contains terminal profiles and other information useful for operating the terminal application on macOS

### Useful Tips & Commands

  - Switching profile of current Terminal tab/window
    - Open Inspector with `cmd + i` or `right click` and select `Show Inspector`
    - From **Profile** tab of Inspector select a different terminal profile configuration
    - This will change the current tab/window, if multiple tabs are present in the same window this will only change the current tab.
    - New tabs will open terminal profiles based on the current tab/window.

  - Adding or appending content to files from terminal
    - useful when adding new path related commands to shell files
    - Use the double caret `>>` to ppe the output from a command into a text file
    - ex: `echo 'export PATH="$(yarn global bin):$PATH"' >> ~/.zshrc` will add `export PATH="$(yarn global bin):$PATH"` as a command at the bottom of your zshrc file

  - Prompting an open terminal window to re-read a shell file
    - use the `source` command to tell terminal to reread files
    - ex: `$ source ~/.zshrc`

  - Using a shell commands standard output as a value for other scripts
    - Enclosing commands in `$(…)` or backticks `` ` … ` `` can be used to pass the standard output of one command as the input or argument for another
    - This is known as Command Substitution 
      - [see ref ->](https://pubs.opengroup.org/onlinepubs/9699919799/utilities/V3_chap02.html#tag_18_06_03)
      - [see more ->](https://unix.stackexchange.com/a/126928)
    - example command `which fswatch` shows the full path of shell commands:
        >`$ which fswatch`
        
        expected output:
        
        >`/usr/local/bin/fswatch`

        the command `head -c 50 <filepath>` will print the first 50 bytes of a file

        >``$ head -c 50 `which fswatch` ``

        expected output:

        > `????????!H__PAGEZERO%`
    - similar example can be made with `$ man file` and `$ echo` commands
        >``$ echo `man file` ``
        
        expected output :

        >`FILE(1) BSD General Commands Manual FILE(1) NAME file...`

  - Changing Between Shells on Linux machine
    - Useful for working with Pop!_OS
    - $ chsh -s `which zsh`
    - $ chsh -s /bin/bash
    - $ gnome-session-quit to log user out or just open new terminal window to open new default shell, current window will remain with current bash or zsh shell
