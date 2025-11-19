# Key Research Questions and Analysis Focus

## 1. How do acceptance rates differ between AI and human pull requests?
*(Corresponding to Fig. 3)*

This analysis examines:

- Differences in acceptance rates across task types (feat / fix / docs).
- Which tasks AI performs better or worse at.
- Whether human reviewers tend to prefer human-authored PRs.

**Findings from the literature:**

- AI PRs have consistently lower acceptance rates than human PRs.
- AI performs best on *documentation-related* tasks.
- Devin generally has higher acceptance rates than GitHub Copilot.
- Claude shows stronger performance on documentation tasks than on code-related tasks.

---

## 2. What patterns exist in the processing speed of AI-submitted PRs?
*(Corresponding to Fig. 4 & Fig. 5)*

Key questions:

- Are AI PRs closed more quickly than human PRs?
- Are AI PRs more prone to “instant rejection” or “instant merge”?
- In what scenarios do AI PRs receive very fast merges?
- Are human PRs processed more slowly but with greater stability?

**Findings from the literature:**

- AI PR turnaround times exhibit a *bimodal distribution*:  
  they are either closed very quickly or merged very quickly.
- Human PRs show smoother, more balanced turnaround time distributions.
- This pattern suggests AI PRs tend to be either extremely simple or of low quality,  
  leading to quick decisions.

---

## 3. How does code complexity change differ between AI and human contributors?
*(Corresponding to Fig. 8)*

The goal is to assess whether AI introduces more or less structural complexity in code changes.

**Findings from the literature:**

- AI-generated code modifications tend to be *simpler*.
- Cyclomatic complexity increases (based on control-flow keywords such as `if`, `for`, etc.)
  are significantly lower in AI PRs.
- Human developers increase complexity more frequently, especially during bugfixes
  or refactoring tasks.

**Interpretation:**  
AI tends to perform template-like, shallow edits rather than modifications involving deep logic or complex structure.

---

## 4. Who reviews AI-generated pull requests — humans, bots, or other AI?
*(Reviewer behavior and ecosystem dynamics)*

Key observations:

- AI PRs are reviewed by **bots** far more frequently than human PRs.
- Some AI agents show evidence of “**AI reviewing AI**” cycles, where automated review bots inspect AI-generated PRs.
- Human developers appear more willing to review PRs submitted by other humans.
