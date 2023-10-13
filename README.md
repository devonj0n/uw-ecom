# A basic Golang project to showcase my skills to UW


Install rtx
```bash
curl https://rtx.pub/rtx-latest-macos-arm64 > ~/bin/rtx
chmod +x ~/bin/rtx
rtx --version
rtx 2023.10.1
```

Hook rtx into your shell (pick the right one for your shell):
```
# note this assumes rtx is located at ~/bin/rtx
echo 'eval "$(~/bin/rtx activate bash)"' >> ~/.bashrc
echo 'eval "$(~/bin/rtx activate zsh)"' >> ~/.zshrc
echo '~/bin/rtx activate fish | source' >> ~/.config/fish/config.fish
```

Install Golang
```bash
rtx use golang
```