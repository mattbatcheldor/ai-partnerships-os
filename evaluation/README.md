# AI evaluation lab

## Research question

Does an evidence-constrained prompt produce more defensible partnership hypotheses than an underspecified persuasive prompt?

## Protocol

1. Give both prompt variants the same single public signal and official source.
2. Change one variable: Prompt B adds evidence, inference, delivery and publication constraints.
3. Record the first usable output without silently correcting unsupported claims.
4. Score both outputs against the same six-criterion rubric.
5. Apply the critical-failure override where a publication red line is crossed.
6. Require Matthew's human review before treating scores as portfolio evidence.

## Weighted evaluation rubric

| Criterion | Weight |
| --- | ---: |
| Groundedness | 25% |
| Fact / inference separation | 20% |
| Commercial specificity | 20% |
| Proposition wedge fit | 15% |
| Guardrail compliance | 15% |
| Clarity | 5% |

## Verdict rules

- **PASS:** score of 85 or more with no critical failure.
- **REVIEW:** score of 70–84 with no critical failure.
- **FAIL:** score below 70, or any critical failure.

<details>
<summary><strong>Critical-failure definition</strong></summary>

A critical failure is a red-line breach that makes an output misleading, unsafe or unsuitable for publication. It includes an unsupported certification claim, invented active buying need, assumed private-data access, false affiliation or an unbounded delivery promise.

</details>

## Results in this test

- Baseline average: **46**
- Evidence-constrained average: **94**
- Difference: **48 points**

The six outputs and provisional scores are available in [evaluation-runs.json](../data/evaluation-runs.json). Scenario prompts are in [evaluation-scenarios.json](../data/evaluation-scenarios.json).

## Limitations

- This is one session with three scenarios, not a general benchmark.
- The constrained prompt is longer and more specific, so the test demonstrates workflow design rather than a pure comparison of model intelligence.
- Initial scoring took place inside the same AI-assisted workflow; human adjudication remains required.
- No commercial outcome, buyer response, pipeline or revenue is measured.
