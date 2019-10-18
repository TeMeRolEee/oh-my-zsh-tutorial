The tutorial of how to install oh-my-zsh
---

1. You need to install **Zsh** first:
    - `sudo apt install zsh`
        - if you get an error (dpkg was interrupted) you must run this command: `sudo dpkg --configure -a`
2. Verify installation:
    - `zsh --version`
3. You need to make it your default shell:
    - ```chsh -s $(which zsh)```
4. You need to log out and login:
    - Test that it worked
        - `echo $SHELL`
        If your result is _/bin/zsh_ or similar then you're good to go
    - Do another test
        - `$SHELL --version`
        Expected result is _zsh 5.4.2_
5. Installing oh-my-zsh:
    - You can use _curl_ or _wget_
        - via curl
        ```bash
            sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
        ```

        - via wget
        ```bash
            sh -c "$wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)
        ```
6. Download the **.zshrc** file to your HOME directory
    - If it's done change the **USER** part to yours:

        ```export ZSH=/home/<USER>/.oh-my-zsh```

        It will look something like this:

        ```export ZSH=/home/theuserijusttyped/.oh-my-zsh```

-----

# OPTIONAL PART
7. Plugins:
    - You can use the _.zshrc_ file I uploaded to github
    it uses:
        - **git**
            - adds a lot of aliases, see [here](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugin:git)
        - **sudo**
            - if you forgot to write `sudo` before some command you can easily put it by pressing the **ESC** key **twice**
        - **docker**
            - gives autocomplete support
        - **docker-compose**
            - gives autocomplete support
        - **history**
            - if you type h (history) oh-my-zsh will show you the command-history
        - **history-substring-search**
            - if you start typing in any previous command (part of it) and hit UP key then the similar one will be shown

# Other (useful) features
## From ZSH
- no need to type `cd` to change directory
    - you can simply type in the correct folder name and press ENTER to... well... ENTER to the directory
    - this is same for leaving a directory as well
        - simply type in `..` instead of `cd ..`
## From oh-my-zsh
- typing `l` is like typing in  `ls -a`
## Custom
- `tre` is a shorthand for tree with hidden files and color enabled
- `reload` will reload your terminal window and you don't need to close and reopen after modifying your environment


