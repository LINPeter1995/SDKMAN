# 1. 安裝 WSL（Windows 子系統 Linux）
wsl --install

# 2. 更新 WSL 到最新版本
wsl --update

# 3. 啟動 Ubuntu（進入 Linux 系統）
wsl -d Ubuntu

# 4. 建立新帳號
# 系統會提示輸入帳號名稱和密碼（密碼會隱藏）
Create a default Unix user account: ibame
New password: 123
Retype new password: 123

# 5. 更新套件清單
sudo apt update

# 6. 安裝 zip / unzip 工具（SDKMAN 需要用到）
sudo apt install zip unzip -y

# 7. 安裝 SDKMAN
curl -s "https://get.sdkman.io" | bash

# 8. 載入 SDKMAN 環境變數
source "$HOME/.sdkman/bin/sdkman-init.sh"

# 9. 檢查目前安裝的 Linux 環境
wsl --list --verbose

# 10. 啟動指定的 Linux 發行版
wsl -d Ubuntu

# 11. 把 Ubuntu 設成預設
wsl --set-default Ubuntu

# 12. 安裝最新版本的 Java（可自選版本）
sdk install java

# 13. 安裝 Spring Boot CLI
sdk install springboot

