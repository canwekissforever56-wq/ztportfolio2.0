# GitHub Pages 上传说明

## 必须保留的目录结构

上传到 GitHub 仓库根目录时，请保持下面结构不变：

```text
portfolio-video-background-scroll/
├─ index.html
├─ game-ui-demo.mp4
├─ assets/
│  ├─ scene-1.mp4
│  ├─ scene-2.mp4
│  ├─ scene-3.mp4
│  ├─ scene-4.mp4
│  ├─ scene-5.mp4
│  ├─ portrait-zengting.jpg
│  ├─ *.ttf
│  ├─ pdf.min.mjs
│  └─ pdf.worker.min.mjs
└─ pdf/
   ├─ same_freq_app.pdf
   ├─ ui_design_guidelines.pdf
   ├─ b_end_ai_platform.pdf
   └─ ai_coding_product.pdf
```

不要把 `assets` 里的文件散着上传到仓库根目录。`index.html` 里的视频、字体和 PDF 渲染脚本都依赖这些相对路径。

## 推荐上传方式

GitHub 网页端一次拖整个大文件夹经常失败，建议使用 GitHub Desktop 上传整个项目目录。

1. 安装并登录 GitHub Desktop。
2. File -> Add local repository。
3. 选择这个文件夹：`D:\claude code\作品网站\portfolio-video-background-scroll`
4. 如果提示不是 Git 仓库，选择 create a repository。
5. Commit to main。
6. Publish repository。
7. 打开 GitHub 仓库 Settings -> Pages。
8. Source 选择 `Deploy from a branch`。
9. Branch 选择 `main`，文件夹选择 `/root`。
10. 保存后等待 1-3 分钟，GitHub 会生成网址。

## 如果继续用网页上传

可以分批上传，但必须先在 GitHub 页面中进入或创建对应文件夹：

- `index.html` 和 `game-ui-demo.mp4` 上传到仓库根目录。
- `assets` 里的文件必须上传到 GitHub 仓库的 `assets` 文件夹内。
- `pdf` 里的文件必须上传到 GitHub 仓库的 `pdf` 文件夹内。

如果把 `scene-1.mp4` 这类文件直接传到根目录，页面会打开，但背景视频不会显示。
