# Markdown Basic Command

## Markdown 列表语法
**有序列表**

要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

1. First item
2. Second item
3. Third item
4. Fourth item

**无序列表**

要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。

- First item
- Second item
- Third item
- Fourth item

**在列表中嵌套其他元素**

要在保留列表连续性的同时在列表中添加另一种元素，请将该元素 ***缩进四个空格或一个制表符***，如下例所示：

段落:

*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.

引用块:

*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.

代码块:

代码块通常采用四个空格或一个制表符缩进。***当它们被放在列表中时，请将它们缩进八个空格或两个制表符***。

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

图片：

1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Wechat app icon](wechat.png)

3.  Close the file. 


列表：

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item


## Markdown 代码语法

要将单词或短语表示为代码，请将其包裹在反引号 (`) 中：

At the command prompt, type `nano`.

如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(``)中：

``Use `code` in your Markdown file.``

**代码块**

要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

    # include <iostream>
    using namespace std;

    int main()
    {
        cout<<"Hello world!"<<endl;
        return 0;
    }

## Markdown 围栏代码块

Markdown基本语法允许您通过将行缩进四个空格或一个制表符来创建代码块。如果发现不方便，请尝试使用受保护的代码块。根据Markdown处理器或编辑器的不同，您将在代码块之前和之后的行上使用三个反引号（```）或三个波浪号（~~~）。

```
# include <iostream>
using namespace std;

int main()
{
    cout<<"Hello world!"<<endl;
    return 0;
}
```

**语法高亮**

许多Markdown处理器都支持受围栏代码块的语法突出显示。使用此功能，您可以为编写代码的任何语言添加颜色突出显示。要添加语法突出显示，请在受防护的代码块之前的反引号旁边指定一种语言。


```C++
# include <iostream>
using namespace std;

int main()
{
    cout<<"Hello world!"<<endl;
    return 0;
}
```


## Markdown 分割线语法

要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。

Try to put a blank line before...

---

...and after a horizontal rule.


## Markdown 链接语法

链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`


> 这是一个链接 [Markdown语法](https://markdown.com.cn)。

**网址和Email地址**

使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

<https://markdown.com.cn>  
<fake@example.com>

许多Markdown处理器会自动将URL转换为链接,即使您***未使用方括号***，您的Markdown处理器也会自动将其转换为链接。

http://www.example.com

如果您不希望自动链接URL，则可以通过将URL表示为带反引号的代码来删除该链接。

`http://www.example.com`


**带格式化的链接**

强调链接, 在链接语法前后增加星号。 

I love supporting the **[EFF](https://eff.org)**.  
This is the *[Markdown Guide](https://www.markdownguide.org)*. 

要将链接表示为代码，请在方括号中添加反引号。 

See the section on [`code`](test_code.py).

链接到标题ID

See the section on [Basic Command](#markdown-basic-command)



**引用类型链接**

引用样式链接是一种特殊的链接，链接分为两部分：与文本保持内联的部分以及存储在文件中其他位置的部分，以使文本易于阅读。

内联部分:

霍比特人百科 [hobbit-hole][1]

链接部分：
可以将链接放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）。

[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle

## Markdown 图片语法

要插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`，图片title为可选。

**链接图片**

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

[![wechat icon](wechat.png "WeChat")](https://markdown.com.cn)


## Markdown 删除线

若要删除单词，请在单词前后使用两个波浪号`~~`。

~~世界是平坦的。~~ 我们现在知道世界是圆的。

## Markdown 任务列表语法

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media


## Markdown 引用语法

要创建块引用，请在段落前添加一个`>`符号。

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

**嵌套块引用**

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

**带有其它元素的块引用**

> The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## Markdown 表格

要添加表，请使用三个或多个连字符（---）创建每列的标题，并使用管道（|）分隔每列。您可以选择在表的任一端添加管道。

| Syntax      | Description |
| ----------- | ------------|
| Header      | Title       |
| Paragraph   | Text        |

**对齐**

您可以通过在标题行中的连字符的左侧，右侧或两侧添加冒号（`:`），将列中的文本对齐到左侧，右侧或中心。

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |


**Tip:** 使用连字符和管道创建表可能很麻烦。为了加快该过程，请尝试使用使形界面构建表格[Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)


## Markdown 使用 Emoji 表情

在大多数情况下，您可以简单地从[Emojipedia](https://emojipedia.org/) 等来源复制表情符号并将其粘贴到文档中。许多Markdown应用程序会自动以Markdown格式的文本显示表情符号。

❄️ ☃️ ❄️ ☃️ ❄️ ☃️ ❄️ ☃️ ❄️ ☃️ ❄️ ☃️

⚡ 🔥 ⚡ 🔥 ⚡ 🔥 ⚡ 🔥⚡ 🔥 ⚡ 🔥


