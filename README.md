# 商业系统实验室

本站由 GitHub Pages 从 `main` 分支发布。研究、目录、实践、关于和联系仍是原来的 HTML 页面。文章用 Markdown 编写，推送到 `main` 后由 GitHub Pages 自带的 Jekyll 自动生成，不需要另外配置构建。

## 如何写一篇新文章并发布

1. 新建文件，路径必须类似：

   `_posts/2026-11-02-decision-notes.md`

   - 文件名以日期开头：`年-月-日-英文短名.md`
   - 日期请用当天或过去的日期。写成未来日期时，文章不会出现在网站上
   - 文件名用英文和连字符。中文标题写在下面的文首信息里，不要写进文件名

2. 在文件最开头写文首信息（front matter），然后空一行，再写正文。正文是普通 Markdown。

   ```yaml
   ---
   title: 文章标题
   description: 用一两句话说明这篇写什么。这段会出现在文章列表和分享摘要里。
   kicker: 研究笔记
   ---
   ```

   - `title`：必填。文章标题。
   - `description`：建议填写。文章列表里显示的摘要。
   - `kicker`：选填。标题上方的短眉题，例如「研究笔记」。不写则显示「文章」。
   - 不用写 `layout`。站点会自动套用文章模板。

3. 发布可以任选一种方式。

   **在 GitHub 网页上：** 打开这个仓库 → Add file → Create new file → 文件名填成上面的路径 → 贴上内容 → Commit changes，分支选择 `main`。

   **在自己的电脑上：** 把文件放进 `_posts/`，保存后执行 `git add`、`git commit`、`git push`，推送到 `main`。

4. 推送后等待一两分钟。GitHub Pages 会自动构建。文章会出现在：

   - 列表：<https://sethhsu.com/articles/>
   - 正文：<https://sethhsu.com/articles/年/月/日/英文短名/>

   例如文件 `_posts/2026-11-02-decision-notes.md` 的地址是 <https://sethhsu.com/articles/2026/11/02/decision-notes/>。

5. `_posts/2026-10-16-sample-article.md` 是版式示例，不是研究结论。熟悉流程后可以删掉，也可以留着。

还没准备好的稿子可以放在 `_drafts/`，文件名不用加日期，但同样要有文首信息。草稿不会发布。要发布时，把文件移到 `_posts/`，并在文件名前加上日期。

修改已有文章：打开对应的 `.md` 文件，改完后提交到 `main` 即可。
