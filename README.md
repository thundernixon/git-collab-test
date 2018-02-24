# git-collab-test
This is a simple repo to test different ways of collaborating on type projects via Git &amp; GitHub

## How to contribute:

### First, clone the repo

1. Open your terminal and navigate to a folder you want this project to live in

    1. If you want to make a new folder while you're in the terminal, you can use the command `mkdir my-awesome-folder-name` (`mkdir` makes a directory, and you should replace the next part with the folder name you want)

    1. If you do make a new directory/folder, make sure you navigate into it with `cd my-awesome-folder-name`

1. When you're in the correct folder, in your terminal, run the command `git clone git@github.com:thundernixon/git-collab-test.git` to clone this repo (download its contents and history) into your new folder
    1. Just so you know, you can get that SSH address in repos by clicking the big green button, "Clone or Download"

1. confirm the files have downloaded by running the command `ls` to list files (you can also just go to the folder in finder by running the command `open .` or by just going to finder and clicking your way to it)

### Next, add a glyph and edit the ampersand in both font files

1. Open the .UFO file in RoboFont, and add any glyph. To save time, you can just copy in a glyph you already have, or click around briefly – we're learning about Git collaboration, not making a masterpiece, here. :)

1. Also edit the ampersand, which is already there. Either clean up a curve or two, add or remove a point, change the hook, whatever. Try to change part of it, and to also **not** change at least a few anchors and handles.

1. Copy the new glyph and the changed ampersand over to the .glyphs font (if you're worried that copying the whole edited ampersand over to the Glyphs file will change all the lines of code for that glyph, I was too – but only the coordinates with changes will show up as changed code in Git)

1. Now, add your changes to your repo with `git add .`, then commit them with `git commit -m "added letter [whatever] and edited ampersand"`

1. To prevent merge issues, run `git pull` to fetch and merge any potential updates to the remote origin

1. You'll either see updates that look something like `57ca341..c842280  master -> master` or you'll see the message "Already up-to-date."
    1. If `git pull` doesn't work yet, you probably need to tell your local git which remote it should be connected to. Use `git branch --set-upstream-to origin/master` to tell Git which "upstream" branch you want to track with your current repo & branch, then run `git pull`

1. Now, push up your changes with `git push`. They should now be on the remote!

