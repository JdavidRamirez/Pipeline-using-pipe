# Pipeline-using-pipe

##  Introduction

This project shows how to build a simple and readable data transformation pipeline in Python using the toolz.pipe() function. I read a blog post that explained the benefits of function pipelines and wanted to try it out. The goal is to see how pipe() helps organize each step in the cleaning process.

The code includes three basic tasks:

* Drop an unnecessary column.

* Convert strings to numbers.

* Label numeric values as "high" or "moderate" based on the column mean.
---

##  Dataset

The dataset includes the concentration of various ions (e.g., Ca²⁺, Mg²⁺, Na⁺) in water samples collected over several years.

**Columns:** `n`, `Año`, `Ca2+`, `Mg2+`, `Na+`, `K+`, `HCO3–`, `SO42–`, `Cl–`, etc.

---

##  Pipeline Steps

1. Drop a column
Remove the column named "n" as it's not useful for the analysis.

2. Convert data types
Convert all columns with object (string) type to float, replacing commas with dots to handle decimal formatting.

3. Label values
Create new columns that label each value as "high" if it’s above the column mean or "moderate" otherwise.


---

## Conclusion:

This project highlights how pipe() can help structure data processing tasks. The steps are easier to follow, and the code remains clean. Even though the example is simple, this method scales well for larger projects and encourages better code organization.






