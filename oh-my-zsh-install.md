#The tutorial of how to install oh-my-zsh
---

##### 1. You need to install **Zsh** first:
- **_sudo apt install zsh_**
    - if you get an error (dpkg was interrupted) you must run this command:
    **_sudo dpkg --configure -a_**
##### 2. Verify installation:
- _zsh --version_
##### 3. You need to make it your default shell:
- _sudo chsh -s $(which zsh)_
##### 4. You need to log out and login.
- Test that it worked
    - **_echo $SHELL_**
    If your result is _/bin/zsh_ or similar then you're good to go
- Do another test
    - **_$SHELL --version_**
    Expected result is _zsh 5.4.2_
##### 5. Installing oh-my-zsh
- You can use _curl_ or _wget_
    - via curl
    ```
        sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    ```

    - via wget
    ```
        sh -c "$wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)
    ```





