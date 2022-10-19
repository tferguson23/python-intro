# install pyenv

Run the following in sequence:
1. `curl https://pyenv.run | bash`
2. `cat ~/.zshrc` # this didn't work but it will when you run number 3
3. `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Add to `.zshrc`

```bash
export PATH="$HOME/.poetry/bin:$PATH"
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```