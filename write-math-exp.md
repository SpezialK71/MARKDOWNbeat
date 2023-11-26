#### Writing inline expressions
There are two options for delimiting a math expression inline with your text.
You can<br> either surround the expression with dollar symbols `$`, or start the
expression with<br> <code>$\` and end it with \`$</code>. The latter syntax is useful
when the expression you are<br> writing contains characters that overlap with
markdown syntax.  

This sentence uses `$` delimiters to show math inline:  $\sqrt{3x-1}+(1+x)^2$

This sentence uses <code>$\` and \`$</code> delimiters to show math inline:  $`\sqrt{3x-1}+(1+x)^2`$  <br> (which seems to be a non-working method; as it diplays the tick marks too ---KRR)

#### Writing expressions as blocks
To add a math expression as a block, start a new line and delimit the expression with<br> two dollar symbols `$$`.

**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$  

Alternatively, you can use the <code>```math code</code> block syntax to display a math expression<br> as a block. With this syntax, you don't need to use <code>$$</code> delimiters. The following will ren-<br>der the same as above: (but it does not ---KRR)<br><br>
**The Cauchy-Schwarz Inequality**

```math
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
```  

#### Writing dollar signs in line with and within mathematical expressions
To display a dollar sign as a character in the same line as a mathematical expression, you need to escape the non-delimiter `$` to ensure the line renders correctly.<br>

* Within a math expression, add a `\` symbol before the explicit `$`.

    This expression uses `\$` to display a dollar sign: $\sqrt{\$4}$

* Outside a math expression, but on the same line, use span tags around the explicit `$`.

    To split <span>$</span>100 in half, we calculate $100/2$


