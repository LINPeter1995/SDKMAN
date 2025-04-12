# SDKMAN
wsl --install         # 安裝 WSL（Windows 子系統 Linux）
wsl --update          # 更新 WSL 到最新版本
wsl -d Ubuntu         # 啟動 Ubuntu（進入 Linux 系統）


# 建立新帳號 ibame（會提示輸入密碼兩次）
# 密碼會隱藏，輸入完按 Enter 即可
Create a default Unix user account: ibame
New password: 123
Retype new password: 123


sudo apt update                         # 更新套件清單
sudo apt install zip unzip -y          # 安裝 zip / unzip 工具（SDKMAN 需要用到）


curl -s "https://get.sdkman.io" | bash         # 安裝 SDKMAN
source "$HOME/.sdkman/bin/sdkman-init.sh"      # 載入 SDKMAN 環境變數


sdk install java                 # 安裝最新版本的 Java（可自選版本）
sdk install springboot          # 安裝 Spring Boot CLI

