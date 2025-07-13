# Vueフレームワーク応用のAzure Static Web Apps

## **はじめに**
### **Visual Studio Code**
- Visual Studio Codeをインストール  
    [![インストーラ](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/250px-Visual_Studio_Code_1.35_icon.svg.png)](https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user)  
- VS Codeの使い方　[VS Codeドキュメント](https://code.visualstudio.com/docs)  
VS Codeエクステンションは後ほど追加説明  
    > **ほかの開発ツールの使用も可能ですが、VS Codeは無料かつ軽量のため推奨**

### **Git**
- Gitをインストール [Gitインストーラ](https://github.com/git-for-windows/git/releases/download/v2.50.0.windows.2/Git-2.50.0.2-64-bit.exe ) 

### **Node.js**
- nvmをインストール [nvm for windows](https://github.com/coreybutler/nvm-windows/releases)  
    > node.jsのバージョン管理ツール。linux 環境はこちらのページに参考 [nvm](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating)
    - インストール成功のあと、システム環境変数は以下のキーが入っている。もし入っていなかったの場合は手動で追加。
    ```
    NVM_HOME=[nvmのインストールフォルダ]
    NVM_SYMLINK=[Node.jsの参照フォルダ]
    PATH+=%NVM_HOME%;%NVM_SYMLINK%
    ```
    > WindowsのPowerShellを使っているの場合、管理員権限で起動する必要があります。  
    > その上、npmのPowerShellスクリプト実行するための権限を与える必要があります。下記のコマンドを実行する。
    > ```
    > Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine```
- Node.jsをインストール  
    nvmインストール成功のあと、下記のコマンドでNode.jsのLTSバージョンをインストール  
    ```
    nvm install lts
    ```
    > 他のバージョンが必要の場合は nvm install \<version\> コマンド  



## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
