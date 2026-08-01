# Label-visible scoring example

This synthetic example is separate from the validation and test phases and contains no challenge ground truth.

- `images/example_page_1.png`: synthetic input page.
- `reference.md`: label-visible reference output.
- `candidates/exact.md`: exact canonical prediction.
- `candidates/compatible-delimiters.md`: mathematically identical prediction using accepted compatibility delimiters.
- `expected_scores.json`: expected scores under `drdocbench-document-parsing-v1`.

Before scoring, the evaluator converts `\( ... \)` to `$ ... $` and `\[ ... \]` to `$$ ... $$`. The two candidate files therefore materialize identically and both receive full component and Overall scores.
