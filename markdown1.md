# 基本撰写和格式语法
  ## 标题
    要创建标题，请在标题文本前添加一至六个 # 符号。 您使用的 # 数量将决定标题的大小。
    例：
    # 一级标题
    ## 二级标题
    ......
    ###### 末级标题
    
  ## 样式文本
    
   |      样式      |      语法      |               键盘快捷键               |            示例            |
   |:--------------:|:--------------:|:--------------------------------------:|:--------------------------:|
   |粗体            |** **或__ __    |Command+B(Mac) or Ctrl+B(Windows/Linux) |**这是粗体文本**            |
   |斜体            |* *或_ _        |Command+I(Mac) or Ctrl+I(Windows/Linux) |_这是斜体文本_              |
   |删除线          |~~ ~~           |                                        |~~这是错误文本~~            |
   |粗体和嵌入的斜体|** **和_ _      |                                        |**此文本 _非常_ 重要**      |
   |全部粗体和斜体  |*** ***         |                                        |***所有文本都非常重要***    |
  
  ## 引用文本
    您可以使用“ > ”来引用文本。
    例：
Text that is not a quote
> Text that is a quote

  ## 引用代码
    使用单反引号“ ` ` ”可标注句子中的代码或命令。快捷键Command+E(Mac) or Ctrl+E(Windows/Linux)。
    例：
使用 `git status` 列出尚未提交的所有新文件或已修改文件。
    
    要将代码或文本格式化为各自的不同块，请使用三反引号。
    例：
一些基本的 Git 命令为：
```
git status
git add
git commit
```

  ## 链接
    通过将链接文本包含在方括号“ [ ] ”内，然后将 URL 包含在括号“ ( ) ”内，可创建内联链接。
    例：
本站点是使用 [GitHub Pages](https://pages.github.com/) 构建的。

  ## 章节链接
    您可以直接链接到渲染文件中的某个部分，方法是将鼠标悬停在该部分标题上以显示链接。
    
  ## 相对链接
    您可以在渲染的文件中定义相对链接和图像路径，以帮助读者导航到仓库中的其他文件。
    相对链接是相对于当前文件的链接。 例如，如果在仓库根目录下有一个自述文件，
    而在 /quickstart.md 中有另一个文件，则自述文件中的 quickstart.md 的相关链接如下所示：
   [快速入门](/quickstart.md)
    GitHub 将根据您当前使用的分支自动转换相对链接或图像路径，从而使链接或路径始终有效。 您可以使用所有相对链接操作符，如 ./ 和 ../。
    相对链接更便于用户克隆仓库。 绝对链接可能无法用于仓库的克隆 - 建议使用相对链接引用仓库中的其他文件。
    
  ## 图像
    您可以通过添加 ! ，然后将替代文本包含在 [] 内，再将图像链接包装在括号 () 中。
    例：
   ![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)
    
    GitHub 支持将图像嵌入到您的议题、拉取请求、讨论、评论和 .md 文件中。 您可以从仓库显示图像、添加在线图像链接或上传图像。
   **提示**：想要显示仓库中的图像时，应该使用相对链接而不是绝对链接。
  
  ## 列表
    通过在一行或多行文本前面添加 - 或 * 可创建无序列表。
    例：
   - George Washington
   - John Adams
   - Thomas Jefferson
    
    要对列表排序，请在每行前面添加一个编号。
  1. James Madison
  2. James Monroe
  3. John Quincy Adams

  ## 嵌套列表
    通过在一个列表项下面缩进一个或多个其他列表项，可创建嵌套列表。
    要通过 GitHub 上的 web 编辑器或使用等宽字体的文本编辑器（例如 Atom）创建嵌套列表，您可以直观地对齐列表。 
    在嵌套列表项的前面键入空格字符，直至列表标记字符（- 或 *）位于其上方条目中第一个文本字符的正下方。
  1. first list item
     - first nested list item
       - second nested list item
    
  ## 任务列表
    要创建任务列表，请在列表前加上 - 和 空格 ，后跟 [ ] 。要将任务标记为已完成，请使用 [x] 。
 - [x] #739
 - [ ] Add delight to the experience when all tasks are complete :tada:

  ## 提及人员和团队
    您可以在 GitHub 上提及人员或团队，方法是键入 @ 加上其用户名或团队名称。 这将触发通知并提请他们注意对话。 
    如果您在编辑的评论中提及某人的用户名或团队名称，该用户也会收到通知。
    例：
   @Marous-LXB 对，就是我~
    
  ## 使用表情符号
    通过键入 :EMOJICODE: 可在您的写作中添加表情符号。
    例：
   :wave:
   
  ## 段落
    通过在文本行之间留一个空白行，可创建新段落。
    
  ## 脚注
    您可以使用 [^ ] 为您的内容添加脚注。
    注意：Markdown 中脚注的位置不会影响该脚注的呈现位置。 您可以在引用脚注后立即写脚注，脚注仍将呈现在 Markdown 的底部。
    例：
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2]. 

[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
  
You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.
    
  ## 忽略 Markdown 格式
    您可以在Markdown格式符前加 \ 来忽视Markdown格式。
    例：
   \*这是在倾斜格式符前加\的效果\*
   
  ## 禁用 Markdown 渲染
    当您查看Markdown文件时，您可以单击文件顶部的 <> 禁用Markdown渲染来查看文件的源码。
