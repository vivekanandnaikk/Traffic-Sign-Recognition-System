# Project plan

This plan is a set of proposed milestones. Items should be marked complete only when supported by repository evidence.

## 1. Define the project scope

- [ ] Decide whether the project covers traffic-sign classification, sign detection, or both.
- [ ] Identify intended inputs and use cases.
- [ ] Document that the project is experimental and not safety-certified.

## 2. Select data and evaluation

- [ ] Choose a dataset suitable for the selected task and review its terms.
- [ ] Record class labels, data format, and preprocessing requirements.
- [ ] Define train, validation, and test splits without test-set leakage.
- [ ] Select metrics appropriate to the task and document their definitions.

## 3. Implement a baseline

- [ ] Add the actual data-loading and preprocessing implementation.
- [ ] Select and document a baseline model.
- [ ] Record environment and dependency versions.
- [ ] Add tests or checks for important data and model behavior.

## 4. Evaluate and document

- [ ] Run evaluation on the documented held-out split.
- [ ] Inspect errors and describe known limitations.
- [ ] Include reproducible commands and verified examples.
- [ ] Add result visualizations only when produced by the project and properly attributed.

## 5. Consider extensions

Potential extensions—such as inference on video, real-time optimization, or deployment to embedded hardware—should be considered only after the baseline and its evaluation are reproducible.
