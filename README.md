<div align="center">
  <a href="https://gridea.dev">
    <img src="public/app-icons/gridea.png"  width="80px" height="80px">
  </a>
  <h1 align="center">
    Gridea
  </h1>
  <h3 align="center">
    A static blog writing client
  </h3>

  [Download](https://github.com/pgs666/gridea/releases) | [Homepage](https://gridea.dev/)

  <a href="https://github.com/pgs666/gridea/releases/latest">
    <img src="https://img.shields.io/github/release/pgs666/gridea.svg?style=flat-square" alt="">
  </a>

  <a href="https://github.com/pgs666/gridea/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/pgs666/gridea.svg?style=flat-square" alt="">
  </a>
  
  <a href="https://github.com/pgs666/gridea/releases/latest">
    <img alt="GitHub All Releases" src="https://img.shields.io/github/downloads/pgs666/gridea/total.svg?color=%2312b886&style=flat-square">
  </a>

</div>

<div align="center">
  <img src="gridea-app-en.png">

</div>

English | [Русский](https://github.com/pgs666/gridea/blob/master/README-ru.md)  | [简体中文](https://github.com/pgs666/gridea/blob/master/README-zh_CN.md)  | [繁體中文](https://github.com/pgs666/gridea/blob/master/README-zh_TW.md)

**[CHANGELOG](https://github.com/pgs666/gridea/blob/master/CHANGELOG.md)**

## Fork status / Windows ARM64

This fork tracks `getgridea/gridea:master` and currently keeps a small set of changes focused on making **Windows ARM64** builds work in GitHub Actions and Releases.

Current file-level differences from upstream:

- `.github/workflows/build-arm.yml`: adds a Windows ARM64 GitHub Actions workflow that builds ARM64 app artifacts and then produces a custom ARM64 installer
- `.github/installers/gridea-arm64-installer.nsi`: adds a custom NSIS installer script used to package the ARM64 app into an installable `.exe`
- `package.json`: adds `yarn electron:build:win-arm64`
- `vue.config.js`: disables main-process minification to avoid the legacy Terser failure in the Electron main process bundle
- `src/assets/locales.ts`: fixes a missing trailing comma in `ja_JP`, which blocked CI builds
- `README.md` / `README-zh_CN.md`: documents this fork's differences from upstream and ARM64 packaging status

Build artifacts for this fork are published from this repository's Actions/Releases instead of upstream releases.

👏  Welcome to use **Gridea**！

✍️  **Gridea** A static blog writing client. You can use it to record your life, mood, knowledge, notes and ideas...


## Features👇
📝  Use the coolest **Markdown** editor to create quickly

🌉  Insert pictures and article cover charts anywhere in the article

🏷️  Label and group articles 

📋  Customize menus and even create external link menus

💻  Use this client on **Windows** or **MacOS**  or **Linux**

🌎  Use **Github Pages** or **Coding Pages** to show the world that more platforms will be supported in the future

💬  Simply configure and access the [Gitalk](https://github.com/gitalk/gitalk) or [DisqusJS](https://github.com/SukkaW/DisqusJS) comment system

🗺️  Use **simplified Chinese**、**traditional Chinese**、 **English**、 **Russian**、 **French**

🌁  Use any default theme within the application or any third-party theme, free theme customization

🖥  Customize the source folder and synchronize multiple devices using OneDrive, iCloud, Dropbox, etc.


🌱  Of course **Gridea** is still very young and has many shortcomings, but please believe it will keep moving forward 🏃

In the future, it will surely become your inseparable partner

Give full play to your talents！

😘  Enjoy~


## Development
If you want to contribute code, please check the [Contribution Guide](https://github.com/pgs666/gridea/wiki/%E8%B4%A1%E7%8C%AE%E6%8C%87%E5%8D%97) in advance.

``` shell
$ # Node version > v10.0.0 is requied
$ git clone https://github.com/pgs666/gridea.git
$ cd gridea
$ yarn
$ yarn electron:serve
$ yarn electron:build
```


## Contact
[Telegram Channel](https://t.me/joinchat/AAAAAEj82_lma0Y1wmyqUQ) | [Telegram Group](https://t.me/joinchat/IDY0ahRqb8NPodv95BNpBg)  | QQ 1 Group: 970332209 | QQ 2 Group: 923131213 | Author Twitter: @EryouHao


## Example Screenshots
<div align="center">
  <img src="./files/themes.png">
</div>


## Contributions
We welcome all contributions. You can submit any ideas as [pull requests](https://github.com/pgs666/gridea/pulls) or as GitHub [issues](https://github.com/pgs666/gridea/issues).   


## Donation
<div>
  <img src="./files/wechat.png" width="240px">
</div>


## License
[MIT](https://github.com/pgs666/gridea/blob/master/LICENSE). Copyright (c) 2020-2023 EryouHao
