This script will prevent macos from sleeping, dimming screen, screensaver and screen lock.

Add the script to ~/.bashrc or ~/.zshrc

Install cliclick with `brew install cliclick`

```bash
keepawake() {
while true; do
    # Moves the mouse cursor by 1 pixel diagonally and back
echo "moving mouse"
cliclick m:+1,+1 m:-1,-1

    # Wait for 3 minutes
    sleep 180
done
}
```