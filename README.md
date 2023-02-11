# ros_auto_source
## Purpose 工具目的
In any directories under a ROS package, it will help you find devel/setup.bash
and source it for you.

每次要跑 ROS 之前都要先```source devel/setup.bash```(或者```setup.zsh```)，
這樣就必須先移動到該資料夾再移回來，使用起來不方便，所以想利用這樣的工具
就可以在 ROS workspace 下的任一個資料夾直接 source 檔案。

## Usage 使用方法
run ```. rossource``` in terminal

在終端機輸入```. rossource```即可幫你自動 source 完檔案，但要注意必須是
在 workspace 底下執行這行指令，否則會出現錯誤訊息。

## Installation 安裝方法
1. 手動安裝
    1. 下載 rossource 這個檔案到你想儲存的地方
    2. 把該路徑加到 PATH 中，然後存在 .bashrc 或 .zshrc
2. 自動安裝(安裝在 $HOME 下)
    直接執行以下指令
    ```
    git clone https://github.com/tars3017/ros_auto_source.git
    cd ~
    cp ros_auto_source/rossource .
    rm -r ~/ros_auto_source
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
    
