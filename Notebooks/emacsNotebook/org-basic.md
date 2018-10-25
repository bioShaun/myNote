# Org-mode Basic


## Table

1.  输入表头 "|Name|Phone|money|usage|left|"。
2.  `tab` 生成表格。
3.  输入表格内容。

| Name  | Phone       | money | usage | left |
|----- |----------- |----- |----- |---- |
| jason | 13981231213 | 1     | 0     | 1    |
| alice | -           | 123   | 23    | 100  |
| bobby | 87636743    | 23    | 12    | 11   |

-   自动计算，输入money, usage两列值，在left 输入 `=$3-$4`, `C-u C-c C-c`, 自动计算所有left值。
-   `C-c |`: 通过输入行x列的方式插入表格。
-   `tab` 跳转至下一格。
-   `enter` 跳转至下一行。
-   `M-up/right/left/right` 上下左右移动行（列）。


## Tag

-   `C-c C-q` 为标题添加标签。


### title     :work:learn:life:

1.  sub     :fun:


## Markup for rich export


### Code

1.  输入 `<s` 再按 `tab` 键 ，就会自动展开为 ~#+BEGIN\_SRC &#x2026; #+END\_SRC~。
2.  将光标移到代码块内，输入 `C-c C-c` ，org-mode会自动生成结果。

```python
a = 1 + 1
print a
```

```python
2
```


## export


### options

-   `#+OPTIONS: ^:nil`: 禁用下划线转义。
-   `#+OPTIONS: toc:nil`: 不生成目录。


### to markdown

-   install `ox-gfm` by `M-x package-install ox-gfm`.
-   exporting can be triggered by calling the (autoloaded) function `M-x org-gfm-export-to-markdown`.
