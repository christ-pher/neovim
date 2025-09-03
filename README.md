# nvim config
This is my personal neovim config, forked from [kickstart](https://github.com/nvim-lua/kickstart.nvim).

### Debian Setup
```bash
# Update and Install dependencies
sudo apt update
sudo apt install make gcc ripgrep unzip git xclip curl

# Now we install nvim
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo rm -rf /opt/nvim-linux-x86_64
sudo mkdir -p /opt/nvim-linux-x86_64
sudo chmod a+rX /opt/nvim-linux-x86_64
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz

# Make it available in /usr/local/bin, distro installs to /usr/bin
sudo ln -sf /opt/nvim-linux-x86_64/bin/nvim /usr/local/bin/

# Clone this repo
git clone https://github.com/christ-pher/neovim.git "${XDG_CONFIG_HOME:-$HOME/.config}"/nvim
```

```bash
# Run neovim
nvim
```
