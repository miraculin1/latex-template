# 科研调研汇总模板

紧凑单栏中文模板，基于 `ctexart`，使用 XeLaTeX 编译。首页左上角为大标题，标题下留一段空白后直接进入正文。

## 编译

```bash
xelatex main.tex
xelatex main.tex
```

需要参考文献时，取消 `main.tex` 末尾两行注释，在 `refs.bib` 中添加条目，然后按 `xelatex → bibtex → xelatex ×2` 编译。

## 文件

- `main.tex`：全部版式与正文。
- `refs.bib`：参考文献条目（可选）。

## 常用调整

| 需求 | 位置 |
|---|---|
| 字号 | `\documentclass[...11pt...]` |
| 页边距 | `geometry` |
| 行距 | `\linespread{1.15}` |
| 标题后空白 | `\maketitle` 中的 `\vspace{1.4\baselineskip}` |
| 章节间距 | `\ctexset` 中的 `beforeskip` / `afterskip` |
