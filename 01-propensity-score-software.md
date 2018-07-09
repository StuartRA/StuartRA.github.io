---
layout: page
title: Propensity Score Software
group: navigation
permalink: "software.html"
---
{% include JB/setup %}

### Software for implementing matching methods and propensity scores
<br>



#### R

[MatchIt](http://gking.harvard.edu/matchit)
* [Ho, D.E., Imai, K., King, G., and Stuart, E.A. (2011). MatchIt: Nonparametric preprocessing for parameteric causal inference. Journal of Statistical Software 42(8).](http://www.jstatsoft.org/v42/i08)
* Two-step process: does matching, then user does outcome analysis (integrated with [Zelig](gking.harvard.edu/zelig/) package for R)
* Wide array of estimation procedures and matching methods available: nearest neighbor, Mahalanobis, caliper, exact, full, optimal, subclassification
* Built-in numeric and graphical diagnostics

[Matching](http://sekhon.berkeley.edu/matching)
* [Sekhon, J. S. (2011). Multivariate and propensity score matching software with automated balance optimization: The Matching package for R. Journal of Statistical Software 42(7).](http://www.jstatsoft.org/v42/i07)
* Uses automated procedure to select matches, based on univariate and multivariate balance diagnostics
* Primarily 1:M matching (where M is a positive integer), allows matching with or without replacement, caliper, exact
* Includes built-in effect and variance estimation procedures

[twang](http://cran.r-project.org/web/packages/twang/index.html)
* Ridgeway, G., McCaffrey, D., and Morral, A. (2006). twang: Toolkit for weighting and analysis of nonequivalent groups.
* Functions for propensity score estimating and weighting, nonresponse weighting, and diagnosis of the weights
* Primarily uses generalized boosted regression to estimate the propensity scores
* Includes functionality for multiple group weighting, marginal structural models

[cem](http://gking.harvard.edu/cem/)
* [Iacus, S.M., King, G., and Porro, G. (2008). Matching for Causal Inference Without Balance Checking.](gking.harvard.edu/files/abs/cem-abs.shtml)
* Implements coarsened exact matching
* Can also be implemented through [MatchIt](http://gking.harvard.edu/matchit)

[optmatch](http://cran.r-project.org/web/packages/optmatch/index.html)
* Hansen, B.B., and Fredrickson, M. (2009). optmatch: Functions for optimal matching.
* Variable ratio, optimal, and full matching
* Can also be implemented through [MatchIt](http://gking.harvard.edu/matchit)

[PSAgraphics](http://cran.r-project.org/web/packages/PSAgraphics/index.html)
* [Helmreich, J.E. and Pruzek, R.M. (2009). PSAgraphics: An R Package to Support Propensity Score Analysis. Journal of Statistical Software 29(6).](www.jstatsoft.org/v29/i06)
* From webpage: "A collection of functions that primarily produce graphics to aid in a Propensity Score Analysis (PSA). Functions include: cat.psa and box.psa to test balance within strata of categorical and quantitative covariates, circ.psa for a representation of the estimated effect size by stratum, loess.psa that provides a graphic and loess based effect size estimate, and various balance functions that provide measures of the balance achieved via a PSA in a categorical covariate."

[Synth](https://cran.r-project.org/web/packages/Synth/)
* [Abadie, A., Diamond, A., and Hainmueller, H. (2011). Synth: An R Package for Synthetic Control Methods in Comparative Cast Studies. Journal of Statistical Software 42(13).](http://www.jstatsoft.org/v42/i13)
* Implements weighting approach to creating synthetic control groups
* Useful when there is a single treated unit, such as a state or country. Main idea is to form a weighted average of comparison units that, when weighted, looks like the treated unit.

[Cobalt: Covariate balance tables and plots](https://cran.r-project.org/web/packages/cobalt/index.html)
* Generates balance tables and figures for covariates following matching, weighting, or subclassification
* Integrated with MatchIt, twang, matching, CBPS, and ebal

[CBPS](https://cran.r-project.org/web/packages/CBPS/index.html)
* Imai, K., and Ratkovic, M. (2014). Covariate balancing propensity score. Journal of the Royal Statistical Society Series B 76(1): 243-263.
* Estimates propensity score in way that automatically targets balance
* Also includes functionality for marginal structural models, three- and four-valued treatment levels, and continuous treatments <br>
&nbsp;&nbsp;&nbsp;[ebal: Entropy reweighting to create balanced samples](https://cran.r-project.org/web/packages/ebal/index.html)
* Hainmueller, J. (2012). Entropy balancing for causal effects: A multivariate reweighting method to produce balanced samples in observational studies. Political Analysis 20: 25-46.
* Reweights dataset such that covariate distributions in reweighted data satisfy a set of user specified moment conditions.
<br>
<br>
<br>

#### Stata

[teffects suite](http://www.stata.com/manuals13/te.pdf)
* Stata written causal inference commands for matching and weighting
* Includes balance diagnostics, 1:1 matching, weighting, doubly robust approaches

[psmatch2](http://ideas.repec.org/c/boc/bocode/s432001.html)
* Leuven, E. and Sianesi, B. (2003). psmatch2. Stata module to perform full Mahalanobis and propensity score matching, common support graphing, and covariate imbalance testing.
* Allows k:1 matching, kernel weighting, Mahalanobis matching
* Includes built-in diagnostics
* Includes procedures for estimating ATT or ATE

[pscore](http://www.lrz-muenchen.de/~sobecker/pscore.html)
* Becker, S.O. and Ichino, A. (2002). Estimation of average treatment effects based on propensity scores (2002) The Stata Journal 2(4): 358-377.
* k:1 matching, radius (caliper) matching, and stratification (subclassification)
* For estimating the ATT

[match](http://www.economics.harvard.edu/faculty/imbens/software_imbens)
* [Abadie, A., Drukker, D., Herr, J. L., and Imbens, G. W. (2004). Implementing matching estimators for average treatment effects in Stata. The Stata Journal 4(3): 290-311.](https://www.stata-journal.com/article.html?article=st0072)
* Primarily k:1 matching (with replacement)
* Allows estimation of ATT or ATE, including robust variance estimators

[cem](http://gking.harvard.edu/cem/)
* [Iacus, S.M., King, G., and Porro, G. (2008). Matching for Causal Inference Without Balance Checking.](gking.harvard.edu/files/abs/cem-abs.shtml)
* Implements coarsened exact matching
<br>
<br>
<br>

#### SAS

[SAS usage note](http://support.sas.com/kb/30/971.html)

Local and global optimal propensity score matching
* [Coca-Perraillon, M. (2007). Local and global optimal propensity score matching. In SAS Global Forum 2007. Paper 185-2007.](http://www2.sas.com/proceedings/forum2007/185-2007.pdf)
* Variety of matching methods. No built in diagnostics. Assumes propensity score already estimated.

[cem](http://gking.harvard.edu/cem/)
* [Iacus, S.M., King, G., and Porro, G. (2008). Matching for Causal Inference Without Balance Checking.](gking.harvard.edu/files/abs/cem-abs.shtml)
* Implements coarsened exact matching

Greedy matching (1:1 nearest neighbor)
* [Parsons, L. S. (2001). Reducing bias in a propensity score matched-pair sample using greedy matching techniques. In SAS SUGI 26, Paper 214-26.](http://www2.sas.com/proceedings/sugi26/p214-226.pdf)
* [Parsons, L.S. (2005). Using SAS software to perform a case-control match on propensity score in an observational study. In SAS SUGI 30, Paper 225-25.](http://www2.sas.com/proceedings/sugi25/25/po/25p225.pdf)
* [Kosanke, J., and Bergstralh, E. (2004). gmatch: Match 1 or more controls to cases using the GREEDY algorithm.](http://www.mayo.edu/research/departments-divisions/department-health-sciences-research/division-biomedical-statistics-informatics/software/locally-written-sas-macros)

1:1 Mahalanbois matching within propensity score calipers
* [Feng, W.W., Jun, Y., and Xu, R. (2005). A method/macro based on propensity score and Mahalanobis distance to reduce bias in treatment comparison in observational study.](www.lexjansen.com/pharmasug/2006/publichealthresearch/pr05.pdf)

Weighting
* [Leslie, S. and Thiebaud, P. (2006). Using propensity scores to adjust for treatment selection bias.](http://www.lexjansen.com/wuss/2006/Analytics/ANL-Leslie.pdf)

Variable ratio matching, optimal matching algorithm
[Kosanke, J., and Bergstralh, E. (2004). Match cases to controls using variable optimal matching.](http://www.mayo.edu/research/departments-divisions/department-health-sciences-research/division-biomedical-statistics-informatics/software/locally-written-sas-macros)
<br>
<br>
<br>

#### SPSS

[Propensity score matching in SPSS](http://arxiv.org/ftp/arxiv/papers/1201/1201.6385.pdf)
* [Thoemmes, F. (2012). Propensity score matching in SPSS.](http://sourceforge.net/projects/psmspss/files/)
* Nearest neighbor propensity score matching with various options (with/without replacement, calipers, k to 1, etc.)
* Detailed balance statistics and graphs
* Actually calls MatchIt using a point and click interface
<br>
<br>
<br>

#### Software for performing analyses of sensitivity to an unobserved confounder

**R**
* [rbounds: An R package for sensitivity analysis with matched data (L. Keele).](http://www.personal.psu.edu/ljk20/rbounds.html)
* [sensitivity function in twang package (G. Ridgeway et al.).](http://rss.acs.unt.edu/Rdoc/library/twang/html/sensitivity.html)

**Stata**
* [rbounds: Stata module to perform Rosenbaum sensitivity analysis for average treatment effects on the treated (M. Gangl)](http://econpapers.repec.org/software/bocbocode/s438301.htm)
* [sensatt: A simulation-based sensitivity analysis for matching estimators (T. Nannicini)](http://www.tommasonannicini.eu/Portals/0/sensatt_wp_4.pdf)
    - Nannicini T. (2007). A Simulation-Based Sensitivity Analysis for Matching Estimators. Stata Journal, 7(3), 334-350
    - Ichino A., Mealli F., Nannicini T. (2008). From Temporary Help Jobs to Permanent Employment: What Can We Learn from Matching Estimators and their Sensitivity? Journal of Applied Econometrics, 23(3), 305-327.
 
**Excel**
* [Love, T.E. (2008) Spreadsheet-based sensitivity analysis calculations for matched samples. Center for Health Care Research & Policy, Case Western Reserve University.](http://www.chrp.org/propensity/)
