## What's this?

Git post-commit hook that snaps a photo for every commit, then shows a macOS notification for success or failure.

## Requirements

- Node.js (to run the hook script)
- `imagesnap` (captures webcam frames)
- macOS notification support via the built-in `osascript`

## Installation (macOS)

```bash
# Clone and set up hooks
git clone https://github.com/leostal/gitshots.git ~/.git-hooks
git config --global core.hooksPath ~/.git-hooks
mkdir -p ~/.git-shots

# Install imagesnap
brew install imagesnap

# Make the hook executable
chmod +x ~/.git-hooks/post-commit
```

After installation, each commit will trigger a background capture. You will see a notification when a photo is saved and a different alert if the capture fails (e.g. camera disconnected). The hook won’t block your commit even if the device needs time to reconnect.

<img width="736" height="342" alt="CleanShot 2025-10-30 at 23 28 10@2x" src="https://github.com/user-attachments/assets/1ac783d5-24f5-4849-a57b-74be73f36caf" />

