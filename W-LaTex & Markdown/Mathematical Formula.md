## Mathematical Formula

### Grammar

- in a line ` $mathematical formula$`
- in another line `$$mathematical formula$$`

### Blank in $LaTex$

- $a \qquad b$
- $a \quad b$
- $a \ b$
- $a \; b$
- $a \, b$

### Matrix

$$
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix} \tag{1}
$$

$$
\left\{
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right\} \tag{2}
$$

$$
\left[
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right] \tag{3}
$$

$$
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix} \tag{4}
$$

$$
\begin{Bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{Bmatrix} \tag{5}
$$

$$
\left[
\begin{matrix}
1      & 2      & \cdots & 4      \\
7      & 6      & \cdots & 5      \\
\vdots & \vdots & \ddots & \vdots \\
8      & 9      & \cdots & 0      \\
\end{matrix}
\right] \tag{6}
$$
### Formula aligned

$$
\begin{eqnarray} a & = & b + c \\ 
& = & d + e + f + g + h + ij + k + l \\ 
&& +\: m + n + o \\ 
& = & p + q + r + s \end{eqnarray}
$$



$$
sign(x)=\begin {cases}
+1, & x\geq0 \\\
-1, & x<0
\end {cases}
$$

### Code Block

``` c++
int main(){
  printf(“hello world!\n”);
  return 0;
}
```

### Superscript and Subscript

- `^` to superscript 

- `_` to subscript

  - use`{ }` to represent a union

    $x = a_{1}^n + a_{2}^n + a_{3}^n$

  - use `\sideset` to have scripts both sides 

    e.g.  $\sideset{^1_2}{^3_4}A$

- use `\overline{ }` to $\overline{A}$

- use `\underline{ }` to $\underline{A}$

- use `\hat{ }` to $\hat{y}$, use `\check{ }` to $\check{y}$, and use `\breve{ }` to $\breve{y}$.

- use `\widehat{ }` to $ \widehat{abc} $

- use `\widetilde{ }` to $\widetilde{abc}$

- use `\overbrace{ }^{ }` to  $\overbrace{a + b + c}^{3}$

- $\vec{a}$

### Brackets

- `( )`, `[ ]`, and `|` represent themselves, but `{ }` need be represent by `\lbrace \rbrace` sometime.

- | Bracks | Code      |
  | ------ | --------- |
  | {      | `\lbrace` |
  | }      | `\rbrace` |
  | ⟨      | `\langle` |
  | ⟩      | `\rangle` |
  | ⌈      | `\lceil`  |
  | ⌉      | `\rceil`  |
  | ⌊      | `\lfloor` |
  | ⌋      | `\rfloor` |

### Fraction

- use grammar like `\cfrac or \frac{denominator}{numerator}`

  - e.g. $\cfrac{1}{3}$$ and  $$\frac{1}{3}$

### Square Root

- use `\sqrt[exponent]{radicand}`

  e.g. $ \sqrt[3]{5 - x}$

### Vector

- use `\vec{ }`

  e.g. $\vec{a}$


### Greek Letter

|    Code    | Capital Letter |    Code    | Lower Case |
| :--------: | :------------: | :--------: | :--------: |
|    `A`     |       A        |  `\alpha`  |  $\alpha$  |
|    `B`     |       B        |  `\beta`   |  $\beta$   |
|  `\Gamma`  |    $\Gamma$    |  `\gamma`  |  $\gamma$  |
|  `\Delta`  |    $\Delta$    |  `\delta`  |  $\delta$  |
|    `E`     |       E        | `\epsilon` | $\epsilon$ |
|    `Z`     |       Z        |  `\zeta`   |  $\zeta$   |
|    `H`     |       H        |   `\eta`   |   $\eta$   |
|  `\Theta`  |    $\Theta$    |  `\theta`  |  $\theta$  |
|    `I`     |       I        |  `\iota`   |  $\iota$   |
|    `K`     |       K        |  `\kappa`  |  $\kappa$  |
| `\Lambda`  |   $\Lambda$    | `\lambda`  | $\lambda$  |
|    `M`     |       M        |   `\mu`    |   $\mu$    |
|    `N`     |       N        |   `\nu`    |   $\nu$    |
|   `\Xi`    |     $\Xi$      |   `\xi`    |   $\xi$    |
|    `O`     |       O        | `\omicron` | $\omicron$ |
|   `\Pi`    |     $\Pi$      |   `\pi`    |   $\pi$    |
|  `\Sigma`  |    $\Sigma$    |   `\rho`   |   $\rho$   |
|    `T`     |       T        |  `\sigma`  |  $\sigma$  |
| `\Upsilon` |   $\Upsilon$   | `\upsilon` | $\upsilon$ |
|   `\Phi`   |     $\Phi$     |   `\phi`   |   $\phi$   |
|    `X`     |       X        |   `\chi`   |   $\chi$   |
|   `\Psi`   |     $\Psi$     |   `\psi`   |   $\psi$   |
|  `\Omega`  |    $\Omega$    |  `\omega`  |  $\omega$  |

### Special Alphabet

|  Symbol  |   Code   |
| :------: | :------: |
| $\aleph$ | `\aleph` |



### Relational Operators

|    Symbol    |     Code     |
| :----------: | :----------: |
|    $\pm$     |    `\pm`     |
|   $\times$   |   `\times`   |
|    $\div$    |    `\div`    |
|    $\mid$    |    `\mid`    |
|   $\nmid$    |   `\nmid`    |
|   $\cdot$    |   `\cdot`    |
|   $\circ$    |   `\circ`    |
|    $\ast$    |    `\ast`    |
|  $\bigodot$  |  `\bigodot`  |
| $\bigotimes$ | `\bigotimes` |
| $\bigoplus$  | `\bigoplus`  |
|    $\leq$    |    `\leq`    |
|    $\geq$    |    `\geq`    |
|    $\neq$    |    `\neq`    |
|  $\approx$   |  `\approx`   |
|    $\sum$    |  `\sum{ }`   |
|   $\prod$    |  `\prod{ }`  |
|  $\coprod$   |  `\coprod`   |

### Set Operators

|   Symbol    |    Code     |
| :---------: | :---------: |
| $\emptyset$ | `\emptyset` |
|  $\wp(\ )$  |  `\wp( )`   |
|    $\in$    |    `\in`    |
|  $\notin$   |  `\notin`   |
|  $\subset$  |  `\subset`  |
|  $\supset$  |  `\supset`  |
| $\subseteq$ | `\subseteq` |
| $\supseteq$ | `\supseteq` |
|  $\bigcap$  |  `\bigcap`  |
|  $\bigcup$  |  `\bigcup`  |
|  $\bigvee$  |  `\bigvee`  |
| $\bigwedge$ | `\bigwedge` |
| $\biguplus$ | `\biguplus` |
| $\bigsqcup$ | `\bigsqcup` |

### Logical Operators

|    Symbol     |     Code      |
| :-----------: | :-----------: |
|  $\because$   |  `\because`   |
| $\therefore$  | `\therefore`  |
|   $\forall$   |   `\forall`   |
|   $\exists$   |   `\exists`   |
|    $\not=$    |    `\not=`    |
|    $\not>$    |    `\not>`    |
| $\not\subset$ | `\not\subset` |



### Trigonometric Operators

|  Symbol  |   Code   |
| :------: | :------: |
|  $\bot$  |  `\bot`  |
| $\angle$ | `\angle` |
|  $\sin$  |  `\sin`  |
|  $\cos$  |  `\cos`  |
|  $\tan$  |  `\tan`  |
|  $\cot$  |  `\cot`  |
|  $\sec$  |  `\sec`  |
|  $\csc$  |  `\csc`  |
| $^\circ$ | `^\circ` |

### Calculus Operators

|    Symbol    |           Code           |
| :----------: | :----------------------: |
|   $\prime$   |         `\prime`         |
|    $\int$    |          `\int`          |
|   $\iint$    |         `\iint`          |
|   $\iiint$   |         `\iiint`         |
|   $\oint$    |         `\oint`          |
|    $\lim$    |          `\lim`          |
|   $\infty$   |         `\infty`         |
|   $\nabla$   |         `\nabla`         |
| $\mathrm{d}$ | `\mathrm{d}`or `{\rm d}` |

### Arrow Symbols

|      Symbol       |       Code        |
| :---------------: | :---------------: |
|    $\uparrow$     |    `\uparrow`     |
|   $\downarrow$    |   `\downarrow`    |
|    $\Uparrow$     |    `\Uparrow`     |
|   $\Downarrow$    |   `\Downarrow`    |
|   $\rightarrow$   |   `\rightarrow`   |
|   $\leftarrow$    |   `\leftarrow`    |
|   $\Rightarrow$   |   `\Rightarrow`   |
|   $\Leftarrow$    |   `\Leftarrow`    |
| $\longrightarrow$ | `\longrightarrow` |
| $\longleftarrow$  | `\longleftarrow`  |
| $\Longrightarrow$ | `\Longrightarrow` |
| $\Longleftarrow$  | `\Longleftarrow`  |

