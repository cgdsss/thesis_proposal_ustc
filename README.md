# thesis_proposal_ustc
中国科学技术大学开题报告LaTeX模板，修改自：[哈工大开题报告论文XeLaTeX模板](https://github.com/dustincys/PlutoThesisProposal)
- 使用 xelatex 编译 [main.tex](main.tex)
- [pdf实例效果](pdf/效果实例.pdf)模仿[学校官方的word样式](pdf/35.doc)
- 主要文件
    - [main.tex](main.tex) : 主要报告正文内容
    - [cover.tex](cover.tex) : 报告封面内容
    - [reference.bib](reference.bib) : BibTeX格式参考文献
- 官方模板的页面边框  
    每页加入tikzpicture部分（注意放在不影响排版的位置），具体每页上下偏移可能需要微调
    ```tex
    \begin{tikzpicture}[overlay,remember picture]
    \draw [line width=0.8pt]
        ($ (current page.north west) + (1.8cm,-2.3cm) $)
        rectangle
        ($ (current page.south east) + (-1.8cm,2.5cm) $);
    \end{tikzpicture}
    ```
- 欢迎提交改进