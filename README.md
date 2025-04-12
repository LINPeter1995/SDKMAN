# SDKMAN

# 安裝 WSL（Windows 子系統 Linux）

wsl --install 

# 更新 WSL 到最新版本

wsl --update 

# 啟動 Ubuntu（進入 Linux 系統）

wsl -d Ubuntu 

# 建立新帳號 ibame（會提示輸入密碼兩次）

Create a default Unix user account: ibame 

# 密碼會隱藏

New password: 123 

# 輸入完按 Enter 即可 

Retype new password: 123  

# 更新套件清單

sudo apt update 

# 安裝 zip / unzip 工具（SDKMAN 需要用到）

sudo apt install zip unzip -y 

# 安裝 SDKMAN

curl -s "https://get.sdkman.io" | bash 

# 載入 SDKMAN 環境變數

source "$HOME/.sdkman/bin/sdkman-init.sh"

# 安裝最新版本的 Java（可自選版本）

sdk install java 

# 安裝 Spring Boot CLI

sdk install springboot 
