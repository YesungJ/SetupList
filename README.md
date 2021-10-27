# SetupList
setup of new pc

1. Chrome
 Install Chrome
 
2. VSCode
added all of optional
 2-1 extends
  - python
  - Material Icon Theme
  - Material Theme
  - Prettier
  - ESLint
  
  
3. Git

4. wsl

5. Chocolatey
 - https://chocolatey.org/
 - this will be helpful if you use packages on windows 
 
6. python install 
 - search chocolaty
 
7. install windows terminal at MSstore

8. install WSL2 for windows
 ```
 #windows Terminal
 
 1.Linux 用 Windows サブシステムを有効にする
 dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
 
 2. install ubuntu at MSstore
 
 3. 再起動
 
 4. Ubuntuのユーザ設定がでれば成功

 5. 仮想マシンの機能を有効にする
 *9の後に実行
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

 6. 再起動 
 
 7. wsl --set-default-version 2
  * アップデートが必要と出た場合、カーナルのアップデートが必要(wsl2-kernal)
  
 8. wsl --list --verbose
  Nameとバージョン確認
  wsl --set-version <name> <2>
  2であったら問題ない
  BIOSによる仮想化設定必要かも
 ```
8. install zsh
 ```
 apt install zsh

 ```


9. oh my zsh
https://ohmyz.sh/#install

//デフォルト設定
$sudo chsh -s $(which zsh) $(whoami) 

おすすめ？
zsh-autosuggestions
zsh-syntax-highlighting
 
 
 theme
https://docs.microsoft.com/ja-jp/windows/terminal/customize-settings/color-schemes 
 
 setting.jsonで
 Solarized Dark
 ```
                 "colorScheme": "Solarized Dark",
 ```
 or terminal splash
https://terminalsplash.com/
でMonokai Night for Windows Terminalのコードダウンロードし
setting.jsonのschemesに入れる

→
```
                "colorScheme": "Monokai Night"
```
にする


10. powerlevel10k 
 https://github.com/romkatv/powerlevel10k#oh-my-zsh
 
 code ~/.zshrc
 

## trouble
### sudoのときは
```
sudo su - 
```
か
rootのpassword 設定が必要
```
$ sudo su -
# passwd
Enter new UNIX password: 
Retype new UNIX password: 
passwd: password updated successfully
```
`su`でエラーが出た場合は1番目を使う
