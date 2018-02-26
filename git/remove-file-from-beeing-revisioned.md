# Remove file from beeing revisioned

If you would like to remove a file from git revision (unfollow).
Use command `git rm --cached [filename]` on each file
you want to remove from beeing tracked. Be sure to add a file to `.gitignore` 
file before using this command to prevent git from
re-track your file after another change made.

__Example:__

File to untrack: myFile.js. 

Command: `git rm --cached myFile.js`

---
_Last update: 26 Feb 2018_ 