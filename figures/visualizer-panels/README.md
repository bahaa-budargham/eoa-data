## Visualizer Panels

Twelve analytical panels produced by the [interactive tool](https://bahaa-budargham.github.io/eoa-symbolic-sequences/)
on the letter-“a” word (`eoa_a_LCR3.14_symbolic_sequence_2000.txt`).

Each panel is a frozen PNG captured from the tool at native resolution.
Click any thumbnail for the full-size file. Every panel carries a caption in the
live tool stating what is **observed**, what is **estimated from a chosen model**,
and what remains an **open hypothesis**. No claim about the infinite-limit
behaviour of the sequence is made by any panel.

| # | Panel | What it shows | Figure |
|---|-------|---------------|--------|
| 1 | Symbolic Turtle Rendering | Geometric embedding of the sequence under a deterministic symbol→angle map. Self-similarity here is a property of the map, not a proof of fractal structure in the sequence. | [![01](eoa-data/figures/visualizer-panels/a-LCR3.14/01-turtle-rendering.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/01-turtle-rendering.png) |
| 2 | Chaos Game Representation | Density of symbol transitions. Empty regions mark transitions absent from the released word. Structure is not proof of long-range order — see Panel 12 for surrogate comparison. | [![02](eoa-data/figures/visualizer-panels/a-LCR3.14/02-chaos-game.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/02-chaos-game.png) |
| 3 | Recurrence Plot | Diagonal structure indicates repeated subwords; block structure indicates subword recurrence at characteristic scales. Periodicity or its absence is observed, not proved. | [![03](eoa-data/figures/visualizer-panels/a-LCR3.14/03-recurrence.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/03-recurrence.png) |
| 4 | Rewrite Engine | Optional user-supplied morphism σ. Renders the resulting word class. In EOA mode no rewriting rule is applied — only the raw symbol waveform is shown. | [![04](eoa-data/figures/visualizer-panels/a-LCR3.14/04-rewrite-engine.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/04-rewrite-engine.png) |
| 5 | Empirical Eigenvector Projection | Prefix Parikh walk projected onto the empirical contracting plane derived from the stride-k letter matrix. Not the substitution Rauzy fractal. | [![05](eoa-data/figures/visualizer-panels/a-LCR3.14/05-eigenvector-projection.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/05-eigenvector-projection.png) |
| 6 | Subword Transition Graph | Order-n factor graph of the released word. Node degree and spectral radius are estimated; h_top is finite-sample, not a proof of asymptotic entropy. | [![06](eoa-data/figures/visualizer-panels/a-LCR3.14/06-subword-graph.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/06-subword-graph.png) |
| 7 | Desubstitution Test | Whether the released word parses uniquely under a candidate morphism σ. Absence of a parse is not proof of non-morphic structure. | [![07](eoa-data/figures/visualizer-panels/a-LCR3.14/07-desubstitution.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/07-desubstitution.png) |
| 8 | Factor Complexity p(k) vs k | Distinct length-k subwords, log-log, with Sturmian (k+1) and linear (Ck) baselines. Two isolated values are insufficient; the shape across all feasible k is the evidence. | [![08](eoa-data/figures/visualizer-panels/a-LCR3.14/08-factor-complexity.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/08-factor-complexity.png) |
| 9 | Abelian Complexity a(k) vs k | Distinct Parikh vectors of length-k factors. Flatness is compatible with balance; boundedness over the language requires a separate proof. | [![09](eoa-data/figures/visualizer-panels/a-LCR3.14/09-abelian-complexity.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/09-abelian-complexity.png) |
| 10 | Finite-Sample Block-Growth Ladder | Sofic upper bounds log ρ(G_k) from order-k factor graphs vs the empirical block-growth rate (1/n)·log p(n). These are estimates on the released word, not the topological entropy of an associated infinite subshift. | [![10](eoa-data/figures/visualizer-panels/a-LCR3.14/10-block-growth-ladder.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/10-block-growth-ladder.png) |
| 11 | Prefix-Frequency Discrepancy | Maximum observed deviation of prefix symbol counts from the asymptotic frequency vector. Bounded here does not establish balance; balance requires uniform boundedness over all factors of the language. | [![11](eoa-data/figures/visualizer-panels/a-LCR3.14/11-prefix-discrepancy.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/11-prefix-discrepancy.png) |
| 12 | Surrogate Controls | Original CGR (top-left) vs frequency-shuffle, Markov order-1, and periodic controls. Structure present in the original but absent in all surrogates is evidence of long-range order. Structure reproduced by the Markov surrogate is explained by lower-order statistics alone. | [![12](eoa-data/figures/visualizer-panels/a-LCR3.14/12-surrogate-controls.png)](eoa-data/figures/visualizer-panels/a-LCR3.14/12-surrogate-controls.png) |

### Reproducing the panels

All twelve panels regenerate from the released word alone. To reproduce:

1. Open the [live tool](https://bahaa-budargham.github.io/eoa-symbolic-sequences/).
2. Paste `eoa_a_LCR3.14_symbolic_sequence_2000.txt` into the sequence field.
3. Set interpreter to **EOA Phonetic Turn**, angle step **22.5°**, turn strength **1.0×**.
4. The twelve panels render in place. Use **Export Proof** to produce a self-contained
   HTML report with all panels embedded as PNGs and the SHA-256 of the input word.

The hash in [`checksum.txt`](checksum.txt) matches the SHA-256 embedded in the report,
which confirms the analysis was run on the exact word released here.
