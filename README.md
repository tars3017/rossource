# rossource
## Purpose
In any directories under a ROS workspace, it will help you find devel/setup.bash or setup.zsh
and source it for you. Then you don't have to navigate around the directories when you want to 
source the file.

## How to Use it
run ```. rossource``` in terminal under a ROS workspace.

You can also run ```cd -``` after using rossource to switch to the root of the workspace.

## Installation 
1. Manual
    1. Download the rossource file to the place you want to store.
    2. Add that path to your $PATH varibale.
2. Automatic
    Run the commands below, it will download the file to your HOME.
    ```
    cd ~
    git clone https://github.com/tars3017/rossource.git
    cp rossource/rossource .
    rm -r ~/rossource
    ```

    - bash
    ```
    echo 'export PATH=$HOME:$PATH' >> ~/.bashrc
    source ~/.bashrc
    ```

    - zsh
    ```
    echo 'export PATH=$HOME:$PATH' >> ~/.zshrc
    source ~/.zshrc
    ```
    
