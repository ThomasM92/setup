# setup
All the programs I used and their setup

## Terminal colortheme
- [Gogh-Co](https://github.com/Gogh-Co/Gogh): easy theme setup
```bash
sudo apt-get install dconf-cli uuid-runtime # prerequisits
bash -c "$(wget -qO- https://git.io/vQgMr)"
```

## Rust utils
- [Starship](https://starship.rs/): a cross-shell prompt
```bash
curl -sS https://starship.rs/install.sh | sh
```
- [Exa](https://the.exa.website/): a modern replacement for ls
```bash
sudo apt install exa
```
- [Fd](https://github.com/sharkdp/fd): a simple, fast and user-friendly alternative to find
```bash
cargo install fd
```
- [Dust](https://github.com/bootandy/dust): a more intuitive version of du in rust
```bash
cargo install du-dust
```
- [Broot](https://github.com/Canop/broot): a better way to navigate directories
```bash
cargo install broot
```
- [Bat](https://github.com/sharkdp/bat): a cat clone with syntax highlilghting and Git integration
```bash
sudo apt install bat
```
- [Ripgrep](https://github.com/BurntSushi/ripgrep): a rust replacement for grep
```bash
sudo apt-get install ripgrep
```
- [Gitui](https://github.com/extrawurst/gitui): a blazing fast terminal-ui for git
```bash
cargo install gitui
```
- [Tokei](https://github.com/XAMPPRocky/tokei): count your code, quickly
```bash
cargo install tokei
```
- [Zellij](https://github.com/zellij-org/zellij): terminal multiplexer
```bash
cargo install --locked zellij
```
