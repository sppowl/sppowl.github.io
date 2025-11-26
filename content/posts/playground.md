+++
title = "Playground"
author = "owl"
date = 2025-03-16T00:00:00+08:00
draft = false
+++

<div class="ox-hugo-toc toc">

<div class="heading">Table of Contents</div>

- [Another Heading](#another-heading)
- [Gen a 3x3 latex matrix, filled with random formulas, not too small](#gen-a-3x3-latex-matrix-filled-with-random-formulas-not-too-small)
- [Headiing2](#headiing2)
- [Gen 5x6 random org table below](#gen-5x6-random-org-table-below)
- [Gen 5x6 random org table below](#gen-5x6-random-org-table-below)
- [Gnuplot Example](#gnuplot-example)
- [Gen random inline latex formulas below](#gen-random-inline-latex-formulas-below)
- [Generate a 5x8 latex matrix non-inlined below, filled with random numbers and letters](#generate-a-5x8-latex-matrix-non-inlined-below-filled-with-random-numbers-and-letters)
- [Org Table Plot](#org-table-plot)
- [Index](#index)

</div>
<!--endtoc-->


## Another Heading {#another-heading}

```text
block belongs to head
```

item2
: level1
    -   nested
        <a id="code-snippet--qqq"></a>
        ```python
        def test():
            print("test")
        print("???")
        test()
        ```

        ```python
        print("another print")
        ```


head4
: 4
    ```text
    block inline of list item
    ```


head5
: 5

it
: ?

item3
: 3

item6
: this is six-th item
    ```python
    print("...")
    ```

    ```text
    ...
    ```


## Gen a 3x3 latex matrix, filled with random formulas, not too small {#gen-a-3x3-latex-matrix-filled-with-random-formulas-not-too-small}

Here is a 3x3 LaTeX matrix filled with random formulas:

\begin{bmatrix}
x^2 + y^2 & \sin(\theta) & e^{\pi i} + 1 \\\\
\log(a + b) & \frac{c}{d} & \sqrt{n^2 + m^2} \\\\
\tan(x) & \int\_0^1 x \\, dx & \sum\_{i=1}^{n} i^2
\end{bmatrix}


## Headiing2 {#headiing2}

special symbols: &pi; &alpha;

This is a inline src block `hello inline shell block`.
This is a inline python[^fn:1] inline block `Inline python print output`
below is a shell src block.

<a id="code-snippet--fun1"></a>
```shell
echo `basename $fname`
```

```text
playground.org
```

And I can refer 'to its output like this: `arg` and something else'


## Gen 5x6 random org table below {#gen-5x6-random-org-table-below}

Here’s a 5x6 table filled with random numbers:

<a id="table--random-table1"></a>
<div class="table-caption">
  <span class="table-number"><a href="#table--random-table1">Table 1</a>:</span>
  Random Table1
</div>

| 1  | 2  | 3  | 4xx | 5  | 6     |
|----|----|----|-----|----|-------|
| 12 | 45 | 23 | 67  | 34 | 89    |
| 68 | 29 | 51 | 74  | 16 | 83    |
| 91 | 22 | 37 | 54  | 18 | 76    |
| 10 | 60 | 33 | 48  | 25 | 92    |
| 15 | 78 | 41 | 57  | 84 | 39    |
|    |    |    |     |    | 10123 |

<a id="figure--fig:reformat-pic"></a>

{{< figure src="/ox-hugo/_20250316_104150screenshot.png" caption="<span class=\"figure-number\">Figure 1: </span>reformat-org-pic1" >}}

<span class="timestamp-wrapper"><span class="timestamp">&lt;2026-04-01 Wed&gt;</span></span>

---

<a id="code-snippet--p1"></a>
```rust { linenos=true, anchorlinenos=true, lineanchors=org-coderef--5c08f3 }
println!("{:?}", 1..10)      (print1)
```

```text
1..10
```

```rust
let x = r#"
def test():
    print("test")
print("???")
test()
"#;
println!("{}", x)
```

In the line [print1](#org-coderef--5c08f3-1) we printed a 1.

Inline shell code: `echo`
Another Inline shell code invode another block: `x.org`


## Gen 5x6 random org table below {#gen-5x6-random-org-table-below}

Here's a 5x6 random Org table:

<a id="code-snippet--org-block-table"></a>
```org
| Col1 | Col2 | Col3 | Col4 | Col5 | Col6 |
|------|------|------|------|------|------|
| 42   | 17   | 35   | 88   | 65   | 22   |
| 10   | 58   | 49   | 71   | 34   | 70   |
| 56   | 92   | 14   | 41   | 27   | 83   |
| 69   | 31   | 94   | 88   | 21   | 65   |
| 84   | 50   | 19   | 95   | 37   | 45   |
```
<div class="src-block-caption">
  <span class="src-block-number"><a href="#code-snippet--org-block-table">Code Snippet 1</a>:</span>
  numbers2
</div>

You can generate a new random table by running code in Emacs or manually changing the numbers.
Run the above code in an Org buffer to generate a 5x3 random table. Adjust the `generate-random-org-table` function parameters as desired for different sizes.


## Gnuplot Example {#gnuplot-example}

<a id="table--data-table"></a>
<div class="table-caption">
  <span class="table-number"><a href="#table--data-table">Table 2</a>:</span>
  numbers1
</div>

| x | y1 | y2 | xx                                                                                           |
|---|----|----|----------------------------------------------------------------------------------------------|
| 0 | 3  | 6  | <span class="timestamp-wrapper"><span class="timestamp">[2025-03-16 Sun]</span></span>       |
| 1 | 4  | 7  | <span class="timestamp-wrapper"><span class="timestamp">&lt;2025-03-16 Sun&gt;</span></span> |
| 2 | 5  | 8  |                                                                                              |

```gnuplot
reset

set title "Putting it All Together"

set xlabel "X"
set xrange [-8:8]
set xtics -8,2,8


set ylabel "Y"
set yrange [-20:70]
set ytics -20,10,70

f(x) = x**2
g(x) = x**3
h(x) = 10*sqrt(abs(x))

plot f(x) w lp lw 1, g(x) w p lw 2, h(x) w l lw 3
```
<div class="src-block-caption">
  <span class="src-block-number">Code Snippet 2:</span>
  plot-src
</div>

{{< figure src="/ox-hugo/example-gnuplot.png" >}}


## Gen random inline latex formulas below {#gen-random-inline-latex-formulas-below}

Here are some random inline LaTeX formulas:

1.  \\( E = mc^2 \\)
2.  \\( a^2 + b^2 = c^2 \\)
3.  \\( \int\_0^{\infty} e^{-x} \\, dx = 1 \\)
4.  \\( \sum\_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6} \\)
5.  \\( \frac{d}{dx}(x^n) = nx^{n-1} \\)


## Generate a 5x8 latex matrix non-inlined below, filled with random numbers and letters {#generate-a-5x8-latex-matrix-non-inlined-below-filled-with-random-numbers-and-letters}

Here is a 5x8 LaTeX matrix filled with random numbers and letters:

\begin{pmatrix}
A & 3 & F & 7 & B & 9 & K & 4 \\\\
2 & D & 1 & X & 8 & E & 5 & M \\\\
Z & 6 & Y & C & 0 & 2 & J & 3 \\\\
H & 4 & T & 8 & Q & 1 & L & 7 \\\\
N & 9 & W & 5 & P & 6 & R & 0 \\\\
\end{pmatrix}

You can copy and paste this code into your LaTeX document to render the matrix.


## Org Table Plot {#org-table-plot}

| Sede      | Max cites | H-index |
|-----------|-----------|---------|
| Chile     | 257.72    | 21.39   |
| Leeds     | 165.77    | 19.68   |
| Sao Paolo | 71.00     | 11.50   |
| Stockholm | 134.19    | 14.33   |
| Morelia   | 257.56    | 17.67   |


## Index {#index}

[^fn:1]: A sad language.
