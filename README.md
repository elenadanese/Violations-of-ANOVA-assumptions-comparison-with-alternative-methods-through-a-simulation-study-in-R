## Violations of ANOVA assumptions comparison with alternative methods through a simulation study in R
My Bachelor’s thesis examined the behavior of ANOVA when its assumptions are violated. Using simulated datasets representing non-ideal conditions, I evaluated the method’s performance and alternative approaches, highlighting the importance of selecting appropriate statistical tools and understanding data structure for interpretable results.
After a brief theoretical introduction, I conducted an analysis based on simulated data, creating many different scenarios, often far from the ideal situation where the assumptions hold. This reflects real-world data, which are often “messy” or structured in a non-ideal way. Analyzing how ANOVA performs in these cases and testing alternative methods helped me understand that it is essential not only to choose the statistical tool best suited for the purpose of the analysis, but also to know the structure of the data well, in order to obtain reliable and interpretable results.

# Key Topics Covered
1. ANOVA theory and assumptions
2. Consequences of assumption violations:
   - Normality
   - Independence
   - Homoscedasticity (test of Cochran, Bartlett, Hartley, Levene, Brown-Forsythe, Fligner-Killeen)
3. Methods to handle heteroscedasticity:
   - Data transformation
   - Non-parametric ANOVA (Kruskal-Wallis)
   - Welch test
   - Alexander-Govern test
   - James of second order test
4. Handling dependent data:
   - Repeated measures ANOVA
   - Friedman test
   - Mixed-effects models
5. Simulation study:
   - Balanced/unbalanced, homo/heteroscedastic, independent/dependent scenarios

# Tools
- R Packages:
  - outliers (cochran.test())
  - stats (bartlett.test(), fligner.test(), kruskal.test(), oneway.test(), aov(), friedman.test())
  - lawstat (levene.test())
  - onewaytests (ag.test(), welch.test(), james.test())
  - lme and nlme (mixed-effects models)
  - generation of simulated datasets (e.g., rnorm(), mvrnorm())
  - ggplot2 (data manipulation and visualization)
