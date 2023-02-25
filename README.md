# qtDeb
The debian environment I use for testing, with Qtile as the window manager

## SUDO for your user

1. Install sudo

```bash
su -
apt install sudo
```

2. Add the user to the sudo group

```bash
usermod -aG sudo <username>
```

3. Logout

Now the user has sudo privileges


## Nvim install and config

1. Download latest stable nvim release

```
wget https://github.com/neovim/neovim/releases/download/stable/nvim-linux64.deb
```

2. Install the package

```
sudo apt install ./nvim-linux64.deb
```

3. Install packer (nvim plugin manager)

```
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
```

4. Download plugins

```
cd ~/.config/nvim/lua/fm
nvim packer.lua
:so
:PackerSync
```
