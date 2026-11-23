# Jingjing 的博客

用 Jekyll 搭建，托管在 GitHub Pages 上，免费。

## 文件说明

```
_config.yml          网站名称、简介、作者等设置（先改这个）
_posts/              所有文章，一篇文章一个 .md 文件
about.md             “关于我”页面
assets/css/main.css  样式（改 --page-accent 就能换主色）
assets/images/       放文章图片（需要时自己新建）
_layouts/            页面模板，一般不用动
index.html           首页
archive.html         归档页
404.md               找不到页面时显示的内容
```

## 发布到网上（第一次）

1. 注册 GitHub 账号：https://github.com/signup
2. 右上角 **+** → **New repository**
   - Repository name 填 `你的用户名.github.io`（例如用户名是 jingjing，就填 `jingjing.github.io`）
   - 选 **Public**，点 **Create repository**
3. 在新仓库页面点 **uploading an existing file**
   （或者 **Add file → Upload files**）
4. 把解压后 `blog` 文件夹**里面的所有文件和文件夹**拖进去（不要拖 `blog` 文件夹本身），点 **Commit changes**
5. 进入仓库 **Settings → Pages**，确认 Source 是 **Deploy from a branch**，Branch 是 **main** / **(root)**
6. 等 1～3 分钟，打开 `https://你的用户名.github.io` 就能看到网站了
7. 回到仓库，打开 `_config.yml`，点铅笔图标编辑，把 `url: ""` 改成 `url: "https://你的用户名.github.io"`，提交

部署进度可以在仓库的 **Actions** 标签里看到，绿色对勾表示已经上线。

## 写一篇新文章

1. 在仓库里进入 `_posts` 文件夹，点 **Add file → Create new file**
2. 文件名格式：`年-月-日-英文短名.md`，例如 `2026-12-01-reading-notes.md`
   （英文短名会出现在网址里，用英文和减号，不要用中文和空格）
3. 文件开头写上：

   ```
   ---
   title: 文章标题
   description: 一句话简介（会显示在首页）
   tags: [读书笔记]
   ---

   正文从这里开始……
   ```

4. 点 **Commit changes**，1～3 分钟后网站自动更新

格式写法见文章《写文章速查：这个博客支持的所有格式》。

## 删除示例文章

进入 `_posts`，点开示例文件，右上角 **⋯ → Delete file**，提交即可。
