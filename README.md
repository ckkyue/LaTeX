# LaTeX
This repository contains a collection of LaTeX templates. The folder names are self-explanatory. The primary goal of establishing this repository is to assist others in avoiding minor, yet vexing issues that I have personally encountered while using LaTeX.
# Important
It is recommended to use Overleaf to prevent problems related to command configuration and package management. If you wish to compile a .tex file on your local computer, please be aware of the following:
1. The .tex filename should not include any spaces.
2. When drawing Feynman diagrams using the feynmp-auto package, you should use
```latex
\usepackage[force]{feynmp-auto} %<-added force
```
If you are using TeXstudio, please change the command of Pdflatex to 
```bash
pdflatex -shell-escape -synctex=1 -interaction=nonstopmode %.tex
```
3. When including figures in a report, it is helpful to use
```latex
\begin{figure}[H]
...
\begin{figure}[!ht]
...
\begin{figure}[!htbp]
...
```
These syntax options provide flexibility in determining the positions of the figures in a report.

4. Most of the content in the "RevTeX 4.2 Template and Sample" folder are from https://www.overleaf.com/latex/templates/revtex-4-dot-2-template-and-sample/yydsrzvrqrzs. The apssamp.tex and apssamp.bib files have been modified.
