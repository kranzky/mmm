# I'm h1

## I'm h2

### I'm h3

#### I'm h4

##### I'm h5

###### I'm h6

```
class MarkdownHelper {


  Map<String, Widget> getTitleWidget(m.Node node) => title.getTitleWidget(node);

  Widget getPWidget(m.Element node) => p.getPWidget(node);

  Widget getPreWidget(m.Node node) => pre.getPreWidget(node);

}
```

*italic text*

**strong text**

`I'm code`

~~del~~

***~~italic strong and del~~***

> Test for blockquote and **strong**

- ul list
- one
  - aa *a* a
  - bbbb
    - CCCC

1. ol list
2. aaaa
3. bbbb
    1. AAAA
    2. BBBB
    3. CCCC

[I'm link](https://github.com/asjqkkkk/flutter-todos)

- [ ] I'm *CheckBox*

- [x] I'm *CheckBox* too

Test for divider(hr):

---

Test for Table:

| header 1 | header 2 |
|---|---|
| row 1 col 1 | row 1 col 2 |
| row 2 col 1 | row 2 col 2 |

Image:

![support](assets/script_medias/1675527935336.png)

Image with link:

[![pub package](assets/script_medias/1675527938945.png)](https://pub.dartlang.org/packages/markdown_widget)

Html Image:

```
<img width="250" height="250" src="assets/script_medias/1675527939855.png"/>
```

Video:

```
<video src="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4">
```

Maths:

- $\pm \, 0.2$
- $\dfrac{0}{1} \neq \infty$
- $0 < x < 1$
- $0 \leq x \leq 1$
- $x \geq 10$
- $\forall \, x \in (1,2)$
- $\exists \, x \notin [0,1]$
- $A \subset B$
- $A \subseteq B$
- $A \cup B$
- $A \cap B$
- $X \implies Y$
- $X \impliedby Y$
- $a \to b$
- $a \longrightarrow b$
- $a \Rightarrow b$
- $a \Longrightarrow b$
- $a \propto b$

$$\forall \; x \in X \quad \exists \; y \leq \epsilon$$

$$P \left( A=2 \, \middle| \, \dfrac{A^2}{B}>4 \right)$$

$$f(X,n) = X_n + X_{n-1}$$

$$\lim_{x \to 0^+} \dfrac{1}{x} = \infty$$

$$
A_{m,n} =
\begin{pmatrix}
a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m,1} & a_{m,2} & \cdots & a_{m,n}
\end{pmatrix}
$$

$\Huge Hello!$
$\huge Hello!$
$\LARGE Hello!$
$\Large Hello!$
$\large Hello!$
$\normalsize Hello!$
$\small Hello!$
$\scriptsize Hello!$
$\tiny Hello!$
Example:
