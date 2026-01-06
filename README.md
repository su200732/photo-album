# 我的GitHub相册

这是一个基于GitHub仓库的HTML相册，用于展示和分享照片。

## 仓库结构

```
photo-album/
├── README.md          # 说明文档
├── example1.jpg       # 示例照片1
├── example2.jpg       # 示例照片2
└── example3.jpg       # 示例照片3
```

## 如何使用

### 1. 上传照片到GitHub仓库

1. 登录GitHub，进入仓库：https://github.com/su200732/photo-album
2. 点击"Add file" -> "Upload files"
3. 选择要上传的照片文件
4. 填写提交信息，点击"Commit changes"

### 2. 获取照片的Raw URL

上传照片后，点击照片文件，然后点击"Download"按钮旁边的"Raw"按钮，即可获取照片的Raw URL。

Raw URL格式：
```
https://raw.githubusercontent.com/用户名/仓库名/分支/文件名
```

示例：
```
https://raw.githubusercontent.com/su200732/photo-album/main/example1.jpg
```

### 3. 更新HTML相册

编辑`index.html`文件，在`photos`数组中添加照片信息：

```javascript
const photos = [
    {
        id: 1,
        title: "照片标题",
        description: "照片描述",
        url: "照片的Raw URL"
    },
    // 添加更多照片...
];
```

### 4. 查看相册

直接在浏览器中打开`index.html`文件，即可查看相册。

## HTML相册功能

- 📱 响应式设计，适配各种设备
- 🖼️ 点击照片可放大预览
- 🔍 支持图片懒加载
- ✨ 美观的卡片式布局
- 🎯 平滑的动画效果

## 相册截图

![相册截图](https://raw.githubusercontent.com/su200732/photo-album/main/screenshot.jpg)

## 注意事项

1. 请确保照片文件大小适中，避免过大影响加载速度
2. 建议使用JPG或PNG格式的照片
3. 可以根据需要修改HTML和CSS样式，自定义相册外观
4. 如果相册访问速度较慢，可以考虑使用CDN加速

## 许可证

MIT
