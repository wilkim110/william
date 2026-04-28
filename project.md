---
layout: page
title: COMP110 Analysis Project
permalink: /project/
---

# Does Experience Level Affect Perceived Difficulty in COMP110?

## Analysis Summary

This project analyzes survey data collected from COMP110 students to explore whether the course difficulty is experienced differently depending on a student's prior programming experience. The central idea is that the course should better match difficulty to student experience level, since beginners may struggle more than students who already have a coding background.

The dataset contains 534 survey responses across 44 columns, including self-reported prior experience, perceived difficulty (1–7 scale), and perceived understanding (1–7 scale). I selected the columns `prior_exp`, `difficulty`, and `understanding` to perform the analysis.

The analysis began with a scatterplot comparing difficulty and understanding across experience groups, then used box plots to isolate each relationship individually, which proved far more interpretable.

---

## Visualizations

### Chart 1: Difficulty vs. Understanding by Prior Experience (Scatter Plot)

<img src="/static/imgs/chart_scatter.png" alt="Scatter plot of difficulty vs understanding by prior experience" width="700"/>

This scatterplot maps each student's reported difficulty on the x-axis and understanding on the y-axis, with color indicating their prior experience group. At a glance, no obvious clustering by experience is visible, which motivates a closer look using box plots that separate the two relationships.

---

### Chart 2: Prior Experience vs. Perceived Difficulty (Box Plot)

<img src="/static/imgs/chart_box_difficulty.png" alt="Box plot of prior experience vs difficulty" width="700"/>

This box plot reveals a clear inverse relationship between prior programming experience and perceived course difficulty. Students with no experience report a median difficulty of around 4, while those with 2+ years of experience report a median near 2. The boxes also tighten at higher experience levels, showing that experienced students agree more consistently that the course feels manageable.

---

### Chart 3: Prior Experience vs. Perceived Understanding (Box Plot)

<img src="/static/imgs/chart_box_understanding.png" alt="Box plot of prior experience vs understanding" width="700"/>

This box plot shows a similar trend for understanding: students with more experience tend to report higher comprehension of the material. The spread is wider across groups compared to the difficulty chart, suggesting that understanding is influenced by more factors than experience alone.

---

## Conclusions

### Findings

The data largely supports the idea that COMP110's difficulty is not evenly distributed across experience levels. The box plots show a consistent inverse relationship, as prior experience increases, perceived difficulty decreases and perceived understanding increases. This gap is most pronounced between students with no experience and those with 1–2+ years of coding background. The scatterplot alone was inconclusive, but the separated box plots made the trend clear.

### Costs, Downsides, and Trade-offs

Adjusting the course to better serve beginners carries real trade-offs. Slowing the pace or adding more foundational support could reduce the challenge for experienced students, potentially lowering their engagement and the value they get from the course. Creating tiered tracks or differentiated assignments would require significant instructor and TA time, raising costs for the department. Additionally, the data relies on students self-reporting their experience level, which introduces measurement error, someone who dabbled in Scratch for a week might rate themselves the same as someone who took AP CS. Finally, any change that visibly separates students by background risks creating a stigma around being a "beginner."

### Extensions and Future Work

Several refinements could strengthen this analysis:

- **Grade outcomes:** Cross-reference experience level with final course grades to confirm whether the perceived difficulty gap translates to actual performance differences.
- **Topic-level difficulty:** Break difficulty ratings down by unit or assignment type to identify which specific topics cause the most friction for beginners, targeted support would be more effective than a blanket pace change.
- **Longitudinal tracking:** Survey students at multiple points in the semester rather than once, to see whether beginners close the gap over time or fall further behind as the course progresses.
- **Experience type:** Distinguish between formal CS coursework (AP CS, prior college course) and self-taught experience, as these may affect outcomes differently.
- **Instructor interventions:** Test whether specific supports, like optional beginner workshops or experience-matched study groups, reduce the difficulty gap in future semesters.
