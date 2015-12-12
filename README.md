# electron-sample

## Dev to Run
### install electron
```
npm -g install electron-prebuilt
```

### init app
```
mkdir electron-sample
cd electron-sample
npm init -y
```

### create app
* index.js
* index.html

### run
```
electron .
```

## Package to Distributing
### install asar
```
npm -g install asar
```

### package
```
asar pack . ~/app.asar
```

### distribution
* unpack electron distribution `~\.electron\electron-v0.36.0-win32-x64` (for Windows)
* copy app
```
cp -r ~/app.asar ~/.electron/electron-v0.36.0-win32-x64/resources
```
* rename electron.exe to electron-sample.exe
```
mv ~/.electron/electron-v0.36.0-win32-x64/electron.exe ~/.electron/electron-v0.36.0-win32-x64/electron-sample.exe
```

