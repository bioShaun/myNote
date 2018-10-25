- [Org-mode](#org0e2f0d9)
  - [Table](#org57ee211)
  - [Tag](#orgf8a3f48)
    - [title](#org84d55d4)
  - [Markup for rich export](#org94895d2)
    - [Code](#org3f9ebfe)



<a id="org0e2f0d9"></a>

# Org-mode


<a id="org57ee211"></a>

## Table

1.  输入表头 "|Name|Phone|money|usage|left|"
2.  tab
3.  输入表格内容

| Name    | Phone       | money | usage | left |
|------- |----------- |----- |----- |---- |
| jason   | 13981231213 | 1     | 0     | 1    |
| alicehh | -           | 123   | 23    | 100  |
| bbq     | 87636743    | 23    | 12    | 11   |

-   自动计算，输入money, usage两列值，在left 输入 "=$3-$4", \`C-u C-c C-c\`, 自动计算所有left值
-   \`C-c |\`: 通过输入行x列的方式插入表格
-   tab: 下一格
-   enter: 下一行
-   \`M-up/right/left/right\` 上下左右移动行（列）


<a id="orgf8a3f48"></a>

## Tag

-   \`C-c C-q\` 为标题添加标签


<a id="org84d55d4"></a>

### title     :work:learn:life:

1.  sub     :fun:


<a id="org94895d2"></a>

## Markup for rich export


<a id="org3f9ebfe"></a>

### Code

1.  <s 再按TAB键 ，就会自动展开为 #+BEGIN<sub>SRC</sub> &#x2026; #+END<sub>SRC</sub>
2.  将光标移到代码块内，按C-c C-c，org-mode会自动生成结果

```python
a = 1 + 1
print a
```
