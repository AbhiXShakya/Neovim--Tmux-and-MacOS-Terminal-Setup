# 🚀 Neovim Tmux MacOS Terminal Setup

Welcome to the ultimate guide for setting up a powerful development environment on MacOS using Neovim, Tmux, and Kitty terminal! This repository contains all the necessary instructions and configuration files to get you up and running with a beautiful, efficient, and feature-rich setup.

## 📋 Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
  - [Homebrew](#-homebrew)
  - [Oh My Zsh](#-oh-my-zsh)
  - [Kitty Terminal](#-kitty-terminal)
  - [Tmux](#-tmux)
  - [Neovim](#-neovim)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Ensure you have a MacOS system with administrative privileges.

## Installation

### 🍺 Homebrew

1. Install Homebrew:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. Add Homebrew to your PATH:
   ```bash
   echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
   ```

3. Install necessary packages:
   ```bash
   brew install git zsh-autosuggestions zsh-syntax-highlighting eza zoxide tmux bash neovim ripgrep fd gcc
   ```

4. Reload your profile:
   ```bash
   source ~/.zprofile
   ```

### 🛠 Oh My Zsh

1. Install Oh My Zsh:
   ```bash
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

2. **Note**: After installation, copy the provided `.zshrc` file to your home directory and set up your desired Oh My Zsh theme.

### 😺 Kitty Terminal

1. Download and install Kitty from the [official GitHub repository](https://github.com/kovidgoyal/kitty/tags).
2. Install the DankMonoNerdFont or your preferred font.
3. Copy all configuration files to `~/.config/kitty/`.
4. To change fonts in Kitty, use:
   ```bash
   kitten choose_font
   ```
   or
   ```bash
   kitty list-fonts
   ```

### 🖥 Tmux

1. Install Tmux Plugin Manager (TPM):
   ```bash
   git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
   ```

2. Replace `~/.tmux.conf` with the provided configuration file.

3. Install plugins:
   - Launch tmux: `tmux`
   - Press `Ctrl+B`, then `I` to install plugins

### 🚧 Neovim

1. Remove existing Neovim configuration:
   ```bash
   rm -rf ~/.config/nvim
   ```

2. Copy the provided `nvim` folder to `~/.config/`.

3. Launch Neovim to automatically install plugins:
   ```bash
   nvim
   ```

## Configuration

Detailed configuration instructions for each tool can be found in their respective directories within this repository.

## Troubleshooting

If you encounter any issues during setup, please check the [Issues](https://github.com/yourusername/Neovim-Tmux-MacOS-Terminal-Setup/issues) section of this repository or open a new issue if your problem isn't addressed.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

⭐️ If you found this helpful, please star this repository to show your support!