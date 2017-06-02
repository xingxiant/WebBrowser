# WebBrowser
超简洁的web浏览器，只能识别html文件
> 核心模块就是JEditorPane
> JEditorPane的最主要功能在于展 现不同类型的文件格式内容。JEditorPane支持的文件类型有三种:第一种是纯文本类型，其类型的表示法为"text/plain",这种类型 的文件就是我们最常使用的txt文件，这类型的文件可以用记事本或WordPad等文书编辑软件来编辑。第二种是RTF类型，其表示法 为"text/rtf",这种类型的文件特色是能对文字内容做字体缩放、变形、上色等特殊效果。第三类是HTML类型，也就是我们在网络上 所浏览的网页类型，其表示法为"text/html",这类文件的特色相信大家都非常的清楚，除了在对字体效果的表现之外还具有在文件 内加入图片、超级链接等相关功能。但是JEditorPane并不是一个全功能的Web Browser,它仅能支持简单的HTML语法.JEditorPane支 持HTML类型的文件最主要的用途是用来制作在线辅助说明文件。 
> 使用的函数：
void javax.swing.JEditorPane.setPage(URL page) throws IOException

```
/*核心代码*/
//新建一个显示板
textPane = new JEditorPane(); 
//将JEditorPane设为不可编辑,这行是相当重要的，若是我们将这个方法设为true,我们将会失去HTML文件本身的特性，如超级链接的功能等等
textPane.setEditable(false);
//选择你要显示的页面，page为目标页面的url 
textPane.setPage(new URL("page"));
```
效果展示：


![Markdown](http://i1.piimg.com/1949/bc6bedb72382770d.png)
