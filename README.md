# Hi, I'm Adinda 👋

Final-year Mathematics student at **Institut Teknologi Bandung (ITB)**, focused on applied statistics for social & health research. Currently building toward a career as a **Data Analyst / Data Scientist**, with statistics and analyst/management-trainee tracks also on the table.

## About Me

- 🎓 B.Sc. Mathematics, ITB — final-year, thesis in progress
- 🔬 Thesis: risk factors of cleft lip and palate (CLP) using **CATPCA** and **GLM (binomial, logit link)**
- 👩‍🏫 Several years of private tutoring experience; involved in educational community service (**Lentera Kecil**)
- 📊 Background spans regression, correlation, classification, and clustering across multiple applied research projects
- 🌱 Currently turning academic research into a data analytics portfolio

## Skills & Tools

**Languages / Tools:** R, Python, SPSS, Minitab

**Statistical Methods:** Categorical PCA (CATPCA), Generalized Linear Models (GLM), Multiple Correspondence Analysis (MCA), K-Means Clustering, multicollinearity diagnostics (VIF), bootstrap resampling, Tjur's R²

**Visualization:** ggplot2, correlation heatmaps (`polycor::hetcor()`), spatial/geographic mapping

## Featured Projects

### 🩺 [Risk Factors of Cleft Lip and Palate — CATPCA & GLM](#)
# Cleft Lip and Palate: Identifying Factors Associated with Cleft Type Using CATPCA & GLM

Undergraduate thesis project (Mathematics, Institut Teknologi Bandung, 2026) analyzing factors associated with cleft type among cleft lip and palate (CLP) patients in West Java and South Sulawesi, Indonesia, using 2023 secondary survey data.

## Problem Statement

Cleft lip and palate (CLP) is a congenital anomaly caused by incomplete fusion of facial tissue during weeks 5-9 of pregnancy. Among diagnosed cases, cleft presentation varies in severity: some patients have a combined cleft lip and palate ("CBL" — generally the more complex presentation), while others have an isolated cleft of the lip or palate only ("CB/L"). This project identifies which parental behavioral, health, and environmental factors are associated with the combined (more complex) presentation versus the isolated one, across two provinces with different demographic and risk profiles — informing more targeted prenatal risk communication and clinical follow-up.

## Novelty / Contribution

Most existing CLP research has been limited to maternal risk factors analyzed one at a time using bivariate methods (e.g., chi-square tests, simple bivariate comparisons), leaving two gaps this project addresses:

- Multivariate rather than bivariate: instead of testing each factor in isolation, this project combines dimensionality reduction with logistic regression in a single multivariate pipeline — allowing many correlated factors (both maternal and paternal) to be modeled jointly rather than one at a time.
- Categorical PCA for mixed-type data: the survey data mixes categorical and numerical variables, which classical PCA cannot handle correctly. This project uses Categorical Principal Component Analysis (CATPCA), which extends PCA to mixed-type data by optimally scaling categorical variables before extracting components — enabling proper dimensionality reduction ahead of the regression stage.
- Paternal factors included: unlike most prior maternal-only studies, this project explicitly incorporates paternal behavioral and health variables (smoking, caffeine, radiation exposure, exercise), which turned out to be some of the most consistent significant predictors across all models.

## Data & Methodology

- Data source: 2023 secondary survey data on non-syndromic CLP patients
  - West Java: 129 collected -> 71 observations after cleaning (60 CBL, 11 CB/L)
  - South Sulawesi: 74 collected -> 62 observations after cleaning (24 CBL, 38 CB/L)
  - Combined dataset: 133 observations
- Response variable: cleft type (binary) — CBL vs CB/L
- Step 1 — Dimensionality reduction (CATPCA):
  - West Java: CATPCA successfully reduced 28 variables to 19 (4 merged composite variables + 15 raw), merging correlated parental health-history variables into "riwayat kesehatan" and correlated environmental-exposure variables into "lingkungan," separately for father and mother
  - South Sulawesi: CATPCA's two dimensions explained only 24.6% of variance (below the 70% adequacy threshold), so no variables could be reduced via CATPCA; reduction instead relied on substantive judgment (e.g., deriving a "miscarriage history" variable from parity and gravidity)
  - Combined dataset: analyzed directly using 12 shared variables plus a region indicator, without CATPCA
- Step 2 — Resampling: Bootstrap resampling (7 iterations) applied before modeling to strengthen the limited sample size
- Step 3 — Modeling: GLM with binomial distribution and logit link function (logistic regression), estimated via IRLS
- Diagnostics: Wald confidence intervals for odds ratios; model fit assessed via deviance reduction (null vs. residual deviance) and AIC

## Key Findings

West Java (AIC = 288.8; deviance reduced from 442.2 to 248.8)
Significant factors increasing odds of the combined (CBL) type: paternal caffeine intake (OR = 3.07), paternal exercise (OR = 2.73), paternal radiation exposure (OR = 1.91), maternal passive smoking (OR = 1.54), maternal caffeine intake (OR = 8.95, wide CI 2.9-27.6), and first-trimester complications (OR = 3.92).
Significant factors decreasing odds of the combined type (i.e., associated with isolated CB/L): maternal health history (OR = 0.65), paternal active smoking (OR = 0.83), paternal passive smoking (OR = 0.82), maternal exercise (OR = 0.15), and maternal radiation exposure (OR = 0.37).

South Sulawesi (AIC = 87.0; deviance reduced from 82.8 to 55.0)
Only three variables were significant, likely reflecting the smaller sample: paternal passive smoking increased odds of the combined type (OR = 3.99), while paternal radiation exposure (OR = 0.06) and maternal passive smoking (OR = 0.01) decreased it — both with wide confidence intervals given the sample size.

Combined dataset (AIC = 520.4; deviance reduced from 761.2 to 494.4)
Region was itself a significant predictor (OR = 5.96), confirming that West Java and South Sulawesi differ meaningfully in cleft-type composition. Also significant: prenatal care visits, first-trimester complications, paternal active/passive smoking, paternal exercise, paternal radiation exposure, and maternal passive smoking.

Cross-model pattern: paternal passive smoking and paternal radiation exposure appear as significant factors in all three models (West Java, South Sulawesi, and combined), making them the most consistent signals across regions — reinforcing the case for including paternal factors in future CLP research.

## Recommendation

The significant region effect indicates that risk-factor profiles for cleft type differ meaningfully between West Java and South Sulawesi, so prenatal counseling and screening protocols should be regionally tailored rather than applying a single national profile. Paternal smoke exposure (active and passive) and paternal radiation exposure are the most consistent factors across both regions, suggesting that expanding risk education to include paternal behavior — not just maternal — could be a high-leverage, low-cost intervention for prenatal clinics.

## Repository Structure

clp-cleft-type-catpca-glm/
- data/               survey data (or description/link if data is restricted)
- scripts/            R scripts: CATPCA, bootstrap, GLM modeling, diagnostics
- outputs/            correlation heatmaps, CATPCA loading plots, OR tables
- report/             full thesis document (BukuTA)

## Tools

R — CATPCA (PRINCALS algorithm), polycor::hetcor() for mixed-data correlation heatmaps, bootstrap resampling, GLM (binomial, logit link) via IRLS, Wald confidence intervals for odds ratios

## Notes & Limitations

- Sample sizes are small after cleaning (71 and 62 observations per region), producing wide confidence intervals for several odds ratios (e.g., maternal caffeine intake in West Java: CI 2.9-27.6)
- CATPCA was only viable for West Java; South Sulawesi's mixed-data structure did not reduce cleanly into low-dimensional components
- One variable in the combined-data model (prenatal care visits) showed a p-value/CI inconsistency worth flagging in discussion with supervisors
- Findings describe factors associated with cleft type among existing CLP cases, not factors that cause CLP incidence overall — an important scope distinction for anyone citing this work

### 🗺️ [Gender Equality Typology in West Java — Clustering & MCA](#)
Built a four-quadrant typology of gender equality across West Java regencies/cities using K-Means clustering and Multiple Correspondence Analysis on mixed-type indicators, paired with spatial mapping to reveal geographic patterns.
**Key skills:** unsupervised learning, mixed-data analysis, spatial visualization, data storytelling

## Currently

🎯 Finishing my thesis and preparing to enter the workforce as a **Data Analyst / Statistician**

## Let's Connect

📫 [LinkedIn](#) · [Email](#)
