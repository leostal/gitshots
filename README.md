## What's that?

Git post-commit hook to make a photo of you on every commit you make!

## Prerequisite

Node.js should be installed

## Installing (macos)

```
# Clone and set up hooks
git clone https://github.com/leostal/gitshots.git ~/.git-hooks
git config --global core.hooksPath ~/.git-hooks
mkdir -p ~/.git-shots

# Install imagesnap
brew install imagesnap

# Make the script executable
chmod +x ~/.git-hooks/post-commit

```
