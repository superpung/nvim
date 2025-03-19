# 💤 LazyVim

A starter template for [LazyVim](https://github.com/LazyVim/LazyVim).
Refer to the [documentation](https://lazyvim.github.io/installation) to get started.

## Installation

1. [nvim](https://github.com/neovim/neovim/blob/master/INSTALL.md):

  ```sh
  # macOS
  brew install neovim
  
  # Linux
  curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
  sudo rm -rf /opt/nvim
  sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
  export PATH="$PATH:/opt/nvim-linux-x86_64/bin"

  # Linux (built with glibc 2.17)
  curl -LO https://github.com/neovim/neovim-releases/releases/download/v0.10.4/nvim-linux-x86_64.tar.gz
  sudo rm -rf /opt/nvim
  sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
  export PATH="$PATH:/opt/nvim-linux-x86_64/bin"
  ```

1. [lazygit](https://github.com/jesseduffield/lazygit):

  ```sh
  # macOS
  brew install lazygit
  
  # Linux
  LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | \grep -Po '"tag_name": *"v\K[^"]*')
  curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/v${LAZYGIT_VERSION}/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
  tar xf lazygit.tar.gz lazygit
  sudo install lazygit -D -t /usr/local/bin/
  ```
