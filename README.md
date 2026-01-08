# Statistics for ML — FAANG-Level Lab

**Goal:** Master ML-relevant statistics: estimators, confidence intervals, hypothesis tests, p-values, multiple comparisons, and common gotchas.

**Outcome:** Students can compute and interpret confidence intervals and tests, understand failure modes (p-hacking, confounding), and connect stats to ML evaluation.

---

# How to Start

1. **Fork** this repository.  
2. Open `stats_student_lab.ipynb` in **Google Colab**.  
3. Complete all **TODO** sections.  
4. **Restart runtime → Run All** cells.  
5. Push changes and submit a **Pull Request**.  

⚠️ **Do NOT edit notebooks directly on GitHub.**

---

## Lab Rules (FAANG Style)

- ✅ State assumptions (IID, normality, equal variances, independence)
- ✅ Use simulation to sanity-check analytical results
- ✅ Interpret results: effect size + uncertainty, not just p-values

---

# Notebook Rules

- Do **NOT** rename the notebook  
- Do **NOT** delete TODOs  
- Do **NOT** hardcode outputs  
- Notebook must run **top-to-bottom**  

---

# Dataset

- Synthetic A/B samples

## Why?

- Removes confounders so you can focus on inference
- Mirrors interview-style A/B reasoning

---

## Section 1 — Estimators

### Task 1.1: Mean + unbiased variance

**Checkpoint Questions:**

- Why does ddof=1 reduce bias?

---

## Section 2 — Confidence Intervals

### Task 2.1: 95% CI for mean (normal approx)

**FAANG Gotcha:**

- CI is for the mean, not individual outcomes.

---

### Task 2.2: Coverage simulation

**Interview Angle:**

- Why does CI have ~95% coverage by design?

---

## Section 3 — Hypothesis Testing

### Task 3.1: Permutation test (no SciPy)

**FAANG Gotcha:**

- p-value is not P(H0 true).

---

## Section 4 — Multiple Comparisons

### Task 4.1: Bonferroni correction

**Interview Angle:**

- Slicing dashboards can create accidental p-hacking.

---

## Out of Scope

- Deep measure-theoretic statistics
- Advanced Bayesian inference

---

## Stretch

- Bootstrap confidence intervals
- Permutation tests for A/B
- Multiple hypothesis correction (Bonferroni / BH-FDR)

---

## Submission Expectations

Students must submit:

- Clean notebook (runs top-to-bottom)
- Answers to **Checkpoint/Explain** prompts
- Short interpretation notes (effect size + uncertainty)

---

## FAANG Interview Evaluation Rubric

| Skill                         | Evaluated |
|------------------------------|-----------|
| Statistical correctness       | ✅        |
| Assumptions awareness         | ✅        |
| Interpretation clarity        | ✅        |
| Simulation sanity checks      | ✅        |
| Multiple comparisons awareness| ✅        |
