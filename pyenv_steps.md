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

## Refresh the shell
`. ~/.zshrc`

## Install 3.10.6
`pyenv install 3.10.6`

This will fail because we havent installed openssl

## Install open ssl and other things we need for pyenv
`brew install openssl@1.1`
`brew install readline`

## Shortcut to reload the shell
`alias rr='. ~/.zshrc'`

## How to ssh
1. `cd ~/.ssh || mkdir ~/.ssh`
2. `cd ~/.ssh`
3. `ssh-keygen`
4. `pbcopy < ~/.ssh/gitgud.pub`