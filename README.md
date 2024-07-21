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
- [Toipe](https://github.com/Samyak2/toipe): terminal typing tester
```bash
cargo install toipe
```
- [Hyperfine](https://github.com/sharkdp/hyperfine?tab=readme-ov-file): command-line benchmarking tool
```bash
cargo install --locked hyperfine
```
- [fzf](https://github.com/junegunn/fzf): general-purpose command-line fuzzy finder
```bash
sudo apt install fzf
```
*aliases*
```bash
export FZF_DEFAULT_OPTS="
	--color=fg:#908caa,bg:#191724,hl:#ebbcba
	--color=fg+:#e0def4,bg+:#26233a,hl+:#ebbcba
	--color=border:#403d52,header:#31748f,gutter:#191724
	--color=spinner:#f6c177,info:#9ccfd8
	--color=pointer:#c4a7e7,marker:#eb6f92,prompt:#908caa"
export BAT_THEME="ansi"
alias f='fd -t f . $HOME | fzf --layout=reverse --info=inline --border --margin=1 --padding=1 --preview "batcat -n --color=always {}" | xargs -r nvim'
alias d='cd $(fd -t d . $HOME | fzf --height=50% --layout=reverse --info=inline --border --margin=1 --padding=1)'
```
## Miscs
- Git logs as an alias in .bashrc
```bash
alias gitl='git log --graph --decorate --oneline --all'
  ```
- wmctrl for window swaping
```bash
sudo apt-get install wmctrl
```
and in linux shortcut
```bash
sh -c 'wmctrl -xa gnome-terminal || gnome-terminal'
sh -c 'wmctrl -xa brave-browser || brave-browser'
```
