# Statement
Determine how to invoke the preprocessor, compiler, assembler, and
linker manually in your local computing environment. Compile a
small complete program that computes a simple expression, and ex-
amine the output at each stage. Are you able to follow the flow of
the program in each form?
# Solution
Compilation steps for `gcc`:
```tikz
\usepackage{tikz-cd}
\usepackage{amsmath}
\begin{document}
\begin{tikzcd}[sep=3em]
\boxed{\large\substack{
	\text{Source}\\
	\texttt{(.c)}}
}
	\arrow[r, "\substack{
	\text{Preprocess}\\
	\texttt{gcc -E}}"]
& \boxed{\large\substack{
	\text{Expanded}\\
	\text{Source}\\
	\texttt{(.i)}}
}
	\arrow[r, "\substack{
	\text{Compile}\\
	\texttt{gcc -S}}"]
& \boxed{\large\substack{
	\text{Assembly}\\
	\texttt{(.i)}}
}
	\arrow[r, "\substack{
	\text{Assemble}\\
	\texttt{gcc -c}}"]
& \boxed{\large\substack{
	\text{Machine}\\
	\text{Code}\\
	\texttt{(.o)}}
}
	\arrow[r, "\substack{
	\text{Link}\\
	\texttt{gcc}}"]
& \boxed{\large\substack{\text{Executable}\\\texttt{(.out)}}}
\end{tikzcd}
\end{document}
```
