# dotfiles

## Prerequisites
```
sudo apt-get install ninja-build gettext cmake unzip curl build-essential python3 python3-venv clang ripgrep
```

## Build
```
git clone https://github.com/neovim/neovim
cd neovim && make CMAKE_BUILD_TYPE=RelWithDebInfo 
sudo make install || cd build && cpack -G DEB && sudo dpkg -i nvim-linux64.deb
```

Add to .bashrc: export PATH=$PATH:$HOME/.local/bin
