---
layout: page
title: "Home"
---

Can we learn to locate objects in images, only from the list of objects those images contain? Or the sentiment of a phrase in a review from the overall score? Can we tell who voted for Obama in 2012? Or which population strata are more likely to be infected by Ebola, only looking at geographical incidence and census data? Are large corporations able to infer sensitive traits of their customers such as sex preferences, unemployment or ethnicity, only based on state-level statistics?

In contrast, how can we publicly release data containing personal information to the research community, while guaranteeing that individuals' sensitive information will not be compromised? How realistic is the idea of outsourcing machine-learning tasks without sharing datasets but only a few statistics sufficient for training?

Despite their diversity, solutions to those problems can be surprisingly alike, as they all play with the same elements: variables without a clear one-to-one mapping, and the search for/the protection against models and statistics sufficient to recover the relevant variables.

Aggregate statistics and obfuscated data are abundant, as they are released much more frequently than plain individual-level information; the latter are often too sensitive because of privacy constraints or business value, or too expensive to collect. Learning in those scenarios has been conceptualized, for example, by multiple instance learning [1,2,3], learning from label proportions [4,5,6,7,8,9], and learning from noisy labels [10,11], and it is common in a variety of application fields, such as computer vision [13,14], sentiment analysis [15] and bioinformatics [1], whenever labels for single image patches, sentences or proteins are unknown, while higher-level supervision is possible.

The setting is not limited to machine learning though. The problem of inferring individual-level behavior from aggregate-level information is commonly faced in the natural, social and medical disciplines, where statistical solutions to problems commonly referred to as aggregation bias [16] or the ecological fallacy [17] are important tools for quantitative reasoning. Solutions and techniques to making valid inference from aggregated data include
the ecological inference in political science [18,19,20], econometrics [21] and epidemiology [22], and the modifiable areal unit problem in spatial statistics [23].

But as those approaches are shown to be effective in practice, to the point that the available statistics reveal sensitive attributes with high accuracy, the question is turned around into a search for privacy guarantees. Traditional statistics has studied the problem of confidential data release [24]. Research in k-anonymity, l-diversity [25, 26, 27, 28] and, more recently, differential privacy [29, 30, 31, 32, 33] has proposed procedures to mask data in a way that one can trade-off protection and usefulness for statistical analysis.

Read the [CFP]({{site.baseurl}}/CFP/).

### Selected references
<ul class="bib">
<li>
T.G. Dietterich, R.H. Lathrop, T. Lozano-Pérez, Solving the multiple instance problem with axis-parallel rectangles, Artificial Intelligence, 1997.
<li>
Z.-H. Zhou, Y.-Y. Sun, Y.-F. Li, Multi-instance learning by treating instances as non-iid samples, ACM, 2009.
<li>
G. Krummenacher, C. S. Ong, J. Buhmann, Ellipsoidal multiple instance learning, ICML, 2013.
<li>
H. Kück, N. de Freitas, Learning about individuals from group statistics, UAI, 2005.
<li>
N. Quadrianto, A.J. Smola, T.S. Caetano, Q.V. Le, Estimating labels from label proportions, JMLR, 2009.
<li>
F.X. Yu, D. Liu, S. Kumar, T. Jebara, S.F. Chang, \propto-SVM for learning with label proportions, ICML, 2013.
<li>
F.X. Yu, K. Choromanski, S. Kumar, T. Jebara, S.-F. Chang, On learning from label proportions, Technical report on arXiv, 2014.
<li>
G. Patrini, R. Nock, P. Rivera, T.S. Caetano, (Almost) no label no cry, NIPS, 2014.
<li>
S. Wager, A. Blocker, N Cardin, Weakly supervised clustering: learning fine-grained signals from coarse side information, Annals of Applied Statistics, 2015 (to appear).
<li>
N. Natarajan, I.S. Dhillon, P. Ravikumar, A. Tewari, Learning with noisy labels, NIPS, 2013.
<li>
B. Frénay, M. Verleysen. Classification in the presence of label noise: a survey,  IEEE Transactions on Neural Networks and Learning Systems, 2014.
<li>
A. K. Menon, B. van Rooyen, C. S. Ong, R. C. Williamson, Learning from Corrupted Binary Labels via Class-Probability Estimation, ICML, 2015.
<li>
B. Babenko, M.H. Yang, S. Belongie, Visual tracking with online multiple instance learning. CVPR, 2009.
<li>
K.-T. Lai; F.X. Yu; M.-S. Chen; S.-F. Chang. Video event detection by inferring temporal instance labels, CVPR, 2014.
<li>
D. Kotzias, D. Misha, N. de Freitas, P. Smyth, From group to individual labels using deep features, KDD, 2015.
<li>
T. M. Stoker, Empirical Approaches to the Problem of Aggregation Over Individuals, Journal of
Economic Literature, 1993.
<li>
W. S. Robinson, Ecological correlations and the behavior of individuals, American Sociological Review, 1950.
<li>
L. Anselin, W. K. Tam Cho, Spatial effects and ecological inference, Political analysis, 2002.
<li>
G. King, A solution to the ecological inference problem: Reconstructing individual behavior from aggregate data, Princeton University Press, 2013.
<li>
S. Flaxman, Y.-X. Wang, A. Smola, Who supported Obama in 2012? Ecological inference through distribution regression, KDD, 2015.
<li>
W. K. Tam Cho, C.F. Manski, Cross-Level/Ecological Inference, Oxford Handbook of Political Methodology, 2008
<li>
J. Wakefield, G. Shaddick, Health-exposure modelling and the ecological fallacy, Biostatistics, 2006.
<li>
S. Openshaw, The modifiable areal unit problem. Norwick: Geo Books, 1983.
<li>
G.T. Duncan, M. Elliot, J.-J. Salazar-González, Statistical confidentiality: principles and practise, Springer New York, 2011.
<li>
L. Sweeney, k-anonymity: A model for protecting privacy, International Journal of Uncertainty, Fuzziness and Knowledge-Based Systems, 2002.
<li>
A. Machanavajjhalam, D. Kifer, J. Gehrkem, M. Venkitasubramaniam, l-diversity: Privacy beyond k-anonymity, ACM Transactions on Knowledge Discovery from Data, 2007.
<li>
A. Friedman, R. Wolff, A. Schuster, Providing k-anonymity in data mining, The VLDB Journal, 2008.
<li>
K. Choromanski, T. Jebara, K. Tang, Adaptive anonymity via b-matching, NIPS, 2013.
<li>
C. Dwork, F. McSherry, K. Nissim, A. Smith, Calibrating noise to sensitivity in private data analysis, Theory of Cryptography, 2006.
<li>
B. Barak, K. Chaudhuri, C. Dwork, S. Kale, F. Mcsherry, K. Talwar, Privacy, Accuracy, and Consistency Too: A Holistic Solution to Contingency Table Release, PODS, 2007.
<li>
M. Hardt, K. Ligett, F. McSherry, A simple and practical algorithm for differentially private data release, NIPS, 2012.
<li>
R. Nock, G. Patrini, A. Friedman, Rademacher observations, private data, and boosting, ICML, 2015.
<li>
Y.-X. Wang, S. E. Fienberg, A. Smola, Privacy for Free: Posterior sampling and stochastic gradient monte carlo, ICML, 2015.
</ul>
