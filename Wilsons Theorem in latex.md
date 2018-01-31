\documentclass{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}

\title{Wilsons Theorem}
\date{\vspace{-5ex}}
\begin{document}

\maketitle

\section{Theorem:}
Wilsons Theorem states that if integer $p>1$, then $(p-1)! + 1$ is divisible by p if and if only if p is prime.
\section{Proofs}
Suppose first that p is composite. Then p has a factor $d>1$  that is less than or equal to p-1. Then d divides $(p-1)!$ , so $d$ does not divide $(p-1)! + 1$. Therefore $p$ does not divide $(p-1)! + 1$.\\
Two proofs of the converse are provided: an elementary one that rests close to basic principles of modular arithmetic, and an elegant method that relies on more powerful algebraic tools.
\\\\
\subsecion{Elementary Proof}
Suppose $p$ is a prime. Then each of the integers $1, . . . , p-1$ has an inverse modulo $p$. This inverse is unique, and each number is the inverse of its inverse. If one integer $a$ is its own inverse then:
\begin{equation*}
    0 \equiv a^2 - 1 \equiv (a-1)(a+1) \quad {(mod\  p)}
\end{equation*}
so that $a \equiv 1$ or $a \equiv p-1$. Thus we can partition the set $\{2, . . . , p-2\}$ into pairs ${a,b}$ such that $ab \equiv 1 (mod\ p)$. It follows that $(p-1)$ is the product of these pairs times $1\cdot(-1)$. Since the product of each pair is congruent to 1 modulo $p$ we have
\begin{equation*}
    (p-1)! \equiv 1\cdot1\cdot(-1) \equiv -1 \quad (mod\ p),
\end{equation*}
as desired.
\subsection{Algebraic Proof}
Let $p$ be a prime. Consider the field of integers modulo $p.$ By Fermat's Little Theorem, every nonzero element of this field is a root of the polynomial
\begin{equation*}
    P(x)\ =\ x^{p-1} - 1.
\end{equation*}
Since this field has only $p-1$ nonzero elements, it folows that
\begin{equation*}
    x^{p-1} -1 = \prod_{r=1}^{p-1}{(x-r)}.
\end{equation*}
Now, either $p=2$, in which case $a \equiv -a\quad (mod\ 2)$ for any integer $a$, or $p-1$ is even. In either case, $(-1)^{p-1} \equiv 1\quad (mod\ p)$, so that
\begin{equation*}
    x^{p-1}-1 = \prod_{r=1}^{p-1}(x-r)=\prod_{r=1}^{p-1}(-x+r).
\end{equation*}
If we set $x$ equal to $0$, the theorem follows.
\\
\section*{References}
$ 1.\ https://artofproblemsolving.com/wiki/index.php?title=Wilson%27s_Theorem $
\end{document}
