---
layout: page
title: "Home"
---

<!-- {% for post in paginator.posts %}
<div class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
        <h2 class="post-title">            {{ post.title }}
        </h2>
        {% if post.subtitle %}
        <h3 class="post-subtitle">
            {{ post.subtitle }}
        </h3>
        {% endif %}
    </a>
    <p class="post-meta">Posted by {% if post.author %}{{ post.author }}{% else %}{{ site.title }}{% endif %} on {{ post.date | date: "%B %-d, %Y" }}</p>
</div>
<hr>
{% endfor %}

<!-- Pager -->
<!-- {% if paginator.total_pages > 1 %}
<ul class="pager">
    {% if paginator.previous_page %}
    <li class="previous">
        <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
    </li>
    {% endif %}
    {% if paginator.next_page %}
    <li class="next">
        <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
    </li>
    {% endif %}
</ul>
{% endif %} -->

Can we learn to locate objects in images, only from the list of objects those images contain? Or the sentiment of a phrase in a review from the overall score? Can we tell who voted for Obama in 2012? Or which population strata are more likely to be infected by Ebola, only looking at geographical incidence and census data? Are large corporations able to infer sensitive traits of their customers such as sex preferences, unemployment or ethnicity, only based on state-level statistics?

In contrast, how can we publicly release data containing personal information to the research community, while guaranteeing that individuals' sensitive information will not be compromised? How realistic is the idea of outsourcing machine-learning tasks without sharing datasets but only a few statistics sufficient for training?

Despite their diversity, solutions to those problems can be surprisingly alike, as they all play with the same elements: variables without a clear one-to-one mapping, and the search for/the protection against models and statistics sufficient to recover the relevant variables.

Aggregated statistics and obfuscated data are abundant, as they are released much more frequently than plain individual-level information; the latter are often too sensitive because of privacy constraints or business value, or too expensive to collect. Learning in those scenarios has been conceptualized, for example, by multiple instance learning [1,2,3], learning from label proportions [4,5,6,7,8,9], and learning from noisy labels [10,11], and it is common in a variety of application fields, such as computer vision [13,14], sentiment analysis [15] and bioinformatics [1], whenever labels for single image patches, sentences or proteins are unknown, while higher-level supervision is possible.

This problem is not limited to computer science, though. In fact, as natural, social and medical disciplines have studied the problem of inference from aggregates for a long time, including the so-called ecological inference in political science [16,17,18], econometrics [19] and epidemiology [20], and the modifiable areal unit problem in spatial statistics [21].

But as those approaches are shown to be effective in practice, to the point that the available statistics reveal sensitive attributes with high accuracy, the question is turned around into a search for privacy guarantees. Traditional statistics has studied the problem of confidential data release [22]. Research in k-anonymity, l-diversity [23, 24, 25, 26] and, more recently, differential privacy [27, 28, 29, 30] has proposed procedures to mask data in a way that one can trade-off protection and usefulness for statistical analysis.

Read the [CFP]({{site.baseurl}}/CFP/).


### Selected references
<ul class="bib">
<li>  T.G. Dietterich, R.H. Lathrop, T. Lozano-Pérez, Solving the multiple instance problem with axis-parallel rectangles, Artificial Intelligence, 1997.
<li> Z.-H. Zhou, Y.-Y. Sun, Y.-F. Li, Multi-instance learning by treating instances as non-iid samples, ACM, 2009.
<li>
  G. Krummenacher, C. S. Ong, J. Buhmann, Ellipsoidal multiple instance learning, ICML, 2013.
<li>
 H. Kück, N. de Freitas, Learning about individuals from group statistics, UAI, 2005.
<li>
 N. Quadrianto, A.J. Smola, T.S. Caetano, Q.V. Le, Estimating labels from label proportions, JMLR, 2009.
<li>
F.X. Yu, D. Liu, S. Kumar, T. Jebara, S.F. Chang, \propto-SVM for learning with label proportions, ICML, 2013.
<li>
F. Xu, K. Choromanski, S. Kumar, T. Jebara, S.-F. Chang, On learning from label proportions, Technical report on arXiv, 2014.
<li>
G. Patrini, R. Nock, P. Rivera, T.S. Caetano, (Almost) no label no cry, NIPS, 2014
<li>
S. Wager, A. Blocker, N Cardin, Weakly supervised clustering: learning fine-grained signals from coarse side information, Submitted.
<li>
N. Natarajan, I.S. Dhillon, P. Ravikumar, A. Tewari, Learning with noisy labels, NIPS, 2013.
<li>
B. Frénay, M. Verleysen. Classification in the presence of label noise: a survey,  IEEE Transactions on Neural Networks and Learning Systems, 2014.
<li>
A. K. Menon, B. van Rooyen, C. S. Ong, R. C. Williamson, Learning from Corrupted Binary Labels via Class-Probability Estimation, ICML, 2015.
<li>
B. Babenko, M.H. Yang, S. Belongie, Visual tracking with online multiple instance learning. CVPR, 2009.
<li>
Yu X. Felix, Liangliang Cao, Michele Merler, Noel Codella, Tao Chen, John R. Smith, Shih-Fu Chang, Modeling attributes from category-attribute proportions, ACM, 2014.
<li>
D. Kotzias, D. Misha, N. de Freitas, P. Smyth, From group to individual labels using deep features, KDD, 2015.
<li>
L. Anselin, W. K. Tam Cho, Spatial effects and ecological inference, Political analysis, 2002.
<li>
G. King, A solution to the ecological inference problem: Reconstructing individual behaviour from aggregated data, Princeton University Press, 2013.
<li>
S. Flaxman, Y.-X. Wang, A. Smola, Who supported Obama in 2012? Ecological inference through distribution regression, KDD, 2015.
<li>
P.J. Cross, C.F. Manski, Regressions, short and long, Econometrica, 2002.
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
M. Hardt, K. Ligett, F. McSherry, A simple and practical algorithm for differentially private data release, NIPS, 2012.
<li>
R. Nock, G. Patrini, A. Friedman, Rademacher observations, private data, and boosting, ICML, 2015.
<li>
Y.-X. Wang, S. E. Fienberg, A. Smola, Privacy for Free: Posterior sampling and stochastic gradient monte carlo, ICML, 2015.
</ul>