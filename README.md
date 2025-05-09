# 各平台支援情況：

# Linux	✅ 完全支援	官方主要目標平台

# macOS	✅ 完全支援	一樣用 curl 安裝

# Windows	❌ 不直接支援	可透過WSL或Git Bash間接使用

# 1.安裝 WSL
wsl --install

# 2. 更新 WSL 到最新版本
wsl --update

# 3. 啟動 Ubuntu（進入 Linux 系統）
wsl -d Ubuntu

# 4. 建立新帳號
# 系統會提示輸入帳號名稱和密碼（密碼會隱藏）
Create a default Unix user account: xxx
New password: xxx
Retype new password: xxx

# 5. 更新套件清單
sudo apt update

# 6. 升級所有可升級的套件
sudo apt upgrade -y

# 7. 安裝 zip / unzip 工具（SDKMAN 需要用到）
sudo apt install zip unzip -y

# 8. 安裝 SDKMAN
curl -s "https://get.sdkman.io" | bash

# 9. 載入 SDKMAN 環境變數
source "$HOME/.sdkman/bin/sdkman-init.sh"

# 10. 檢查目前安裝的 Linux 環境
wsl --list --verbose

# 11. 啟動指定的 Linux 發行版
wsl -d Ubuntu

# 12. 把 Ubuntu 設成預設
wsl --set-default Ubuntu

# 13. 安裝最新版本的 Java（可自選版本）
sdk install java 21.0.7-tem

# 14. 安裝 Spring Boot CLI
sdk install springboot
