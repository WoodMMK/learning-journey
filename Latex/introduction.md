# My LaTeX Notes

## Resources
[overleaf tutorial](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#What_is_LaTeX?)

## LaTeX Commands
### Preamble (before body)
- `\documentclass{'class'}` i.e. resume, report, article, book, etc.
- `\documentclass[fontsize('00pt'), 'paperSize']{'class'}`
- `\title{'document name'}`
- `\maketitle` typeset title
- `\author{'fullname'}`
- `\date{in any format}`

### Body Commands
new line and new paragraph
- press 'enter' twice
newline but still in same paragraph
- use `\\` 

more spaces between paragraph
```latex
\usepackage{parskip}
```

before adding images in project
- `\usepackage{graphicx}` include external package
- `\graphicspath{{'foldername'}}` set filepath



create figure block
```latex
\begin{figure}[h] % start figure block
    \centering % set center
    \includegraphics[width=0.75\textwidth]{'filename'} % add 'filename' image with width = 0.75 of text area 
    \caption{A nice plot.}  % caption under image
    \label{fig:mesh1} % variable that represent this block
\end{figure}
```

create unordered list
```latex
\begin{itemize} % start unordered list block
  \item first item
  \item second item
\end{itemize}
```

start inline mode
- `\( equation \)` or `$ equation $ ` or open with `\begin{math}` and end with `\end{math}`.
