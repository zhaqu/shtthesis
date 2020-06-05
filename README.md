# ShangHaiTech university THESIS (shtthesis)

`shtthesis` project, forked from [`ucasthesis`](https://github.com/mohuangrui/ucasthesis), is an **unofficial** LaTeX thesis template for ShanghaiTech University and satisfies all format requirements in 《上海科技大学研究生学位论文撰写规范（初稿）》. The user just need to set `\documentclass{shtthesis}` and to setup mandatory information via `\shtsetup`, then his or her thesis document will be typeset properly:
```latex
\documentclass{shtthesis}

\shtsetup{
  title = {论文标题},
  title* = {Title~of~Thesis},
  author = {作者姓名},
  author* = {Name~of~Author},
  % ...
}

\begin{document}
% ...
```

## Get the Template
- Stable version:
  - GitHub Release: please refer to [release](https://github.com/lirundong/sht-thesis/releases) page, and download required files based on release information;
  - CTAN: TODO
- Develop version: directly clone the GitHub repo
  ```bash
  git clone https://github.com/lirundong/sht-thesis.git
  ```

## Get Started

After cloning or downloading this template, please

0. Install a modern TeX distribution **in full scheme**:
   - Windows or Linux: [TeX Live](https://www.tug.org/texlive/)
   - macOS: [MacTeX](https://www.tug.org/mactex/)
1. Open your terminal (CMD for Windows users) and switch to this directory, compile this template by `latexmk` tool with LuaLaTeX or XeLaTeX engine (**note**: pdfLaTeX is not supported):
   ```bash
   latexmk -pdflua
   # if you prefer XeLaTeX engine:
   # latexmk -pdfxe
   ```
   the output file shtthesis-user-guide.pdf is the compiled user guide document
2. We strongly recommend you to skim though the compiled user guide, or the [pre-compiled version](shtthesis.pdf)
3. Open the document source file [shtthesis-user-guide.tex](shtthesis-user-guide.tex) and enjoy TeXing :smirk:

## License

`shtthesis` project is licensed under GNU Public License V3, see [LICENSE](LICENSE) for details.
