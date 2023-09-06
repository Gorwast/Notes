
Related to [[Obsidian]]

1. **For inline formulas, enclose the formula in `$`…`$`. For displayed formulas, use `$$`…`$$`.**
    
    - These render differently. For example, type the following to show _inline_ mode:  
        `$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$`  

$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$

    - or type the following for display mode:  
        `$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$`  

$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$

2. For **Greek letters**, use `\alpha`, `\beta`, …, `\omega`: α, β, …, ω.
    
    - For uppercase letters, use `\Gamma`, `\Delta`, …, `\Omega`: ΓΓ, ΔΔ, …, ΩΩ.
    - For other Greek capital letters, use Latin `$A,`, `B`, `E$` and so on: A,B,E.
    - Some Greek letters have variant forms: `\epsilon \varepsilon` ϵ, ε, `\phi \varphi` ϕ, φ, and others.
3. For **superscripts and subscripts**, use `^` and `_`. For example, `x_i^2`: x2i2, `\log_2 x`: log2xlog2⁡.
    
4. **Groups**. Superscripts, subscripts, and other operations apply only to the next “group”. A “group” is either a single symbol, or any formula surrounded by curly braces `{`…`}`.
    
    - If you do `10^10`, you will get a surprise: 10101010. But `10^{10}` gives what you probably wanted: $10^{10}$.
    - Use curly braces to delimit a formula to which a superscript or subscript applies: `x^5^6` is an error; `{x^y}^z` is xyz, and `x^{y^z}` is xyz. Observe the differences between `x_i^2` x2i2, `x_{i^2}` xi22 and `{x_i}^2` xi22.
5. **Parentheses** Ordinary symbols `()[]` make parentheses and brackets (2+3)[4+4](2+3)[4+4]. Use `\{` and `\}` for curly braces {}{}.
    
    - These do _not_ scale with the formula in between, so if you write `(\frac{\sqrt x}{y^3})` the parentheses will be too small: (x√y3)(3). Using `\left(`…`\right)` will make the sizes adjust automatically to the formula they enclose: `\left(\frac{\sqrt x}{y^3}\right)` is (x√y3)(3).
        
    - `\left` and`\right` apply to all the following sorts of parentheses: `(` and `)` (x)(), `[` and `]` [x][], `\{` and `\}` {x}{}, `|` |x|||, `\vert` |x|||, `\Vert` ∥x∥‖‖, `\langle` and `\rangle` ⟨x⟩⟨⟩, `\lceil` and `\rceil` ⌈x⌉⌈⌉, and `\lfloor` and `\rfloor` ⌊x⌋⌊⌋. `\middle` can be used to add additional dividers. There are also invisible parentheses, denoted by `.`: use `\left.x^2\right\rvert_3^5 = 5^2-3^2` to get
        
        $$x2∣∣53=52−322|35=52−32$$
        
6. **Sums and integrals** `\sum` and `\int`; the subscript is the lower limit and the superscript is the upper limit, so for example `\sum_1^n` ∑n1∑1. Don't forget `{`…`}` if the limits are more than a single symbol. For example, `\sum_{i=0}^\infty i^2` is ∑∞i=0i2∑=0∞2.
    
    - Similarly, `\prod` ∏∏, `\int` ∫∫, `\bigcup` ⋃⋃, `\bigcap` ⋂⋂, `\iint` ∬∬, `\iiint` ∭∭, `\idotsint` ∫⋯∫∫⋯∫.
7. **Fractions** There are [three ways to make fractions](https://math.meta.stackexchange.com/questions/12978/should-dfrac-be-edited-in). `\frac ab` applies to the next two groups, and produces ab; for more complicated numerators and denominators use `{`…`}`: `\frac{a+1}{b+1}` is a+1b+1+1+1.
    
    - If the numerator and denominator are complicated, you may prefer `\over`, which splits up the group that it is in: `{a+1\over b+1}` is a+1b+1+1+1.
    - For continued fractions, [use `\cfrac` instead of `\frac`](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference/5058#5058).

8. **Fonts**
- Use `\mathbb` or `\Bbb` for "blackboard bold": $\mathbb{CHNQRZ\ chnqrzℎ}$.
- Use `\mathbf` for boldface: $\mathbf{CHNQRZ\ chnqrzℎ}$.
    - For expression based characters, use `\boldsymbol` instead: $\boldsymbol{CHNQRZ\ chnqrz\ α}$
- Use `\mathit` for italics: $\mathit{CHNQRZ\ chnqrzℎ}$.
- Use `\pmb` for boldfaced italics: $\pmb{CHNQRZ\ chnqrzℎ}$.
- Use `\mathtt` for "typewriter" font: $\mathtt{CHNQRZ\ chnqrzℎ}$.
- Use `\mathrm` for roman font: $\mathrm{CHNQRZ\ chnqrzℎ}$.
- Use `\mathsf` for sans-serif font: $\mathsf{CHNQRZ\ chnqrzℎ}$.
- Use `\mathcal` for "calligraphic" letters: $\mathcal{CHNQRZ}$ (Uppercase only.)
- Use `\mathscr` for script letters: $\mathscr{CHNQRZ\ chnqrzℎ}$
- Use `\mathfrak` for "Fraktur" (old German style) letters: $\mathfrak{CHNQRZ\ chnqrzℎ}$.

9. **Radical signs / roots** Use `sqrt`, which adjusts to the size of its argument: `\sqrt{x^3}` $\sqrt{x^3}$ ; `\sqrt[3]{\frac xy}` $\sqrt[3]{\frac xy}$. For complicated expressions, consider using `{...}^{1/2}` instead.

10. Some **special functions** such as "lim", "sin", "max", "ln", and so on are normally set in roman font instead of italic font. Use `\lim`, `\sin`, etc. to make these: `\sin x` sinxsin⁡, not `sin x` sinx. Use subscripts to attach a notation to `\lim`: `\lim_{x\to 0}`
    
    $\lim_{x\to 0}$
    
    Nonstandard function names can be set with `\operatorname{foo}(x)` foo(x)foo⁡().
    
11. There are a very large number of **special symbols and notations**, too many to list here; see the short listing [LATEX and AMS-LATEX Symbols](https://pic.plover.com/MISC/symbols.pdf) prepared by Dr. Emre Sermutlu, or the exhaustive listing [The Comprehensive LATEX Symbol List](https://www.ctan.org/tex-archive/info/symbols/comprehensive/symbols-a4.pdf) by Scott Pakin. Some of the most common include:
    

- `\lt \gt \le \ge \neq` <<, >>, ≤≤, ≥≥,≠≠. You can use `\not` to put a slash through almost anything: `\not\lt` ≮≮ but it often looks bad.
    
- `\times \div \pm \mp` ××, ÷÷, ±±, ∓∓. `\cdot` is a centered dot: x⋅y⋅
    
- `\cup \cap \setminus \subset \subseteq \subsetneq \supset \in \notin \emptyset \varnothing` ∪∪, ∩∩, ∖∖, ⊂⊂, ⊆⊆, ⊊⊊, ⊃⊃, ∈∈, ∉∉, ∅∅, ∅∅
    
- `{n+1 \choose 2k}` or `\binom{n+1}{2k}` (n+12k)(+12)
    
- `\to \gets \rightarrow \leftarrow \Rightarrow \Leftarrow \mapsto \implies \iff` →→, ←←, →→, ←←, ⇒⇒, ⇐⇐, ↦↦, ⟹⟹, ⟺⟺
    
- `\land \lor \lnot \forall \exists \top \bot \vdash \vDash` $\land \lor \lnot \forall \exists \top \bot \vdash \vDash$

- `\star \ast \oplus \circ \bullet` $\star \ast \oplus \circ \bullet$
  
- `\approx \sim \simeq \cong \equiv \prec \lhd` ≈≈, ∼∼, ≃≃, ≅≅, ≡≡, ≺≺, ⊲⊲

- `\infty \aleph_0` ∞ℵ0∞ℵ0 `\nabla \partial` ∇∇, ∂∂ `\Im \Re` Iℑ, Rℜ

- For modular equivalence, use `\pmod` like this: `a\equiv b\pmod n` a≡b(modn)≡(mod). For the binary mod operator, use `\bmod` like this: `a\bmod 17` amod17mod17.

- Use `\dots` for the triple dots in a1,a2,…,an1,2,…, and a1+a2+⋯+an1+2+⋯+

- Script lowercase l is `\ell` ℓℓ.

    [Detexify](https://detexify.kirelabs.org/classify.html) lets you draw a symbol on a web page and then lists the TEX symbols that seem to resemble it. These are not guaranteed to work in MathJax, but it's a good place to start. To check that a command is supported, note that MathJax.org maintains a [list of currently supported LATEX commands](https://docs.mathjax.org/en/latest/input/tex/macros/index.html), and one can also check Dr. Carol JVF Burns's page of [TEX Commands Available in MathJax](https://www.onemathematicalcat.org/MathJaxDocumentation/TeXSyntax.htm).

12. **Spaces** MathJax usually decides for itself how to space formulas, using a complex set of rules. Putting extra literal spaces into formulas will not change the amount of space MathJax puts in: `a␣b` and `a␣␣␣␣b` are both ab. To add more space, use `\,` for a thin space ab; `\;` for a wider space ab. `\quad` and `\qquad` are large spaces: ab, ab.

    To set plain text, use `\text{…}`: {x∈s∣x is extra large}{∈∣ is extra large}. You can nest `$…$` inside of `\text{…}`, for example to access spaces.

13. **Accents and diacritical marks** Use `\hat` for a single symbol $\hat{x}$, `\widehat` for a larger formula $\widehat{xy}$. If you make it too wide, it will look silly. Similarly, there are `\bar` $\bar{x}$ and `\overline` $\overline{xyz}$, and `\vec` $\vec{x}$ → and `\overrightarrow` $\overrightarrow{xy}$ and `\overleftrightarrow` $\overleftrightarrow{xy}$. For dots, as in $\frac{d}{dx}x\dot{x}=\dot{x}^2+x\ddot{x}$, use `\dot` and `\ddot`.

14. Special characters used for MathJax interpreting can be escaped using the `\` character: \$ $, `\{` {{, `\}` }}, `\_` __, `\#` ##, `\&` &&. If you want `\` itself, you should use `\backslash` (symbol) or `\setminus` ([binary operation](https://tex.stackexchange.com/questions/511328/difference-between-commands-setminus-and-backslash/511332#511332)) for ∖∖, because `\\` is for a new line.

