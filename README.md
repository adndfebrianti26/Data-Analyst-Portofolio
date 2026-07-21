# Adinda - Data Analyst / Statistician Portfolio

## About

Hi, I'm Adinda! I'm a Mathematics graduate from Institut Teknologi Bandung (ITB), with a strong foundation in applied statistics — regression, correlation, classification, and clustering — built through thesis research and academic projects. I'm aiming for roles as a Data Analyst / Statistician, with interest in management trainee and officer development programs as well.

Alongside my studies, I've spent several years as a private tutor and have been involved in an educational community service organization (Lentera Kecil), which sharpened my ability to explain technical ideas clearly to non-technical audiences.

This repository showcases projects from my academic research, focused on applying statistical methods to real survey data in the health and social policy space.

## Table of Contents

- [About](#about)
- [Portfolio Projects](#portfolio-projects)
  - R
    - [Risk Factors of Cleft Lip and Palate — CATPCA & GLM](#risk-factors-of-cleft-lip-and-palate--catpca--glm)
    - [Gender Equality Typology in West Java — Clustering & MCA](#gender-equality-typology-in-west-java--clustering--mca)
- [Education](#education)
- [Contact](#contact)

## Portfolio Projects

In this section I list my main research/analytics projects, briefly describing the methodology and technology stack used.

### Risk Factors of Cleft Lip and Palate — CATPCA & GLM

**Code:** [`clp-cleft-type-catpca-glm`](#)

**Goal:** To identify which parental behavioral, health, and environmental factors are associated with cleft type (combined lip-and-palate vs. isolated lip- or palate-only) among CLP patients in West Java and South Sulawesi, Indonesia.

**Description:** Undergraduate thesis (completed) using 2023 secondary survey data (133 patients across two provinces). The pipeline combines Categorical Principal Component Analysis (CATPCA) to reduce mixed-type predictor variables, followed by a Generalized Linear Model (binomial distribution, logit link) to model cleft type. Unlike most prior CLP research — which is largely maternal-only and bivariate — this project takes a multivariate approach and explicitly includes paternal factors.

**Skills:** dimensionality reduction for mixed-type data, logistic regression, odds ratio interpretation, bootstrap resampling, multicollinearity diagnostics (VIF), model evaluation (AIC, deviance, Tjur's R²).

**Technology:** R, CATPCA (PRINCALS), `polycor::hetcor()`, `ggplot2`.

**Results:** Paternal passive smoking and paternal radiation exposure were significant predictors of cleft type across all three models (West Java, South Sulawesi, and combined). Region itself was a significant predictor (OR = 5.96) in the combined model, indicating regionally distinct risk profiles.

### Gender Equality Typology in West Java — Clustering & MCA

**Code:** [`gender-equality-clustering-westjava`](#)

**Goal:** To classify regencies/cities in West Java into a typology of gender equality profiles to support geographically targeted policy recommendations.

**Description:** Research project combining K-Means Clustering and Multiple Correspondence Analysis (MCA) on mixed-type gender equality indicators, resulting in a four-quadrant typology (Progresif, Anomali Politik, Marjinal, Kesenjangan Pasif), paired with spatial mapping to visualize geographic patterns.

**Skills:** unsupervised learning, mixed-data analysis, spatial visualization, data storytelling.

**Technology:** R / Python (add whichever you used), MCA, K-Means.

**Results:** *(fill in with your actual cluster distribution / key regional finding)*

## Education

Institut Teknologi Bandung (ITB) — B.Sc. Mathematics

## Contact

- LinkedIn: [Adinda Febrianti](https://www.linkedin.com/in/adinda-febrianti-370a44285)
- Email: adndfebrianti26@gmail.com
