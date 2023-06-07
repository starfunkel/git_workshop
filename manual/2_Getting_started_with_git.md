# Install and configure Git for Windows on Windows 10
<br>

## 1. CLI only Installation

```powershell
winget install --id Git.Git -e --source winget
```

## Test it

```powershell
ssh git@github.com
```

## Set global Git config

```powershell
git config --global  user.name ""
git config --global user.email ""
git config --global credential.helper cache
git config --list 
```

## Create a new repository on the command line

```powershell
Write-Output "# STUFF" >> README.md
git init
git add README.md
git add     # was commitet werden soll
git add .  # für ganzen Ordner
git commit -m "first commit"
git branch -M main
git remote add origin <Repo URL>
git push --set-upstream -origin main
git push -u origin main
```

## Pull existing Github Repo

```powershell
git init
git branch -M main
git remote add origin <Repo URL>
git pull pull <remote repo URL> <branch>
git add .
git commit -m ""
git push --set-upstream origin main
git push
```

## Push an existing repository from the command line

```powershell
git remote add origin <remote repo URL>
git branch -M main
git push -u origin main
