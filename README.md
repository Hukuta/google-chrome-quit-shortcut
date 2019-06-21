# Google Chrome Quit Shortcut

### Problem
Google Chrome does not support "Ctrl+Q" to quit on Linux. "Ctrl+Shift+Q" does nothing too.

### Solution
Use pkill with tiny script to gracefully terminate Google Chrome using hotkey.

### How to use
Make sure *xdotool* is installed:
`which xdotool`
shoud be "/usr/bin/xdotool". If xdotool not found, please install it.

Bind *quit-chrome.sh* bash script to any hotkey. I prefer "Ctrl+Win+Q", which does not conflict with "Ctrl+Q".

`/bin/bash YOUR_PATH_TO_SCRIPT/quit-chrome.sh > /dev/null`

Keep in mind that the script will work if the browser window is active. Thereby, You can add other programs to the script to provide the desired logic for each one.
