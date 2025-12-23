# electron-demo


## 参考资料：
```
https://www.electronforge.io/
https://www.electronjs.org/docs
```


## 创建项目：
```
npx create-electron-app@latest electron-demo --template=vite-typescript
nvm use v22.17.1
npm install electron --save-dev 
```

## 常见问题

若下载慢考虑切换源，方法如下：
```
npm config edit
```
将下面三行放到配置文件并保存
```
registry=https://registry.npmmirror.com
electron_mirror=https://cdn.npmmirror.com/binaries/electron/
electron_builder_binaries_mirror=https://npmmirror.com/mirrors/electron-builder-binaries/
```
清除npm 缓存
```
npm cache clean --force
```
安装 
```
npm install --save-dev electron
```


## forge交叉编译
打包windows
```
brew install mono
brew install --cask xquartz
brew install --cask wine-stable 
或
brew install --cask wine-devel

wine --version
```


打包deb
```
brew install dpkg
brew install fakeroot

dpkg --version
fakeroot --version
```