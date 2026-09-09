# EOA Data: Pre-Convergence Sequences and Supplementary Materials

This repository contains the datasets, figures, and supplementary materials for the EOA Program.

---

## Contents

| File/Directory | Description |
| :--- | :--- |
| `data/encodings/` | Letter-name input strings for five encodings (English primary, English alternative, Arabic, Hebrew, Greek). |
| `figures/` | Figures from EOA papers and tool outputs. |
| `notebooks/` | Colab notebooks for benchmarks and experiments. |
| `LEADERBOARD.md` | Tracks submissions for open theoretical questions. |
| `EOA_logo.png` | EOA program logo. |

---

## Figures

| Figure | Description |
| :--- | :--- |
| `figure1_pca_cumulative_variance.png` | PCA cumulative variance of substitution matrices. |
| `lcr_across_encodings.png` | LCR values across different encodings (English, Arabic, Hebrew, Greek). |
| `tool-eoa-anagram-comparator-figure1.png` | **EOA Anagram Word Signature Comparator Tool:** Evaluates position vs. position-index letter-weighting methods to separate anagram vectors while demonstrating a ~98.8% memory reduction compared to GPT-2 embedding tables. |
| `tool-eoa-sequence-to-json-builder-figure1.png` | **EOA Sequence to JSON Builder Tool:** Converts unformatted, space- or tab-separated numerical sequences into structured, valid JSON mapping files for downstream EOA applications. |
| `tool-eoa-term-sequence-ratio-figure1.png` | **EOA Term Sequence Ratio Tool:** Performs 50-digit precision division between user-selected sequence terms to compute ratios up to 17 decimal places for investigating sequence convergence and collinearity. |
| `tool-index-eoa-vector-generator-figure1.png` | **EOA Vector Generator Tool:** Processes bulk word lists—or preset corpora like wordfreq and NLTK—to output position-and-index weighted 43-term EOA vectors as a downloadable CSV. |

All figures are stored in the `figures/` directory.
---

## Notebooks

The `notebooks/` folder contains interactive Colab notebooks to reproduce the analyses and benchmark tools.

---

## Citation

If you use any data from this repository, please cite the relevant EOA paper:

- **EOA Program, Part 0:** [Link](https://github.com/bahaa-budargham/eoa-part0-paper)
- **EOA-43 (Part I):** [Link](https://github.com/bahaa-budargham/eoa-part1-paper)

---

## License

All rights reserved. Access to files is granted for review or reference upon request. Reproduction, redistribution, or commercial use is prohibited without express permission.

---

## Related Repositories

- [EOA Program Main Page](https://github.com/bahaa-budargham/engineering-of-alphabets)
- [EOA Part 0 Paper](https://github.com/bahaa-budargham/eoa-part0-paper)
- [EOA Part I Paper](https://github.com/bahaa-budargham/eoa-part1-paper)
