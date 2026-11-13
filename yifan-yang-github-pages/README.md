# Yifan Yang · 个人学术网站

这是一个可直接部署到 GitHub Pages 的英文静态网站。用浏览器打开 `index.html` 即可在本地预览。项目内已包含原站肖像、CV、求职论文 PDF 和字体，无需安装依赖。期刊、SSRN 和机构链接需要联网。

## 发布到 GitHub Pages

1. 登录 GitHub，创建一个公开仓库，命名为 `你的GitHub用户名.github.io`。如果同名仓库已存在，先检查仓库里现有的内容。
2. 解压 ZIP，用仓库页面的 **Add file → Upload files** 上传解压后的内容并提交到 `main`。确认打开仓库就能看到 `index.html`、`research.html`、`.nojekyll` 和 `assets/`，并且 `assets/` 保留了原有目录结构。如果上传时漏了 `.nojekyll`，可以在仓库根目录单独新建这个文件。
3. 打开仓库的 **Settings → Pages**。在 **Source** 选择 **Deploy from a branch**，分支选 `main`，目录选 `/(root)`，然后保存。
4. 部署完成后，在 **Settings → Pages** 点 **Visit site**。个人站地址格式为 `https://你的GitHub用户名.github.io/`。打开 Research 和两个 PDF，确认都能访问。

[GitHub Pages 建站文档](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) · [发布来源设置](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 更新内容

| 文件 | 用途 |
| --- | --- |
| `index.html` | 首页简介和求职论文入口 |
| `research.html` | 已发表论文、工作论文、进行中的研究及求职论文摘要 |
| `assets/yifan-yang-cv.pdf` | CV，可用同名 PDF 替换 |
| `assets/yifan-yang-job-market-paper.pdf` | 求职论文，可用同名 PDF 替换 |
| `assets/yifan-yang.jpg` | 个人肖像。替换时将两页图片的 `width`、`height` 改为新图片的尺寸 |
| `assets/site.css` | 颜色、字体和响应式布局 |

全站使用相对链接。文件名区分大小写，更新后提交到 `main` 即可触发重新部署。CV 沿用原站公开链接中的版本，包含原 PDF 上的联系方式。

## Google 搜索收录

页面已包含独立标题与描述，首页含人物结构化数据。正式地址确认后，可以在两页的 `<head>` 添加 `rel="canonical"` 链接，分别指向正式首页和 `research.html` 的完整 HTTPS 地址。然后在 [Google Search Console](https://search.google.com/search-console) 添加正式地址作为 **URL prefix** 资源，完成验证，再通过 **URL Inspection** 检查首页和 Research 页并申请收录。

[Google 的抓取与收录说明](https://developers.google.com/search/docs/crawling-indexing/ask-google-to-recrawl)

## 内容来源

- 简介、肖像、研究列表及 PDF 来自 [原首页](https://sites.google.com/view/yangyf/home) 和 [原 Research 页](https://sites.google.com/view/yangyf/home/research)。公开邮箱及个人资料页来自 [Stockholm School of Economics](https://research.hhs.se/esploro/profile/yifan_yang)。
- 将求职论文入口放在首页，Research 页的可展开摘要沿用论文 PDF。多分析者项目补上了 CV 中的 [项目链接](https://www.manydaughters.com/)。
- 发表信息以正式记录为准。daughters 论文使用期刊版标题并保留 SSRN 链接。Scientific Reports 论文同时标出 2026 卷期和 2025 年在线发表。Economic Inquiry 论文链接换为公开 DOI。Ploughs 论文中的 Alina Zeltikova 拼写按 SSRN 和 LSE 资料修正。 [期刊版标题](https://doi.org/10.1016/j.jebo.2026.107641) · [Scientific Reports 文章](https://www.nature.com/articles/s41598-025-33362-3) · [Economic Inquiry 文章](https://doi.org/10.1111/ecin.13217) · [LSE 名录](https://www.lse.ac.uk/economics/people/predocs)
- 双栏布局和衬线排版参考 [Dominik Wehr 的个人站](https://dominikwehr.github.io/)。Newsreader 字体的许可随项目附在 `assets/fonts/OFL.txt`。
