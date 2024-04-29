# Tarea-2

\documentclass{article}
\usepackage[spanish]{babel}
\usepackage{pifont}
\usepackage{amsmath,amsthm,amsfonts}
\usepackage{latexsym,amssymb}
\usepackage{setspace}
\setstretch{1.5}
\usepackage{titlesec}
\usepackage{multicol}
\usepackage[a4paper, margin=1.8cm]{geometry}
\newtheorem{theorem}{Teorema}
\newtheorem{lemma}{Proposicion}
\newtheorem{definition}{Definición}
\newtheorem{corollary}{Corolario}
\renewcommand{\qedsymbol}{$\blacksquare$}
\usepackage{microtype}
\usepackage{xcolor}
\usepackage{enumitem}
\usepackage{graphicx}
\usepackage{natbib}


\title{CÁLCULO 1 - LÍMITES}
\Large
\author{Ervin Mauricio Lima Suxo}
\date{28 de abril de 2024}

\begin{document}
\maketitle

\section{\LARGE Introducción} La teoría de límites es indispensable conocer, puesto que es la base sobre el cuál se dan los conceptos fundamentales del cálculo como son: la continuidad, la derivada, la integral, etc. Antes de dar la definición de límite de una función daremos la idea intuitiva. \\ Sea L un número real y f una función definida en las proximidades del número c no necesaiamente en c y denotaremos por: $\lim_{x\rightarrow c} f(x)=L$. 
\begin{figure}[h]
  \centering
  \includegraphics[width=0.5\textwidth]{limiteEpsilonDelta.png}
  \label{fig:nlimiteEpsilonDelta}
\end{figure}
\\
Donde para todo $\epsilon $ cuando x se aproxima a c; f(x) se aproxima a L ó para x próximo a c; f(x) está próximo a L ó para x apoximadamente igual a c, f(x) es aproximadamente igual a L.\citep{espinoza2012grupo}
\\
\subsection{\large Definición}
Suponga que $L$ denota un número. El concepto de $f(x)$ que tiende a $L$ a medida que $x$ tiende a un número $a$ puede definirse informalmente así: Si $f(x)$ puede hacerse arbitrariamente próximo al número $L$ al tomar $x$ suficientemente cerca de, pero diferente de, un número $a$, por la izquierda y por la derecha de $a$, entonces el límite de $f(x)$ cuando $x$ tiende a $a$ es $L$.

  \textbf{Notación:} Por facilidad suele usarse el símbolo flecha ``$\rightarrow$'' para significar la palabra "tiende". Por tanto:
  \begin{enumerate}
    \item $x \rightarrow a^-$ indica que $x$ tiende al número $a$ por la izquierda, es decir, "$x$ está muy cercano a $a$ pero $x$ es menor que $a$, $x \approx a$, $x < a$.
    \item $x \rightarrow a^+$ indica que $x$ tiende al número $a$ por la derecha, es decir, "$x$ está muy cercano a $a$ pero $x$ es mayor que $a$, $x \approx a$, $x > a$.
    \item $x \rightarrow a$ indica que $x$ tiende al número $a$ por la izquierda y por la derecha, es decir, "$x$ está muy cercano a $a$ pero $x$ es diferente de $a$, $x \approx a$, $x \neq a$.
  \end{enumerate}

\subsection{\large Tipos de límites}

\subsubsection{\large Límite por la izquierda y derecha}
Suponga una función $f$ definida en un intervalo $(c, a)$. Decimos que el límite de $f$ cuando $x$ tiende a $a$ por la izquierda es $L$ si $f(x)$ se acerca a $L$ cuando $x$ se acerca a $a$ para valores $x$ menores a $a$. Esto se escribe como:

$\lim_{{x \to a^-}} f(x) = L$

Suponga una función $f$ definida en un intervalo $(a, c)$. Decimos que el límite de $f$ cuando $x$ tiende a $a$ por la derecha es $L$ si $f(x)$ se acerca a $L$ cuando $x$ se acerca a $a$ para valores $x$ mayores a $a$. Esto se escribe como:

$\lim_{{x \to a^+}} f(x) = L$

\begin{figure}[h]
  \centering
  \includegraphics[width=0.5\textwidth]{IS5b.png}
  \label{fig:IS5b}
\end{figure}

\subsubsection{\large Existencia o no de Límite} 
Es “pensable” que un límite (lateral o bilateral) puede no existir. Sin embargo, es
importante tener presente lo siguiente:
“La existencia de un límite de una función f cuando x tiende a a (lateral o bilateral) no depende de
si f está o no definida en a, sino únicamente de si f está definida para x cercanos del número a”

La función $f(x) = \frac{1}{x}$ tiene una asíntota vertical en $x = 0$ y una asíntota horizontal en $y = 0$, es decir:

$$\begin{tabular}{|c|c|c|c|c|c|c|c|c|c|c|c|}
\hline
     $x\rightarrow 0^+$& 0,1 & 0,01&0,001&0,0001&...&$x\rightarrow +\infty$&10&$10^2$&$10^3$&$10^4$&... \\
     \hline
     $f(x) = \frac{1}{x}$&10&$10^2$&$10^3$&$10^4$&...&$f(x) = \frac{1}{x}$&0,1 & 0,01&0,001&0,0001&... \\ 
     \hline
\end{tabular} $$

$$\lim_{{x \to 0^+}} f(x) = +\infty \quad \text{y} \quad \lim_{{x \to +\infty}} f(x) = 0^+.$$

Como $f(-x) = -f(x)$, es decir, $f(x)$ es una función impar, entonces:

$$\lim_{{x \to 0^-}} f(x) = -\infty \quad \text{y} \quad \lim_{{x \to -\infty}} f(x) = 0^-.$$

Por tanto, $f$ no está definida en $x = 0$ y además $\lim_{{x \to 0}} f(x)$ no existe.\citep{villalimites}

\subsubsection{\large Límites al infinito}
De manera intuitiva, el límite de una función real en el infinito (o en el menos infinito) es el valor al que se aproxima la función (es decir, su coordenada y) a medida que la coordenada x se hace "más y más grande".\citep{ayres1991calculo}

\begin{figure}[h]
  \centering
  \includegraphics[width=0.5\textwidth]{WhatsApp Image 2024-04-28 at 22.42.49.jpeg}
  \label{fig:WhatsApp Image 2024-04-28 at 22.42.49}
\end{figure}

Esta misma posee sus inderteminaciones, o dicho de manera grotesca "Los siete pecados del límite"

$$\begin{tabular}{|c|c|} \hline
     $+\infty$ + $+\infty$ & 0 * $\infty$  \\
     \hline
      $\frac{0}{0}$ & $\frac{\infty }{\infty }$\\
      \hline
      $0^0$ & $1^\infty $, $\infty ^0$ \\
      \hline
\end{tabular}$$\citep{leithold1987calculo}


\section{\LARGE Demostración de fórmulas, teoremas y proposiciones}
\begin{theorem}
UNICIDAD DEL LÍMITE El límite de una función si existe, es único, es decir:$$\begin{tabular}{|c|}
\hline
Si \lim_{x\rightarrow a} f(x)= L y \lim_{x\rightarrow a} f(x)= L*\, \, \, entonces \, \, L=L*\\
     \hline
\end{tabular}$$

\begin{proof}
    Por definición de límite:

$$
f(x) = L \quad \text{si dado } \varepsilon > 0, \exists \delta_1 > 0 \text{ tal que si } 0 < \left| \frac{x - a}{2} \right| < \delta_1 \Rightarrow \left| f(x) - L \right| < \varepsilon \quad (1)
$$

$$
f(x) = L^* \quad \text{si dado } \varepsilon > 0, \exists \delta_2 > 0 \text{ tal que si } 0 < \left| \frac{x - a}{2} \right| < \delta_2 \Rightarrow \left| f(x) - L^* \right| < \varepsilon \quad (2)
$$

Si a la expresión $\frac{1}{2} \left| L - L^* \right|$ se le suma y resta $f(x)$, se obtiene:

$$
\frac{1}{2} \left| L - L^* \right| = \frac{1}{2} \left( f(x) - L^* \right) - \left( f(x) - L \right)
$$

Recordando la propiedad de valor absoluto: $\left| a - b \right| \leq \left| a \right| + \left| b \right|$, se tiene:


$$\frac{1}{2} \left( f(x) - L^* \right) - \left( f(x) - L \right) \leq \frac{1}{2} \left| f(x) - L \right| + \frac{1}{2} \left| f(x) - L^* \right|$$


Por $(1)$ y $(2)$ se obtiene:

$$\frac{1}{2} \left| L - L^* \right| \leq \frac{1}{2} \left| f(x) - L \right| + \frac{1}{2} \left| f(x) - L^* \right| \quad \text{para } 0 < \frac{\left| x - a \right|}{2} < \delta$$

El único número no negativo que es menor a otro positivo por pequeño que sea es el cero.

$$\frac{1}{2} \left| L - L^* \right| = 0 \Rightarrow L = L^*$$

Se ha demostrado que, si existe, el límite de una función es único.
\end{proof}
\end{theorem}

\begin{lemma}
    Límite de una suma de funciones:

Si $\lim_{x \to c} f(x) = L$ y $\lim_{x \to c} g(x) = G$, entonces:

$$
\lim_{x \to c} \left( f(x) + g(x) \right) = L + G
$$

En otras palabras, el límite de la suma de dos funciones que tienen límite es igual a la suma de los respectivos límites de cada función para la misma tendencia.
\begin{proof}
    De acuerdo con la definición de límite, para los límites de la hipótesis se debe cumplir que para todo $\varepsilon > 0$ (arbitrariamente pequeño y positivo) debe existir un $\delta_1$ y un $\delta_2$ (también arbitrariamente pequeños y positivos) que dependan de $\varepsilon$, tal que:

$$
0 < |x - c| < \delta_1 \Rightarrow |f(x) - L| < \frac{\varepsilon}{2}
$$

$$
0 < |x - c| < \delta_2 \Rightarrow |g(x) - G| < \frac{\varepsilon}{2}
$$

En otras palabras, para cualquier $\varepsilon$ positivo, existe un $\delta_1$ y un $\delta_2$ tales que si la distancia entre $x$ y $c$ es menor que $\delta_1$, entonces la diferencia entre $f(x)$ y $L$ es menor que $\frac{\varepsilon}{2}$, y si la distancia entre $x$ y $c$ es menor que $\delta_2$, entonces la diferencia entre $g(x)$ y $G$ es menor que $\frac{\varepsilon}{2}$.
\\
Llamando $\delta$ al más pequeño de los valores del par $(\delta_1, \delta_2)$, se tendrá que:
$$0<|x-c|<\delta \Rightarrow |f(x)+g(x)|-|L+G|=|f(x)-L|+|g(x)-G|$$ $$\leq |f(x)-L|+|g(x)-G|$$ $$\leq \frac{\varepsilon }{2} + \frac{\varepsilon }{2}$$ $$\leq \varepsilon$$ 
El resultado indica que a medida que la variable $x$ toma valores suficientemente cercanos a $c$, se pueden obtener valores de $f(x) + g(x)$ cada vez más cercanos a $(L + G)$.\citep{piskunov1977calculo}
\end{proof}
\end{lemma}
\begin{theorem}
    Si f y g son dos funciones tales que f(x)$\leq$g(x), paa todo x de un intervalo con x$\neq$a, y $\lim_{x\rightarrow a} f(x)=L, \lim_{x\rightarrow a} g(x)=M$ entones L$\leq$M es decir $\lim_{x\rightarrow a} f(x)\leq \lim_{x\rightarrow a} g(x)$,
    \begin{proof}
        Demostraremos por el absurdo. Supongamos que $L>M$ entonces $L-M>0$. Como $\lim_{x\rightarrow a} f(x)=L$ y $\lim_{x\rightarrow a} g(x)=M$, para $\varepsilon = \frac{L-M}{2}$, existen $\delta _1 >0$ y $\delta _2 >0$ tales que: $$\left\{\begin{matrix}
 0<|x-a|\delta _1 \\ 
  0<|x-a|\delta _2
\end{matrix}\right. \Rightarrow \begin{matrix}
 |f(x)-L|<\varepsilon \\ 
 |g(x)-M|<\varepsilon 
\end{matrix}\; entonces \left\{\begin{matrix}
 L-\varepsilon <f(x)<L+\varepsilon  \\ 
 M-\varepsilon <g(x)<M+\varepsilon
\end{matrix}\right. (1) $$ Ahora tomando $\delta =min\left \{ \delta _1,\delta _2 \right \}$ y si $0<|x-a|<\delta $, se tiene: $M-\varepsilon<g(x)<M+\varepsilon=L-\varepsilon<f(x)$ entonces $f(x)\leq g(x)$ lo cual es una contradicción puesto que $g(x)\leq f(x)$ y esto es debido a la suposición $L>M$ por lo tanto debe cumplirse $L\leq M$.
    \end{proof}
\end{theorem}
\subsection{\Large Resumen}
\begin{figure}[h]
  \centering
  \includegraphics[width=0.5\textwidth]{Formulario de Límites Matemáticos.jpg}
  \label{fig:Formulario de Límites Matemáticos}
\end{figure}

\clearpage
\bibliographystyle{plain}
\bibliography{exporef}
\end{document}




@book{Espinoza2012grupo,
    author = "Eduardo Espinoza Ramos",
    title = "Análisis Matemático I",
    publisher = "Edukperu",
    year = {2012}
}

@book{leithold1987calculo,
  title={EL CALCULO 2},
  author={Leithold, Louis},
  year={1987}
}

@article{villalimites,
  title={L{\'\i}mites \& Continuidad},
  author={Villa, Alexander Holgu{\'\i}n and C{\'a}lculo, I}
}

@book{ayres1991calculo,
  title={C{\'a}lculo diferencial e integral},
  author={Ayres, Frank and Mendelson, Elliott and Abellanas, Lorenzo},
  year={1991},
  publisher={McGraw-Hill M{\'e}xico}
}

@book{piskunov1977calculo,
  title={C{\'a}lculo diferencial e integral},
  author={Piskunov, Nikolai and Medkov, K and others},
  volume={1},
  year={1977},
  publisher={Mir}
}
