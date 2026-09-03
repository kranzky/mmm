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

![support](cernettes.png)

Image with link:

[![pub package](cernettes.webp)](https://pub.dartlang.org/packages/markdown_widget)

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

Emoji:

- Raw emoji in text: 🚀 🎉 👍 ❤️ ✨ 🐛 🌏
- Shortcodes: :rocket: :tada: :+1: :heart: :sparkles: :bug: :earth_asia:
- Unknown shortcodes stay as written: :not_an_emoji:, and times like 10:30 are safe
- In code they are literal: `:rocket:`
- Outside the bundled set the browser shows a placeholder: 🐙

```
:tada: inside a code block is also literal
```

Code blocks with a language (syntax highlighting):

```python
def fib(n: int) -> int:
    """Return the n-th Fibonacci number."""
    return n if n < 2 else fib(n - 1) + fib(n - 2)  # naive
```

```c
#include <stdio.h>

int main(void) {
    const char* who = "world";  /* classic */
    printf("hello, %s\n", who);
    return 0;
}
```

```javascript
const greet = (name = "world") => `hello, ${name}`;
export default greet;
```

```json
{ "name": "vertext", "free": true, "version": 0.1, "tags": ["markdown", "browser"] }
```

```
A very long line without a language: the quick brown fox jumps over the lazy dog again and again until the line is wider than any pane can show
```

Tables with alignment, inline formatting and wrapping:

| Left | Centre | Right |
|:-----|:------:|------:|
| `code` | **bold** | 1,234.56 |
| [link](index.md) | *emphasis* | 7 |
| A long cell that should wrap onto several lines when the column is narrow | ~~struck~~ | 0 |

| One | Two | Three | Four | Five | Six | Seven | Eight |
|-----|-----|-------|------|------|-----|-------|-------|
| a | b | c | d | e | f | g | h |

Images:

- PNG: ![Cernettes PNG](cernettes.png "The first photo on the web")
- WebP (unsupported until further notice, alt text shows): ![Cernettes WebP](cernettes.webp)
- Missing file (alt text and a broken marker): ![Not here](missing.png)
- Absolute URL: ![Twemoji rocket](https://raw.githubusercontent.com/twitter/twemoji/master/assets/72x72/1f680.png)

Links of every kind:

- Markdown, same site: [Vertext](vertext.md)
- Anchor on this page: [I'm h2](#im-h2), and a broken one: [nowhere](#no-such-heading)
- External HTML: [Wikipedia](https://en.wikipedia.org/wiki/Markdown)
- Autolink: https://mmm.kranzky.com/index.md and <mailto:hello@example.com>
- Wiki link: [[index]] and [[vertext|the browser]]
- Reference style: [the spec][cm]

[cm]: https://spec.commonmark.org/

Quotes containing other blocks:

> A quote with a list:
>
> - one
> - two
>
> and code:
>
> ```
> quoted code
> ```
>
> > and a nested quote with a [link](index.md).

Escapes and edge cases:

- Escaped markers: \*not emphasis\*, \`not code\`, \# not a heading
- Hard break with two spaces  
  continues here; and with a backslash\
  continues here too
- A very long unbroken word: Pneumonoultramicroscopicsilicovolcanoconiosisantidisestablishmentarianismsupercalifragilisticexpialidocious
- A long URL in text: https://example.com/a/very/long/path/that/keeps/going/and/going/with/no/spaces/at/all/index.md
- Non-Latin text: 日本語のテキストは単語の区切りがないので、どこでも折り返せる必要があります。 Ελληνικά, кириллица, العربية (right-to-left is shown left-to-right for now)
- Raw HTML is dropped: <span style="color:red">this span's text stays, the tag goes</span>

<div align="center">
This block-level HTML is dropped entirely.
</div>

Heading with inline formatting and an explicit id:

### A *styled* `heading` with a [link](index.md) {#styled-heading}

Footnotes are not supported and stay literal[^1].

[^1]: This line is shown as ordinary text.
