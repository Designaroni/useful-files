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
