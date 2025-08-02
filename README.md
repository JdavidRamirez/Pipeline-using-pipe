# Pipeline-using-pipe

##  Introduction

This project demonstrates how to build a clean, modular, and readable data transformation pipeline in Python using the `toolz.pipe()` function. Inspired by a blog post discussing the benefits of function pipelines, I wanted to explore how `pipe()` can help structure data cleaning code in a more elegant and functional way.

The pipeline is designed to clean and enrich a dataset containing chemical compound measurements.

---

##  Dataset

The dataset includes the concentration of various ions (e.g., Ca²⁺, Mg²⁺, Na⁺) in water samples collected over several years.

**Columns:** `n`, `Año`, `Ca2+`, `Mg2+`, `Na+`, `K+`, `HCO3–`, `SO42–`, `Cl–`, etc.

---

##  Pipeline Steps

The pipeline follows these main steps:

1. **Remove unnecessary column** `n`.
2. **Convert object-type columns** to `float`, taking care of commas as decimal separators.
3. **Create new label columns** (e.g., `Ca2+_concentration`) to classify values as `"high"` or `"moderate"` based on the column mean.

All of this is handled using the `toolz.pipe()` function to promote:
-  **Readability** (linear, easy-to-follow transformations)
-  **Modularity** (each transformation is clearly separated)
-  **Clean code structure** (no intermediate variables)

---

## Conclusion:

This project shows how pipe() helps organize data steps in a clear way. The code stays simple and easy to follow. While this example is basic, the structure works well for larger tasks. Using pipe() can make your data work more readable and easier to manage.







