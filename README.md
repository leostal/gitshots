## What's that?

Git post-commit hook to make a photo of you on every commit you make!

## Prerequisite

Node.js should be installed

## Installing

```
git clone https://github.com/leostal/gitshots.git ~/.git-hooks
git config --global core.hooksPath ~/.git-hooks
mkdir -p ~/.git-shots
sudo apt-get install fswebcam
sudo chmod a+x ~/.git-hooks/post-commit
```
