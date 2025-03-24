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
  // 自动切换编码类型
  "files.autoGuessEncoding": true, 
      
  // 使光标移动更加丝滑
  "workbench.list.smoothScrolling": true,
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "editor.cursorBlinking": "smooth",
  
  // crl + 鼠标滚轮 进行视图缩放
  "editor.mouseWheelZoom": true,
   
  // 格式化代码设置
  "editor.formatOnPaste": true,
  "editor.formatOnType": true,
  "editor.formatOnSave": true,
      
  // 自动折行，会把挤出去的代码显示到下一行，不改变行号
  "editor.wordWrap": "on",
      
  // 彩虹括号
  "editor.guides.bracketPairs": true,
  //"editor.bracketPairColorization.enabled": true, (此设置vscode在较新版本已默认开启)
  
  // 代码补全，如有其它代码补全工具，可不开启
  "editor.suggest.snippetsPreventQuickSuggestions": false,
  "editor.acceptSuggestionOnEnter": "smart",
  "editor.suggestSelection": "recentlyUsed",
   
  // 应用的主题风格习惯
  "window.dialogStyle": "custom",
      
  // 断点设置更明显，会在最右边的滚动条中显示，方便更快的定位断点位置
  "debug.showBreakpointsInOverviewRuler": true,
}

~~~

