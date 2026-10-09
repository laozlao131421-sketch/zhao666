用 GitHub 搭一个无服务器博客 —— 配套文件
========================================

解压后，你会看到这些文件和文件夹，它们和 GitHub 仓库的结构是一一对应的：

  hugo.toml                        → 放到仓库根目录
  .gitignore                       → 放到仓库根目录
  .github/workflows/hugo.yml       → 放到 .github/workflows/ 这一层
  assets/css/extended/custom.css   → 放到 assets/css/extended/ 这一层
  content/about.md                 → 放到 content/
  content/archives.md              → 放到 content/
  content/search.md                → 放到 content/
  content/posts/*.md               → 放到 content/posts/

也就是说：解压出来之后，直接把里面的东西按同样的层级拖进 GitHub 仓库就行。

提醒两点
--------
1. Windows 资源管理器默认不显示以「点」开头的文件和文件夹。
   上传前先点「查看」→ 勾上「隐藏的项目」，否则 .github 和 .gitignore 看不到、也选不中。

2. hugo.yml 必须放在 .github/workflows/ 里面，不能直接丢在仓库根目录。
   放错了 GitHub 就不会自动生成网页。
