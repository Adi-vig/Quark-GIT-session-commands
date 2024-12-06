# Line by line commands till first push-


1. Open your terminal in your folder 
    - right click and click ```open in terminal```

2. Paste the following to clone and open vscode in repository folder

```bash 
git clone <https link to your repo>
code <name-of-your-repo>
```

NOTE: here onwards we will only use VSCODE integrated Terminal and all the commands are to be used in VSCODE integrated terminal

3. You should see your ```README.md```
4. Modify the file and save it.

## 5. Go to terminal type: This step is Local

you should see the modified file and not added to staging area

Type in terminal
```bash
git status
```

add the file to staging area
```bash
git add .\README.md
```

you should see the modified file and added to staging area
```bash
git status
```

to commit anything to any repo you have to set identity (which shows up in commit)
```bash
git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"
```

Commit the staged changes
```bash
git commit -m "this is a Commit message"
```


## 6. Now going remote
## Add your PAT 
## WARNING: do not leak your PAT ......... otherwise just use browser sign in method

## Procedure for PAT: 
1. Go to github.com -> setting (scroll down) -> Developer settings -> Personal access tokens ->  Tokens(classic) -> Generate new token -> Generate new token(classic)
![](./Screenshot%20from%202024-12-06%2016-59-25.png)  

Authorize yourself password/ 2FA
 
2. Type your note for token so you can remember it later
3. Give a expiration time.
4. Mark all the checkboxes.

![](./Screenshot%20from%202024-12-06%2017-02-47.png)

5. Scroll down and click on -> Generate token
6. Click on copy and copy the token 

7. Go back to VScode terminal:
```bash 
git push 
```

Wait a few seconds a new window will open

Select authorization mode from the window
```
    1) browser/device
    2) Token 
```

Select token -> Paste your token press sign in



go back to vscode and type
```bash
git push -u origin main
```

7. To get your repo link
```bash
git remote -v
```




# Further Readings (MUST READ):
- [Link for cheat sheet for 40 commands ](https://dev.to/ruppysuppy/git-cheat-sheet-with-40-commands-concepts-1m26)

## What else needs to be covered:

- branching (branch merge)
- restore, reset 
- reflog
- gitk (useful for seeing commits and branch tree)
- stash (advanced)
- rebase (advanced)

## HAPPY CODING