The tutorial of how to install oh-my-zsh
---

##### 1. You need to install **Zsh** first:
- **_sudo apt install zsh_**
    - if you get an error (dpkg was interrupted) you must run this command:
    **_sudo dpkg --configure -a_**
##### 2. Verify installation:
- _zsh --version_
##### 3. You need to make it your default shell:
- _sudo chsh -s $(which zsh)_
##### 4. You need to log out and login:
- Test that it worked
    - **_echo $SHELL_**
    If your result is _/bin/zsh_ or similar then you're good to go
- Do another test
    - **_$SHELL --version_**
    Expected result is _zsh 5.4.2_
##### 5. Installing oh-my-zsh:
- You can use _curl_ or _wget_
    - via curl
    ```
        sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    ```

    - via wget
    ```
        sh -c "$wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)
    ```
-----

# OPTIONAL PART
##### 6. Plugins:
- You can use the _.zshrc_ file I uploaded to github
it uses:
    - **git**
        - you can see what branch are you on which is quite handy
    - **sudo**
        - if you forgot to write **_sudo_** before some command you can easily put it by pressing the ESC key **twice**
    - **docker**
    - **docker-compose**
    - **history**
        - if you type h (history) oh-my-zsh will show you the command-history
    - **history-substring-search**
        - if you start typing in any previous command (part of it) and hit UP key then the similar one will be shown

# Other (useful) features
- no need to type **cd** to change directory
    - you can simply type in the correct folder name and press ENTER to... well... ENTER to the directory
    - this is same for leaving a directory as well
        - simply type in **..** instead of **cd ..**
- typing **l** (L) is like typing in  **ls -a**




