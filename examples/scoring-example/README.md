# Label-visible scoring example

This synthetic example is separate from the validation and test phases and contains no challenge ground truth.

- `images/example_page_1.png`: synthetic input page.
- `reference.md`: label-visible reference output.
- `candidates/exact.md`: exact canonical prediction.
- `candidates/compatible-delimiters.md`: mathematically identical prediction using accepted compatibility delimiters.
- `expected_scores.json`: expected scores under `drdocbench-document-parsing-v1`.

The Markdown parser natively accepts both delimiter families. The evaluator preserves submitted Markdown rather than globally rewriting delimiters, which also preserves math markup inside structured HTML table cells. Both candidates receive full component and Overall scores.
