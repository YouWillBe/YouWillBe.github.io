---
layout: post
title: 新博客搭建实录
---
Jekyll + Github搭建新博客

图片问题难以解决，最终还是用了七牛

![node](http://7xtfpb.com1.z0.glb.clouddn.com/post/node.png)
# 待续

### 1.标题
# h1
## h2
### h3
#### h4
##### h5

### 2.有序列表
1. dsadas
2. dsaa
1. list 1 item 1
 2. list 1 item 2 (indent 1 space)
  3. list 1 item 3 (indent 2 spaces)
   4. list 1 item 4  (indent 3 spaces)
    5. lazy text belonging to above item 4
^
1. aaa
2. dsa

### 3.无序列表
- dads
- dadas

dsadda
### 4.表格

|aaa|bbb
|:-:|-:
| |

|---
| Default aligned | Left aligned | Center aligned | Right aligned
|-|:-|:-:|-:
| First body part | Second cell | Third cell | fourth cell
| Second line |foo | **strong** | baz
| Third line |quux | baz | bar
|---
| Second body
| 2 line
|===
| Footer row

### 5.引用
> 第一行引用
>
> * 第二行
>
> 最后一行

### 6.代码块
    console.log('hello, world')

```ruby
def what?
  42
end
```

{% highlight ruby linenos %}
def what?
  42
end
{% endhighlight %}

### 7.数学公式

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

dasdas $$ 5 + 5 $$ dsadsa

### 8.链接
This is a [link](http://example.com){:hreflang="de"}

This is [a link](http://rubyforge.org) to a page.

A [link](../test "local URI") can also have a title.

And [spaces](link with spaces.html)!

This is a [reference style link][linkid] to a page. And [this]
[linkid] is also a link. As is [this][] and [THIS][].

[linkid]: http://www.example.com/ "Optional Title"

*some text*

_some text_

**some text**

__some text__

This is un*believe*able! This d_oe_s not work!

Use `<html>` tags for this.

Here is a literal `` ` `` backtick.
And here is ``  `some`  `` text (note the two spaces so that one is left
in the output!).

This is a Ruby code fragment `x = Class.new`{:.language-ruby}
