# Capstone Black-Box Optimization Competition

The project is part of the following course at Imperial College:
Professional Certificate in Machine Learning and Artificial Intelligence



# Key Documents

Data Sheet
https://github.com/BriarCloudview/Capstone1/blob/data/DataSheet\_v01.docx

Model Card
https://github.com/BriarCloudview/Capstone1/blob/main/ModelCard\_2026-04-13.docx



# Project Summary

## Project Overview

This project involved a capstone challenge mimicking a **Bayesian optimization competition**. The core objective was to find the maximum values of **eight unknown "black-box" functions**. These functions simulated complex real-world tasks where testing is expensive or limited, such as **radiation detection, robot control, and drug discovery**.

## The Challenge

* Each function was a **maximization task**.
* We started with only **ten known data points** per function.
* The difficulty increased across the set, with dimensionality growing from **2D to 8D**.
* We could not see the internal equations; we could only observe how the functions responded to specific inputs.

## Optimization Process

The project followed an iterative, weekly cycle to build understanding:

1. **Review:** Analyzed the growing data set.
2. **Query:** Chose a single new input point per function each week.
3. **Submit:** Used the project portal to get new output values.
4. **Refine:** Updated strategies based on the new results.

## Methodology \& Strategies

We were free to use any machine learning method to guide our search. Strategies employed included:

* **Bayesian Optimization:** Using Gaussian Process Regression and kernels (like Matern or RBF) to balance exploring new areas with exploiting known "peaks".
* **Exploration Algorithms:** Utilizing Upper Confidence Bound (UCB) and Expected Improvement (EI) to navigate "needle-in-a-haystack" landscapes.
* **Dimensionality Reduction:** Identifying "inert" variables to focus on high-influence parameters in high-dimensional spaces.

## Key Outcomes by Function

|Function|Application|Dimensionality|Result Summary|
|-|-|-|-|
|**1**|Radiation Detection|2D|Located a "Sharp Needle" peak using log-transformation for extreme gradients.|
|**2**|ML Model Score|2D|Found a high-intensity peak pinned against a boundary.|
|**3**|Drug Discovery|3D|Reduced adverse side effects by 53x through synergy mapping.|
|**4**|Warehouse Logistics|4D|Identified a central "high-ground" plateau surrounded by steep "cliffs".|
|**5**|Chemical Yield|4D|Confirmed a perfect maximum at the extreme boundary.|
|**6**|Cake Recipe|5D|Optimized a complex five-ingredient balance to maximize quality.|
|**7**|Hyperparameter Tuning|6D|Navigated a non-stationary landscape to find a stable "performance ridge".|
|**8**|High-Dim Optimization|8D|Successfully breached a performance bottleneck through bisection refinement.|

## Conclusion

Success in this project was defined not just by achieving high scores, but by demonstrating **thoughtful, data-driven decision-making** through iterative reflection and strategy revision.



