# taskfile-zsh-autocompletion

## Installation

### MacOs

- Clone the repository
- Run this command which will add line to the `.zshrc` with additional `FPATH` path for taskfile autocomplete:

    `echo FPATH=$(PWD)\/src:\$FPATH >> ~/.zshrc`

- In some cases autocomplete after previous command doesn't work, so I added below comands:

    `echo autoload -U _task >> ~/.zshrc`
    `echo compdef _task task >> ~/.zshrc`