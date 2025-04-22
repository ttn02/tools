# 插件

- Chinese(Simplified) 官方
- Fitten Code: Faster and Better AI Assistant
- Tailwind CSS IntelliSense
- Vue - Official vue官方插件
- vscode-icons 图标优化
- Error Lens 语法错误提醒
- Image preview 导入图片时鼠标放在上面显示图片内容
- Prettier - Code formatter 代码格式化扩展，保存时格式化代码
- Remote - SSH  【SSH连接】连接远程服务器或虚拟机



# 快捷键

- `crl + D` 删除行
- `alt + (数字)` 切换tab
- `alt + 鼠标单击` 在多个地方输入
- `alt + 上下键` 移动选中行进行上下行移动

# VsCode系统文件配置

`settings.json`其中的一些基础配置（点击左下角设置，在搜索框中输入如下关键词，或者是点击右上角<img src="C:\Users\ttn\Desktop\project\image\vscode文件配置\1.png" style="zoom: 33%;" />进入配置文件添加设置)

~~~js
{
  "fittencode.languagePreference.displayPreference": "zh-cn",
  "fittencode.languagePreference.commentPreference": "zh-cn",
  "workbench.startupEditor": "none",
  "explorer.confirmDelete": false,
  "[vue]": {
    "editor.defaultFormatter": "Vue.volar"
  },
  "git.openRepositoryInParentFolders": "never",
  "files.autoGuessEncoding": true,
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "editor.cursorBlinking": "smooth",
  "terminal.integrated.smoothScrolling": true,
  "workbench.list.smoothScrolling": true,
  "editor.mouseWheelZoom": true,
  "editor.formatOnPaste": true,
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
  "editor.guides.bracketPairs": true,
  "window.dialogStyle": "custom",
  "debug.showBreakpointsInOverviewRuler": true,
  "workbench.iconTheme": "material-icon-theme",
  "git.autofetch": true,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "notebook.defaultFormatter": "esbenp.prettier-vscode",
  "prettier.bracketSameLine": true,
  // "background.editor": {
  //   "useFront": true,
  //   "style": {
  //     "background-position": "55% 20%",
  //     "background-size": "auto",
  //     "opacity": 0.4
  //   },
  //   "styles": [{}, {}, {}],
  //   "images": ["https://w.wallhaven.cc/full/5g/wallhaven-5ge715.jpg"],
  //   "interval": 0,
  //   "random": false
  // },
  "background.fullscreen": {
    "images": [
      "https://w.wallhaven.cc/full/5g/wallhaven-5ge715.jpg"
    ],
    "opacity": 0.15,
    "size": "cover",
    "position": "center",
    "interval": 0,
    "random": false
  },
  "workbench.colorTheme": "One Dark Pro Night Flat",
  "vue.autoInsert.dotValue": true,

  "prettier.singleAttributePerLine": true,
  "prettier.printWidth": 80,
  "prettier.requireConfig": true,
  "html.format.wrapAttributes": "force-expand-multiline",
  "background.enabled": false

  
}

~~~

