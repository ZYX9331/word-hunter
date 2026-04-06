# Word Hunter 项目记忆

## 项目基本信息
- 路径：`c:\Users\ZYX\Desktop\word-hunter\`
- 文件：`word-hunter-v4.html`（单文件纯前端），`cet4-high-frequency-words.csv`（词库）
- 定位：上传 GitHub Pages，主要面向手机用户在线使用

## 技术约定
- 纯 HTML + CSS + JS，无框架无构建，字体用 Google Fonts
- 格子字母小写显示（`text-transform: lowercase`）
- 单词存储为小写字符串
- CSV 格式支持 CET4 带词性前缀（`parseCET4Meanings()` 负责提取纯中文）
- 找到单词动效：格子变色 + pop 弹跳，无删除线

## CSV 格式说明
- 支持：`word,释义` 或 `word,v. 放弃，抛弃` 或 `book,书|书本|书籍`
- `parseCET4Meanings()` 会去掉词性前缀，提取中文片段
