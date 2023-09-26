## Linux Configuration after installation

### 1. Update all currently installed packages
   ```
    sudo apt-get update
   ```

### 2. Terminal configuration with zsh
    ```
    1. install zsh
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

    2. nano ~/.zshrc

    3. Add these: 
    
    # skype path
    export PATH="$PATH:/snap/bin"

    # Path to your oh-my-zsh installation.
    export ZSH="$HOME/.oh-my-zsh"

    # See https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
    ZSH_THEME="jonathan"

    plugins=(zsh-autosuggestions git)

    source $ZSH/oh-my-zsh.sh

    figlet -f digital "              Ayon Jodder" |lolcat

    export NVM_DIR="$HOME/.nvm"
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
    [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_compl>
    ```

### 3. Install nvm and nodejs
    ```
    1. curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash

    2. apply the changes to your current session
    source ~/.bashrc

    3. install nodejs
    nvm install 18.18.0

    4. use nodejs version
    nvm use 18.18.0
    ```

### 4. Install git
    ```
    sudo apt install git-all

    git config --global user.name "Your Name"
    git config --global user.email "youremail@example.com"

    ```

### 5. Install vscode
    ```
    1. Donwload vscode.
    2. sudo dpkg -i file_name.deb
    ```

### 6. Install chrome
    ```
    1. Download chrome.
    2. sudo dpkg -i file_name.deb
    ```

### 7. Install cascadia code font
    ```
    1. Download cascadia code font.
    2. cp /Downloads/CascadiaCode-2111.01/*.ttf /usr/local/share/fonts/
    3. sudo fc-cache -f -v
    4. fc-list | grep "Cascadia Code"
    ```

### 8. Install snap
    ```
    1. sudo apt update
    2. sudo apt install snapd
    3. sudo systemctl start snapd
    ```

### 9. Install skype
    ```
    1. sudo snap install skype --classic
    ```

### 10. Install whatsapp
    ```
    1. sudo apt-get update
    2. snap install whatsapp-for-linux
    3. snap run whatsapp-for-linux
    ```