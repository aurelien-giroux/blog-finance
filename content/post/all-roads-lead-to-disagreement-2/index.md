---
title: "All Roads Lead to Disagreement (II): Pricing Disagreement Without Pricing Truth"
description: "How competing forecasts can become a contract—and change what lenders are willing to finance before everyone agrees."
slug: "all-roads-lead-to-disagreement-2"
author: "Aurélien Giroux"
draft: false
date: 2026-09-26
math: true
readingTimeMinutes: 40
categories:
  - Finance
  - Epistemology
---

Two lenders disagree about a group of utilities. One expects an industrial transition that some of the borrowers will struggle to finance. The other expects them to adapt without much damage to their creditors. Both have models, evidence and arguments, and neither finds the other convincing.

“Put your money where your mouth is” sounds like a way to settle it. It leaves rather a lot for the lawyer to write.

They would first have to agree on what counts as an outcome, when it will be observed, and how their forecasts turn into a payment. None of that is obvious. A high default rate might favour one forecast without showing why the defaults happened. A low one might favour the other while hiding an emergency rescue that kept a few borrowers alive. And the fact that each of them is keen to bet tells us nothing about the price at which anyone else would take the other side.

[Part I](https://aurelien-giroux.github.io/blog-finance/p/all-roads-lead-to-disagreement-1/) of this essay asked why serious disagreement survives careful inquiry. A companion piece, [*What Can a Market See?*](https://aurelien-giroux.github.io/blog-finance/p/what-can-a-market-see/), asked which parts of a disagreement existing markets let an investor act on. This one builds something: a contract that attaches money to a comparison between two forecasts, gives each lender an exposure it can use, and lets anyone inspect the comparison. Choosing the payment, arranging the trade and deciding what its record can prove turn out to be parts of the same design problem.

Several sections have optional mathematical explanations. Open a box for the assumptions and derivations behind the examples; the main argument can be read with all the boxes closed.

## First agree on the test

Suppose the lenders pick a list of one hundred utilities and a five-year window. They will compare forecasts of how many default: fewer than five, five to nine, or ten or more. Three bands keep the arithmetic readable; a real contract could use finer ones. Before the window opens, each lender writes down a probability for each band.

That already takes a good deal of agreement. The lenders can hold completely different views about technology and policy, and keep their models to themselves. But they have to recognise the same borrowers, the same horizon and the same three possible answers, and each has to commit to three numbers in a form that cannot be edited once the defaults start arriving.

Before settling on default counts, though, they should ask what the contract is for. A lender worried about a few very large borrowers cares more about the amount lost than about the number of defaults. A lender concentrated in one region may learn little about its own losses from a national count. A statistic can be measured perfectly and still provide poor protection if the payment it triggers does not correspond to those losses. What a lender is exposed to is the reason to look for an observation; the fact that an observation is easy to obtain does not make it the right one.

Then come the questions that sound tedious. Does a distressed restructuring count as a default? What happens if a utility merges, leaves the sector or stops reporting? Who keeps the record, and which version of it is final? Once money depends on the answer, a disagreement about the future can turn into a disagreement about a definition remarkably quickly. The contract has to settle these questions in advance, and say what happens when data are missing or disputed.

Three conditions have to hold together. The disagreement has to matter to somebody's decision. The observation has to be verifiable. And the forecasts must differ about that observation in a way relevant to the decision. An emissions record can be excellent evidence about emissions and a poor test of a claim that climate policy will lead to defaults. The emissions, the policy and the financial losses are related through an economic explanation that may itself be disputed. A default count asks the narrower question of how many borrowers fail, which two lenders who disagree about the causes might both accept as a basis for payment.

One further choice concerns where the second forecast comes from. It need not be declared by another lender; a benchmark could instead be constructed from market prices. The extraction method would then belong in the contract. Prices reflect both expectations about outcomes and how much money received in each outcome is worth to investors, and a finite set of quotations can be consistent with several probability assignments. An extracted pricing distribution would therefore need an interpretation before it could serve as a forecast of defaults. In our example both forecasts are declared by the lenders themselves. With a market benchmark, the extraction method and its interpretation would instead sit, unstated, inside the phrase “what the market believes”.

## What should the contract pay?

> “One geometry cannot be more true than another; it can only be more convenient.”
>
> — Henri Poincaré, *Science and Hypothesis* (1905), Chapter III, p. 50.[1]

Poincaré was writing about the geometry of physical space, but there is a literal geometry here too. A forecast over the three default bands is a point whose three coordinates are probabilities adding up to one, and the lenders' forecasts are two such points. Measuring how far apart they are requires a rule for distances between forecasts; the mathematics of such rules is called *information geometry*. There is more than one reasonable rule. Two forecasters might disagree mildly about ordinary outcomes, while another pair agrees almost everywhere and differs sharply about a catastrophe. A geometry that emphasises rare disasters can rank the second pair as further apart; one centred on ordinary predictive performance can reverse the ranking. No geometry is truer than another; once the purpose is fixed, some are more convenient. The lenders' purpose is what decides.

For this contract, the lenders want to reward how well each forecast anticipated an agreed observation. The comparison should depend on what their probabilities say, not on what the categories are called. If the record is made more detailed, the comparison should change when the lenders disagree about the new detail and stay the same when they agree about it; an example of each follows shortly. And a forecaster who seeks the highest expected reward should do best by declaring the probabilities they actually believe.

The comparison should also work over time. Suppose the contract settles first on a report about refinancing conditions and later on defaults. The second settlement should use forecasts made after the refinancing report is known, so that its information is not counted twice. Each settlement can then simply be added to the earlier ones. I want a payment tied to the relative probability of what occurred, with settlements that add up in this way.

I will use a baseline called *relative surprise*. Call the more pessimistic lender A and the other lender B. When the result is known, divide the probability A gave it by the probability B gave it. A twofold ratio earns one unit of payment, a fourfold ratio earns two units, and an eightfold ratio earns three. A ratio of one half loses one unit. Equal probabilities produce no comparison payment. The operation that counts these doublings is the base-two logarithm, and one doubling is called a *bit*; the logarithm also gives intermediate payments for ratios between those values.

Here is the whole contract on one example. A gives the low, middle and high bands 20%, 40% and 40%. B gives them 40%, 40% and 20%. They set the unit at €10,000 per doubling. For now there is no fixed entry fee.

| Defaults over five years | A's forecast | B's forecast | Payment to A |
|---|---|---|---|
| Fewer than 5 | 20% | 40% | −€10,000 |
| 5 to 9 | 40% | 40% | €0 |
| 10 or more | 40% | 20% | +€10,000 |

If ten or more utilities default, A had given that band twice B's probability, and B pays A €10,000. In the low band it is the reverse. In the middle band they agreed, and nothing changes hands. Every amount in the table was fixed before the first default.

We can now see what it would mean to add detail without adding disagreement. Suppose the lenders divide “ten or more” into “ten to fourteen” and “fifteen or more”. They still disagree about the chance of reaching ten defaults. But suppose both say that, *if ten or more defaults occur*, the two more detailed outcomes are equally likely. A therefore divides its 40% into 20% and 20%; B divides its 20% into 10% and 10%. In either new category A still assigned twice B's probability, so the payment remains €10,000. Learning which of these categories occurred gives no further reason to favour one forecast over the other. Later we will examine a different subdivision, in which the lenders also disagree about what happens once defaults reach ten.

A is not paid merely for sounding alarmed. Its higher probability of the high band had to be accompanied by a lower probability elsewhere, here in the low band, where the contract can cost it money. Nor does one win establish general forecasting superiority: B also gave the high band a real chance, one in five. The payment records which forecast assigned more probability to what happened. Whether A forecasts better across repeated observations is a further question.

Why use a logarithm rather than another function of the probability ratio? Three arguments help explain the choice.

The first concerns how forecasts are evaluated. A *scoring rule* is a formula chosen in advance that takes a probability forecast and the outcome that occurs, then returns a number—the *score*. Here higher scores are better. Because a forecast gives a probability to every outcome, a score can reward how much confidence was placed on what happened, not merely whether the most likely category came up. The logarithmic rule takes the logarithm of the probability assigned to the outcome that occurred. In the high band, A's 40% gives a score of about −1.32, while B's 20% gives about −2.32. A's score is higher by one. Multiplying that difference by €10,000 gives the payment in the table.[2]

The scores can be negative; the difference between them determines who pays. More importantly, a rule needs to give the forecaster a reason to report their genuine uncertainty rather than exaggerate confidence. A scoring rule is *proper* when reporting one's actual probabilities maximises the expected score, computed with those same probabilities. It is *strictly proper* when every other report does worse. The logarithmic rule is strictly proper. It is also essentially the only such rule, provided there are at least three possible outcomes, the rule is smooth, and the score uses the reported forecast only through the probability given to the outcome that occurred, a requirement called *locality*. For the payment, which subtracts one lender's score from the other's, the only freedom left is the choice of unit.[2]

The second argument starts from a budget for a different kind of bet. Suppose A pays a stake and receives a non-negative multiple of it when the default band is known. B offers any payment schedule whose expected payout under B's probabilities is no greater than the stake. Among all such schedules, A chooses the one with the highest expected logarithm of the amount returned per unit staked. Logarithms add when successive returns are reinvested, which is why this objective is used to study multiplicative wealth growth. Under this objective, A chooses a multiple equal to A's probability divided by B's: half the stake back in the low band, the stake in the middle, double in the high band.[3] The logarithm of that multiple is relative surprise again. This reinvestment bet and the signed payment in the table are different contracts. A lender maximising expected money would instead stake everything on the high band.

The third argument returns to geometry. A proper scoring rule measures the discrepancy between two forecasts by asking how much expected score a forecaster would lose by reporting the other one. For the logarithmic rule, that loss is the expected relative surprise: 0.2 bits per settlement in the lenders' example. It is not quite a distance, since swapping the two forecasts can change it, but for nearby forecasts it behaves like one, and what it then measures is how readily observations can tell the two forecasts apart.

Suppose we observe many independent borrowers with the same default probability. Under a 50% forecast, 10,000 borrowers give a standard error of half a percentage point, so the gap between 50% and 51% is two standard errors. Under a 1% forecast, the same one-point gap reaches two standard errors with about 400 borrowers, or about 800 if the standard error is computed at 2%. Relative to sampling noise, a one-point difference is far larger near 1% than near 50%; at 1% it is a doubling.

The *Fisher information metric* measures small changes in probabilities against this sampling noise. For a single yes-or-no event, its squared distance is the squared change in probability divided by the variance of one observation. The same one-point change is therefore a larger distance near 1% than near 50%. For nearby forecasts, the expected relative surprise is proportional to this squared distance, so the expected payment is larger where observations can distinguish the forecasts more easily. The first box derives this.[4][16]

This geometry also respects the earlier subdivision of the high band, in which A's 40% became 20% and 20% and B's 20% became 10% and 10%: the extra detail leaves the distance unchanged. Čencov proved that Fisher's metric is, up to scale, the only way of measuring small differences between forecasts that stays unchanged, for every number of outcomes, whenever outcomes are split in proportions both forecasts share.[4] Other measures of disagreement share Fisher's geometry for nearby forecasts, but among proper scoring rules only the logarithm has it everywhere, at a fixed scale.

Other questions call for other geometries. Relative surprise requires no distance between different outcomes: it compares the probabilities assigned to the outcome that occurred. Suppose instead that the lenders want a comparison sensitive to how far their predicted default counts differ. A difference of one default might matter less than a difference of twenty. A *Wasserstein distance* begins by specifying the cost of moving probability from one possible outcome to another, then finds the least total cost of converting one forecast distribution into the other.[14] Where outcomes are actual default counts, that cost could be the difference between the counts. Where outcomes describe losses or electricity shortfalls, it could instead use euros or megawatt-hours.

For the simplest transport distance, there is also a contingent payment whose expected value under A's forecast exceeds its expected value under B's by exactly that distance. The second box constructs the payment and compares it with the logarithmic one. The choice is between specified financial questions, not between a good mathematical distance and a bad one. How to give beliefs a geometry is a rich subject in its own right; here the alternatives show why the financial purpose belongs in the choice of comparison.

<details>
<summary><strong>The mathematics:</strong> scoring rules and the logarithmic comparison</summary>

**Forecasts, scores and units.** Let \(\mathcal Y\) be a finite set of possible outcomes. A forecast \(r\) assigns a strictly positive probability \(r(y)\) to each \(y\in\mathcal Y\), with \(\sum_y r(y)=1\). Write \(p\) for A's beliefs, \(q\) for B's, and \(Y\) for the outcome that will be observed. An expectation \(\mathbb E_p\) uses probabilities \(p\).

A *scoring rule* is a function \(S(r,y)\): it evaluates the report \(r\) when outcome \(y\) occurs, with larger values better. Its expected score under belief \(p\) is

$$
\overline S(p,r)=\mathbb E_p[S(r,Y)]=\sum_{y\in\mathcal Y}p(y)S(r,y).
$$

The rule is *proper* when \(\overline S(p,p)\ge\overline S(p,r)\) for all forecasts \(p\) and \(r\), and *strictly proper* when equality requires \(r=p\). For a proper rule the *regret*

$$
R_S(p,r)=\overline S(p,p)-\overline S(p,r)
$$

is non-negative. It measures the expected score sacrificed by reporting \(r\) instead of \(p\).

For the logarithmic rule, \(S(r,y)=\log_2 r(y)\). Define its relative entropy in bits by

$$
D(p\|q)=\sum_y p(y)\log_2\frac{p(y)}{q(y)}.
$$

Throughout the article, \(D\), entropy \(H\) and mutual information \(I(S;Y)\) use base-two logarithms. Natural logarithms are always written \(\ln\). The signed payment to A is

$$
X(y)=c\,[S(p,y)-S(q,y)]
=c\log_2\frac{p(y)}{q(y)},\qquad c=10{,}000.
$$

Here \(c\) is measured in euros per bit.

**Why base two?** It makes one doubling worth one unit, which keeps the payments in the table simple. The same euro claim can be written \(X(y)=(c/\ln 2)\ln[p(y)/q(y)]\): another base changes the unit of information, \(c\) absorbs the change, and no payment moves.

**1. Honest reporting.** With belief \(p\), the expected logarithmic score of a report \(r\) satisfies

$$
\overline S(p,r)
=\sum_y p(y)\log_2 r(y)
=\sum_y p(y)\log_2 p(y)-D(p\|r).
$$

The first term is independent of the report. Jensen's inequality for the concave logarithm gives

$$
-D(p\|r)
=\sum_y p(y)\log_2\frac{r(y)}{p(y)}
\le\log_2\!\left(\sum_y p(y)\frac{r(y)}{p(y)}\right)
=\log_2 1=0.
$$

Equality requires the ratios \(r(y)/p(y)\) to be constant. Since both forecasts sum to one, that constant is one. The expected score is therefore uniquely highest at \(r=p\). This is Gibbs' inequality and establishes strict propriety. Subtracting the score of a fixed comparator \(q\), then multiplying by \(c>0\), leaves that optimum unchanged, so the signed payment rewards honest reporting too.

For uniqueness, call a score *local* when \(S(r,y)=s_y(r(y))\): only the reported probability of the realised outcome enters the score. Suppose each \(s_y\) is differentiable and the rule is strictly proper throughout the simplex interior, the set of strictly positive probability vectors. At the honest report, maximisation subject to \(\sum_y r(y)=1\) requires

$$
p(y)s_y'(p(y))=\lambda(p)\qquad\text{for every }y.
$$

With at least three outcomes, vary the probability of one while holding a second fixed and adjusting a third to keep the sum equal to one. The expression on the second outcome stays fixed, so the expression on the first must also stay fixed. Since any two interior forecasts can be linked by such moves, every function \(t s_y'(t)\) equals one and the same constant \(a\). Integrating yields

$$
s_y(t)=a\ln t+b_y.
$$

Here \(b_y\) may depend on the outcome but not on the report. Strict propriety requires \(a>0\): a negative coefficient reverses the preference and zero makes every report equally good. Thus smooth local strictly proper scores are logarithmic up to positive scale and outcome-dependent additions.[2]

With two outcomes, fixing one probability fixes the other, so this argument no longer applies. For example, the reward version of the Brier score is

$$
S_{\rm B}(r,y)=-\frac12\sum_{z\in\mathcal Y}
\big(r(z)-\mathbf 1_{\{z=y\}}\big)^2.
$$

Its regret is \(\tfrac12\sum_z(p(z)-r(z))^2\). It is strictly proper and bounded. For two outcomes it reduces to \(-[1-r(y)]^2\), which is also local; with three or more it generally depends on the other entries of the report as well.

**2. A budget for logarithmic growth.** B offers every non-negative payout multiple \(m(y)\) satisfying \(\mathbb E_q[m(Y)]\le1\). A chooses among them to maximise \(\mathbb E_p[\log_2 m(Y)]\), interpreting \(m\) as money returned per unit staked.

Write \(m(y)=[p(y)/q(y)]u(y)\). Then

$$
\begin{aligned}
\mathbb E_p[\log_2 m(Y)]
&=D(p\|q)+\mathbb E_p[\log_2 u(Y)]\\
&\le D(p\|q)+\log_2\mathbb E_p[u(Y)]\\
&=D(p\|q)+\log_2\mathbb E_q[m(Y)]\\
&\le D(p\|q).
\end{aligned}
$$

Equality is obtained by \(u(y)=1\), hence \(m(y)=p(y)/q(y)\). For the lenders this is \((1/2,1,2)\). Its expected payout under B is \(0.4/2+0.4+0.2\times2=1\), and its expected logarithmic return under A is 0.2 bits. In this finite positive setting,

$$
D(p\|q)=\max_{m\ge0,\,\mathbb E_q[m]\le1}
\mathbb E_p[\log_2 m].
$$

This is a form of the Donsker–Varadhan variational identity.[3] Expected money has a different optimum: the ratio schedule returns 1.3 units on average under A, whereas a feasible schedule paying five units only in the high band returns two units on average under A. The latter pays nothing elsewhere and therefore has expected logarithmic return minus infinity.

**3. Local geometry and evidence.** Fix a strictly positive forecast \(p\) and a vector \(h\) satisfying \(\sum_yh(y)=0\). Let \(q=p+\varepsilon h\), where \(\varepsilon\) is small enough that all entries remain positive. The Fisher quadratic form at \(p\) is

$$
g_p(h,h)=\sum_y\frac{h(y)^2}{p(y)}.
$$

For the actual probability change \(\delta=\varepsilon h\), put \(d^2=g_p(\delta,\delta)\). This is the squared *local* length of that displacement at \(p\); it is not the exact finite distance obtained by integrating a metric along a path. Taylor expansion, with \(p\) and \(h\) fixed, gives

$$
D(p\|p+\varepsilon h)
=\frac{\varepsilon^2}{2\ln 2}\sum_y\frac{h(y)^2}{p(y)}
+O(\varepsilon^3)
=\frac{d^2}{2\ln2}+O(\varepsilon^3).
$$

The expected euro payment is therefore approximately \(c d^2/(2\ln2)\).

**Why that quadratic form measures statistical distinguishability.** For one observation define the evidence in bits in favour of \(p\) against \(q\) by

$$
\ell(y)=\log_2\frac{p(y)}{q(y)}
=\frac{1}{\ln2}\left[-\frac{\delta(y)}{p(y)}
+\frac{\delta(y)^2}{2p(y)^2}\right]+O(\varepsilon^3).
$$

The linear term has mean zero under \(p\), because \(\sum_y\delta(y)=0\). Its variance is \(d^2/(\ln2)^2\). The quadratic term has mean \(d^2/(2\ln2)\). Consequently, to leading order, \(n\) independent observations with law \(p\) give a cumulative comparison with

$$
\text{mean}\simeq\frac{n d^2}{2\ln2},\qquad
\text{standard deviation}\simeq\frac{d\sqrt n}{\ln2}.
$$

Their ratio is \(d\sqrt n/2\). Within this local approximation, obtaining the same ratio when the separation \(d\) is halved requires four times as many observations.

For a yes-or-no event, let \(\theta\) be its probability and \(\delta\) a small change. The two changes are \(\delta\) and \(-\delta\), so

$$
d^2=\frac{\delta^2}{\theta}+\frac{\delta^2}{1-\theta}
=\frac{\delta^2}{\theta(1-\theta)}.
$$

The observed frequency in \(n\) independent cases has standard error \(\sqrt{\theta(1-\theta)/n}\). A gap of size \(|\delta|\) equals two standard errors when \(n=4\theta(1-\theta)/\delta^2=4/d^2\). For \(\delta=0.01\), this gives 10,000 at \(\theta=0.5\), 396 at \(\theta=0.01\), and 784 at \(\theta=0.02\). The Taylor expansion needs the relative changes \(|\delta(y)|/p(y)\) to be small; a change from 1% to 2% does not meet that approximation well.

**The relation to likelihood curvature.** In a regular model with a scalar parameter \(\theta\), write \(p_\theta(y)\) for the probability or density of an observation. Assume parameter-independent support and sufficient smoothness and integrability to differentiate the normalisation and expectations. With natural logarithms, the Fisher information in one observation is

$$
I_{\rm F}(\theta)
=\mathbb E_\theta\!\left[\big(\partial_\theta\ln p_\theta(Y)\big)^2\right]
=-\mathbb E_\theta\!\left[\partial_\theta^2\ln p_\theta(Y)\right].
$$

It is the expected *negative* curvature of the log-likelihood. A small parameter change \(\Delta\theta\) has squared local length \(I_{\rm F}(\theta)(\Delta\theta)^2\). For \(n\) independent observations from this model and an unbiased estimator \(\widehat\theta\) satisfying the Cramér–Rao regularity conditions,

$$
\operatorname{Var}_\theta(\widehat\theta)\ge\frac{1}{nI_{\rm F}(\theta)}.
$$

These are two uses of the same local sensitivity: it enters both the discrimination between nearby forecasts and the precision attainable when estimating a parameter.[16]

**Refining categories without adding a disagreement.** Let each original outcome \(y\) be divided into disjoint categories \(z\in\mathcal Z_y\), so that observing \(z\) also identifies \(y\). Specify numbers \(\kappa(z\mid y)>0\) adding up to one for each \(y\). They are the conditional chances of the detailed outcomes once the original outcome is known. Use the same numbers in both forecasts:

$$
p'(z)=p(y)\kappa(z\mid y),\qquad
q'(z)=q(y)\kappa(z\mid y),\qquad z\in\mathcal Z_y.
$$

Then \(p'(z)/q'(z)=p(y)/q(y)\), so the realised logarithmic comparison is exactly unchanged. For a tangent change \(h\), the refined change is \(h'(z)=h(y)\kappa(z\mid y)\), and

$$
\sum_{z\in\mathcal Z_y}\frac{h'(z)^2}{p'(z)}
=\frac{h(y)^2}{p(y)}\sum_{z\in\mathcal Z_y}\kappa(z\mid y)
=\frac{h(y)^2}{p(y)}.
$$

Thus the local Fisher length is unchanged too. In the main example, \(\kappa=(1/2,1/2)\) inside the high band: A's 40% becomes 20% and 20%, while B's 20% becomes 10% and 10%. This is different from the later refinement in which the conditional forecasts are 50–50 and 90–10.

Čencov's theorem identifies Fisher's metric, up to one overall positive scale, among smooth families of Riemannian metrics defined consistently over all finite outcome sets and invariant under the specified recoverable refinements and relabellings.[4] (A Riemannian metric measures local lengths by a positive quadratic form, as \(g_p\) does.)

**What the scoring argument adds.** Many global discrepancies, including the convex-generator divergences defined in the next box, have this local geometry. To select a score, impose an additional condition. For a smooth proper reward score \(S\), define \(G(p)=\overline S(p,p)\), its convex expected score under honest reporting. Its regret can be written

$$
R_S(p,r)=G(p)-G(r)-\nabla G(r)\mathbin{\cdot}(p-r).
$$

This is a Bregman divergence, the difference between the value of the convex function at \(p\) and its tangent-plane prediction from \(r\). For nearby forecasts it equals, to second order, one half of the quadratic form given by the Hessian, or matrix of second derivatives, of \(G\), evaluated on changes whose coordinates sum to zero; the local metric is that Hessian. Put \(F(p)=\sum_y p(y)\ln p(y)\). Its Hessian on those changes is Fisher's metric. If the Hessian of \(G\) equals \(a\) times that of \(F\) throughout the connected simplex interior, with the same constant \(a>0\), then \(G-aF\) has zero Hessian and is affine. The score is therefore logarithmic up to scale and outcome-dependent additions.[2] Requiring the metric only at one forecast would not establish this result.

**Why contributions from successive observations add.** Let \(p(y_1,y_2)\) and \(q(y_1,y_2)\) be joint forecasts for two observations. Their conditional probabilities describe the second observation after the first is known. The chain rule gives

$$
\log_2\frac{p(y_1,y_2)}{q(y_1,y_2)}
=\log_2\frac{p(y_1)}{q(y_1)}
+\log_2\frac{p(y_2\mid y_1)}{q(y_2\mid y_1)}.
$$

No independence assumption is used. Conversely, let \(h\) be a continuous real-valued function of a positive probability ratio. Requiring \(h(ab)=h(a)+h(b)\) for every \(a,b>0\) and \(h(1)=0\) forces \(h(a)=C\log_2 a\). To see this, set \(g(x)=h(2^x)\). Then \(g(x+y)=g(x)+g(y)\), and continuity makes \(g\) linear. An increasing reward fixes \(C>0\).

</details>

<details>
<summary><strong>The mathematics:</strong> other rules, other geometries</summary>

**Setting.** Take strictly positive forecasts \(p\) and \(q\) on the same finite set of outcomes \(\mathcal Y\). Let \(Y\) denote the observed outcome and \(\eta_y=p(y)/q(y)\) its likelihood ratio. In this box \(b>0\) is the number of euros paid per unit of the chosen comparison; to compare payment schedules, we take \(b=10{,}000\), as for the logarithmic contract.

**Is a positive bargaining interval special to the logarithm?** Let A's payment be \(b\,g(\eta_Y)\), where \(g\) is any real-valued non-decreasing function. Then

$$
\begin{aligned}
\mathbb E_p[g(\eta_Y)]-\mathbb E_q[g(\eta_Y)]
&=\sum_y q(y)(\eta_y-1)g(\eta_y)\\
&=\sum_y q(y)(\eta_y-1)\big[g(\eta_y)-g(1)\big]\ge0.
\end{aligned}
$$

The second equality uses \(\sum_yq(y)(\eta_y-1)=0\). In the final sum each pair of bracketed factors has the same sign. If \(p\ne q\) and \(g\) is strictly increasing, the gap is positive.

Suppose both lenders value expected money alone, assess this claim in isolation and settle any fee on the same date as its payment. A's maximum acceptable fee to B is \(b\mathbb E_p[g]\); B's minimum is \(b\mathbb E_q[g]\). Their difference is the width of the interval in which both expect to benefit, so any strictly increasing \(g\) leaves room to trade when the forecasts differ.

**Convex generators.** A differentiable convex function \(\phi:(0,\infty)\to\mathbb R\) with \(\phi(1)=0\) defines an *f-divergence* by

$$
D_\phi(p\|q)=\sum_yq(y)\phi\!\left(\frac{p(y)}{q(y)}\right).
$$

Convexity makes its derivative \(g=\phi'\) non-decreasing, so this derivative supplies a payment function for the preceding argument. The divergence is a number comparing two forecasts; the derivative evaluated at the realised ratio supplies the contingent payment. For smooth generators with \(\phi''(1)>0\), the local expansion is

$$
D_\phi(p+\delta\|p)
=\frac{\phi''(1)}2\sum_y\frac{\delta(y)^2}{p(y)}
+o(\|\delta\|^2),\qquad \sum_y\delta(y)=0,
$$

which explains why many such divergences have the same Fisher geometry locally, up to scale. For example, \(\phi(t)=(\sqrt t-1)^2\) gives the squared Hellinger discrepancy \(\sum_y(\sqrt{p(y)}-\sqrt{q(y)})^2\). Its local form is also proportional to Fisher, although its global values differ from relative entropy.

The choice \(\phi(t)=(t\ln t-t+1)/\ln2\) gives \(g(t)=\log_2 t\). The choice \(\phi(t)=(t-1)^2/2\) gives \(g(t)=t-1\). On the lenders' forecasts the second rule pays \((-0.5,0,1)\) units, compared with \((-1,0,1)\) for the base-two logarithm. Its expectation is zero under B and 0.3 units under A.

A generator does not by itself supply honest reporting. If A reports \(r\) and receives \(b[r(Y)/q(Y)-1]\), its expectation under its actual belief \(p\) is

$$
b\left[\sum_y r(y)\frac{p(y)}{q(y)}-1\right].
$$

This increases as A moves its reported probability towards the outcome with the largest \(p(y)/q(y)\), here the high band, so honest reporting is not the optimum. The logarithmic rule adds the honesty and additivity properties derived in the first box.

**A transport comparison.** Number the three categories 0, 1 and 2, in order from fewer than five defaults to ten or more. Specify a distance of one between neighbouring categories and two between the lowest and highest. In symbols, the distance is \(|i-j|\).

Let \(p_i\) and \(q_i\) be the category probabilities. For \(m\) categories numbered \(0,\ldots,m-1\), define the cumulative probabilities

$$
F_p(k)=\sum_{i=0}^k p_i,\qquad
F_q(k)=\sum_{i=0}^k q_i.
$$

The Wasserstein-1 distance for this equally spaced category scale is

$$
W_1(p,q)=\sum_{k=0}^{m-2}|F_p(k)-F_q(k)|.
$$

Why cumulative probabilities? The difference \(F_p(k)-F_q(k)\) is the excess probability one forecast assigns to categories at or below \(k\). Converting that forecast into the other requires moving that excess across the boundary between \(k\) and \(k+1\). Each boundary has unit distance here; summing the absolute excesses gives the least transport cost.[14]

Kantorovich–Rubinstein duality represents the same number as

$$
W_1(p,q)=\max_{u:\,|u(i)-u(j)|\le|i-j|}
\left\{\mathbb E_p[u(Y)]-\mathbb E_q[u(Y)]\right\}.
$$

Here \(u\) assigns a numerical payment to each category and is allowed to change by no more than the assigned distance between categories. A maximising function \(u\), fixed before the outcome, gives a cash payment \(b\,u(Y)\) whose expected-money bargaining interval has width \(bW_1(p,q)\). Adding a constant to \(u\) shifts both reservation values equally without changing the width.

For the three bands, the cumulative probabilities are \((0.2,0.6,1)\) under A and \((0.4,0.8,1)\) under B. Thus \(W_1=0.2+0.2=0.4\). One optimal schedule is \(u=(-1,0,1)\), giving expectations 0.2 under A and −0.2 under B. With the chosen coefficient \(b=10{,}000\), this happens to reproduce the original logarithmic payments and the €4,000 interval.

Now consider the *informative* subdivision used later in the article: A gives 20% and 20% to ten-to-fourteen and fifteen-or-more defaults, whereas B gives 18% and 2%. Number all four resulting categories 0, 1, 2 and 3, again assigning distance one between neighbours. The calculation is

$$
W_1=0.2+0.2+0.18=0.58,
\qquad u=(-1,0,1,2).
$$

The transport payment has expectations 0.4 under A and −0.18 under B. With the same \(b\), the logarithmic schedule is instead approximately \((-1,0,0.152,3.322)\). It pays most in the last category because A assigned it 20% and B only 2%. The transport schedule rises by one unit between each neighbouring pair because, in this example, A assigns less cumulative probability than B at every boundary. Different cumulative comparisons can make an optimal schedule rise at some boundaries and fall at others.

Assigning the two high categories separate locations was part of this new transport specification. If both retained the old high category's location 2, their transport distance would remain 0.4. The change to 0.58 therefore comes from the chosen distances between the new categories as well as from the more detailed forecasts.

The two comparisons can serve different purposes. A lender wanting payment to increase with the severity of losses might choose distances derived from those losses; one wanting to reward relative anticipation can choose the logarithmic comparison. The transport payment does not by itself reward honest reporting: on this line the schedule depends only on the signs of the cumulative differences, so many different reports produce the same payments.

</details>

## From a payment to a price

Under A's forecast, A expects to receive €2,000 from this contract: a 40% chance of €10,000 against a 20% chance of paying €10,000. B assesses the opposite side under its own probabilities and also expects to gain €2,000. Each expects to profit because each uses its own probabilities; the contract itself is zero-sum, since whatever one lender receives the other pays.

Suppose each lender cares only about expected money, looks at this contract on its own, and any fixed fee is paid on the same date as the comparison payment. A would pay B any fee below €2,000 to enter. B would accept any fee above minus €2,000: a negative fee means B pays A, and B would pay up to €2,000 for its side. Every fee strictly between those limits leaves both expecting to gain, before costs. Zero is one possible fee, and nothing in this calculation singles it out. An auction, a dealer or plain haggling has to produce the actual terms.

The interval is €4,000 wide, and the width has an informational interpretation. A's expected relative surprise is the *Kullback–Leibler divergence* of A's forecast from B's: the average of the logarithmic probability ratio, taken using A's probabilities. It is 0.2 bits here, worth €2,000 at €10,000 per bit. Reversing the forecasts gives B's expected relative surprise, also 0.2 bits in this example but generally a different number. The sum of the two divergences is called the *Jeffreys divergence*. Multiplying it by €10,000 per bit gives the width of the bargaining interval.[3]

<details>
<summary><strong>The mathematics:</strong> expected gains and the bargaining interval</summary>

Take strictly positive probabilities \(p(y)\) and \(q(y)\) on a finite set of outcomes \(y\). They are A's and B's forecasts. Write \(D(p\|q)=\sum_y p(y)\log_2[p(y)/q(y)]\), in bits, and \(c=10{,}000\) euros per bit. The signed payment to A is \(X(y)=c\log_2[p(y)/q(y)]\), with B receiving \(-X(y)\).

Their expected own-side payments, each evaluated under its own forecast, are

$$
\mathbb E_p[X(Y)]=cD(p\|q),\qquad
\mathbb E_q[-X(Y)]=cD(q\|p).
$$

Both are non-negative by Gibbs' inequality and positive when the forecasts differ. For A in the example,

$$
\begin{aligned}
D(p\|q)
&=0.2\log_2\frac{0.2}{0.4}
+0.4\log_2\frac{0.4}{0.4}
+0.4\log_2\frac{0.4}{0.2}\\
&=-0.2+0+0.4=0.2\text{ bits}.
\end{aligned}
$$

By the symmetry of these particular forecasts, \(D(q\|p)=0.2\) bits too.

Let \(f\) be a fixed fee from A to B, paid on the same date as \(X\). Under expected-money valuation, with this claim assessed in isolation and before costs, A strictly prefers the trade when \(cD(p\|q)-f>0\). B strictly prefers it when \(f+cD(q\|p)>0\). Thus both prefer trade exactly when

$$
-cD(q\|p)<f<cD(p\|q).
$$

At either endpoint one side is indifferent. The interval in the example runs from −€2,000 to €2,000. Define the Jeffreys divergence by \(J(p,q)=D(p\|q)+D(q\|p)\). The interval width is \(cJ(p,q)\), here 0.4 bits multiplied by €10,000 per bit, or €4,000.

</details>

Each limit is a *reservation value*: the fee at which that lender would be indifferent between entering the trade and declining it. An actual institution's limits can differ from the €2,000 figures. A lender already heavily exposed to utility failures may value the high-band payment as protection and pay more for it. It may also be unable to deposit the collateral securing its own payment, or lack permission under its mandate to hold the contract at all. Calculating an interval is not evidence that orders already exist within it.

The payment is also protection. If A's loan book loses heavily when defaults are high, the contract offsets part of that loss in exchange for paying out when defaults are low, and it does so while the two lenders go on disagreeing about the transition.

A classic result explains why learning that somebody wants to trade can itself change the calculation. Milgrom and Stokey consider traders whose starting allocation is already efficient: judged by their prior beliefs, no trade could benefit one of them without harming another. The traders agree on how new signals relate to the payoff-relevant outcome. If it then becomes common knowledge that a feasible trade is acceptable to all—each knows this, knows that the others know it, and so on—every trader is indifferent to that trade; with strict risk aversion, the trade is zero.[5] In our expected-money example, both lenders prefer a suitable bet before any new private information arrives. Their starting position therefore does not meet the theorem's efficiency condition. Real demand could also come from hedging needs, mandates and existing exposures.

### Why not use ordinary securities?

The lenders can already act on their views by lending more or less, or by trading bonds. But a bond's return depends on much more than the number of defaults in the sector: interest rates, the amount recovered after a default, and the fortunes of its particular issuer. The proposed contract instead makes payment depend on the specified comparison of the sector forecasts.

That does not make its cash flow new. If existing securities can reproduce the payment in each of the three outcomes, they replicate it, and complete markets in those outcomes would do exactly that. What replication takes as given is everything the lenders have just had to agree: the forecasts, the observation, the fixing date, the rule and the unit. A dedicated contract organises and authenticates that specification and makes it easier to quote and transfer. Differences of logarithmic scores are not new either; prediction markets built on scoring rules already use them.[6] What is proposed here is the combination of declared forecasts, a financial purpose, a settlement procedure and the governance to run it.

A derivative is useful here because the lender can add a payment conditional on the agreed observation while keeping its loans. Buying a utility's equity would bring ownership and exposure to the rest of its business; it would not, by itself, give this forecast comparison a separate payment. The same payment clause could also be included in a funded note or in a loan agreement. A swap creates the stated exchange of payments; an option could give a one-sided entitlement in return for a premium. These forms differ in funding, liability and who is permitted to hold them.

Could publishing the forecasts do the same job? Publication allows scrutiny but moves no money; the contract attaches a payment to the comparison.

## The liability limit changes the comparison

Our example has a reassuring feature: no payment can exceed €10,000 in either direction. That comes from the forecasts, not from the rule. With finer outcomes, probability ratios can become enormous. If A gives some outcome a 10% chance and B gives it one in a million, the payment if it happens is about €166,000. If one side gives an outcome zero probability and the other gives it positive probability, the raw log payment is infinite.

The expected-payout limit in the stake example does not prevent this. It restricts an average under B's forecast, not the largest amount B could owe. The terms must address that liability separately: restrict the permitted probability ratios, specify a maximum payment and secure it with collateral, or change the payment rule. A symmetric cap, for example, replaces a payment larger than €20,000 with €20,000 and a payment below −€20,000 with −€20,000. Capping the payment can destroy honest reporting. In the four-category example in the next section, a cap of €20,000 in either direction allows A to raise its expected payment from about €2,300 to about €4,000 by reporting probabilities different from its actual beliefs.

One alternative keeps the logarithmic rule but sets a minimum probability that either lender may give any outcome. If that minimum is one in a thousand, which requires at most a thousand possible outcomes, no payment can exceed about €99,700 in either direction, and honest reporting remains optimal for any belief that respects the minimum. Another route is a bounded proper rule such as the *Brier score*, which penalises the squared differences between the reported probabilities and the outcome (one for what happened, zero for everything else). It gives a firm liability limit, at the price of the links to evidence and information that the logarithm provides.[2]

Unbounded liability can arise even when both forecasts give every outcome some probability. With infinitely many possible outcomes, every realised payment can be finite while the expected payment under one of the forecasts is infinite. “We'll work out the bill when it arrives” is no answer for the institution that has to value and fund the promise today.

A lender might instead want larger payments on very high default counts. Simply multiplying the logarithmic score by a larger weight on those outcomes would reward exaggerating their probabilities; tail-sensitive proper scores need a different construction. Quotes for contracts with different tail weights and maturities could help show which outcomes and horizons participants most want protection against, provided the forecasts, observations and valuation conventions remain comparable. Otherwise a change in the quote may reflect a changed measuring rule, a dealer's existing positions or financing costs.

## What settlement leaves unresolved

Suppose for a moment that the lenders agreed on the probability of each band but disagreed about which utilities would fail. The three-band contract would pay nothing in every outcome: the probabilities entering the payment would be identical. Yet the disagreement could matter greatly to a lender whose loans were concentrated in the borrowers A considered vulnerable.

Return to the original probabilities and consider a more detailed default count. Divide the high band into ten to fourteen defaults and fifteen or more, as before, but now let the lenders disagree about that detail. A still assigns 40% to the high band, divided equally into 20% and 20%. B assigns 20% in total, divided into 18% and 2%. Thus, conditional on reaching ten defaults, A considers the two new categories equally likely, whereas B gives nine tenths of its high-band probability to ten-to-fourteen and only one tenth to fifteen-or-more. This is different from the earlier subdivision on which they agreed.

The original three-band contract is unchanged, because it still uses only the total probabilities of the high band. A contract using the finer record raises A's expected payment from €2,000 to about €4,950. The additional €2,950 reflects their different conditional predictions within the high band. The three-band contract cannot pay for that difference: once defaults reach ten, it pays the same amount whatever the count. The split is exact: A's expected payment on the detailed record equals the part the three-band record captures plus the expected disagreement left inside the bands, both computed with A's probabilities.[3]

The finer comparison also increases the largest possible payment in this example. If fifteen or more utilities fail, A assigned that outcome ten times B's probability, and B owes about €33,200 instead of €10,000. In general, refining the record can raise either side's largest possible payment but never lower it: the ratio on a coarse band is an average of the ratios on its finer parts, so at least one finer ratio is at least as extreme. A richer record can improve the comparison while making the liability harder to fund.

The disagreement omitted by the settlement record is different from the representational residue of Part I. That residue concerned choices left open while *building* a forecast, such as which outcomes to distinguish or which similarities to rely on. Here the forecasts are already specified, and we are asking what their probabilities imply for one particular observation. Even a complete record of defaults can leave their causes unresolved, including the role of policy and what would have happened under another financing decision.

The contract also gives A a way to assess a possible source of information. Suppose A can receive an early report on refinancing conditions before fixing its forecast, while B's forecast and the other terms stay fixed. A can use its own model to compare the expected payment with and without that report. Averaged over the reports and default outcomes A considers possible, the improvement equals the report's *mutual information* with the default band, multiplied by €10,000 per bit. Mutual information is the average reduction in uncertainty about the band after observing the report.[3]

This values information for the specified contract. Blackwell's comparison of experiments asks a broader question: would one information source be at least as useful in every decision problem? In the finite setting, this holds when the second source can be reproduced from the first by a random transformation of the observed message, using the same transformation regardless of the unknown state. The transformation can discard or obscure information but cannot consult the state itself. This is called a *garbling*. A larger mutual-information value for one particular model and question does not establish that stronger ordering.[7]

<details>
<summary><strong>The mathematics:</strong> what settlement records and what a signal adds</summary>

**Notation and the decomposition.** Let \(Z\) be a detailed outcome on a finite set, and let \(Y=g(Z)\) be the coarser category used for settlement. In the example \(Z\) has four default bands and \(Y\) combines the two high bands into one. A and B specify strictly positive laws \(p_Z\) and \(q_Z\). Their induced probabilities of \(Y\) are \(p_Y\) and \(q_Y\). Write \(D(P\|Q)=\sum_z P(z)\log_2[P(z)/Q(z)]\), in bits, and \(c=10{,}000\) euros per bit.

For \(y=g(z)\), factor \(p_Z(z)=p_Y(y)p(z\mid y)\), and similarly for \(q\). Taking the logarithmic ratio and averaging under A gives

$$
D(p_Z\|q_Z)
=D(p_Y\|q_Y)
+\sum_y p_Y(y)D\big(p(\cdot\mid y)\|q(\cdot\mid y)\big).
$$

The first term is the expected comparison available to a contract on \(Y\). The second is the expected additional comparison available if \(Z\) is recorded too. Both are non-negative.

**The example.** Within the high band A gives conditional probabilities \((0.5,0.5)\) to ten-to-fourteen and fifteen-or-more defaults; B gives \((0.9,0.1)\). Their conditional divergence from A's perspective is

$$
0.5\log_2\frac{0.5}{0.9}
+0.5\log_2\frac{0.5}{0.1}
\simeq-0.424+1.161=0.737\text{ bits}.
$$

A reaches the high band with probability 0.4, so its expected additional comparison is \(0.4\times0.737\simeq0.295\) bits. Adding the original 0.2 gives about 0.495 bits: €2,000 from the coarse contract and about €2,950 more from the refinement. Evaluating the reversed comparison under B gives €2,000 plus about €1,060. The last category has signed payment \(c\log_2(0.2/0.02)\simeq3.322c\), or about €33,200.

**A signal received before reporting.** Let \(S\) be a finite-valued signal with possible values \(s\), and let A specify a joint law \(p_{S,Y}\). Before receiving it, A forecasts \(p_Y(y)\); after receiving \(s\), A can report \(p(y\mid s)\). Assume positive conditional probabilities, keep B's forecast \(q_Y\) and all payment terms fixed, and average under A's joint law. Then

$$
\begin{aligned}
c\,\mathbb E_p\!\left[\log_2\frac{p(Y\mid S)}{q_Y(Y)}\right]
&=c\,\mathbb E_p\!\left[\log_2\frac{p(Y\mid S)}{p_Y(Y)}\right]
+c\,\mathbb E_p\!\left[\log_2\frac{p_Y(Y)}{q_Y(Y)}\right]\\
&=cI(S;Y)+cD(p_Y\|q_Y).
\end{aligned}
$$

The signal's mutual information, in bits, is

$$
I(S;Y)=\sum_{s,y}p(s,y)\log_2\frac{p(s,y)}{p_S(s)p_Y(y)}.
$$

It is the relative entropy between A's joint law and the law making the signal and outcome independent while retaining their marginal probabilities. Equivalently,

$$
\begin{aligned}
H(Y)&=-\sum_y p_Y(y)\log_2 p_Y(y),\\
H(Y\mid S)&=\sum_s p_S(s)\left[-\sum_y p(y\mid s)\log_2 p(y\mid s)\right],\\
I(S;Y)&=H(Y)-H(Y\mid S).
\end{aligned}
$$

Since \(H(Y\mid S)\ge0\), the expected-payoff improvement \(cI(S;Y)\) cannot exceed \(cH(Y)\). A's probabilities \((0.2,0.4,0.4)\) give \(H(Y)\simeq1.52\) bits, so no signal can raise A's expected payment by more than about €15,200.

</details>

## A quote is not a consensus probability

Once the contract trades, someone will want to infer the probability “the market” gives to the adverse outcome. A single quote does not generally supply it. Even in a model that prices by expected payments alone, the value of our signed contract depends on the high-band probability minus the low-band probability. Many three-band forecasts have the same difference. The quote therefore need not identify the whole forecast, even before considering the other reasons an institution might value the payment.

A larger collection of quotes can constrain the interpretation more tightly, but it still requires an economic model. The absence of arbitrage requires consistent prices for identical payments. It does not choose whose probabilities become a public forecast. That depends on the participants, their capacity to bear risk, their resources and the arrangement through which they trade.

One specific economy shows what such a model looks like. Suppose participants can trade a payment for every possible outcome, and each has exponential utility, meaning that their tolerance for risk, measured in euros, does not change with their wealth. Competitive trading then pools the probabilities they trade on in a particular way: it takes a weighted average of the logarithms of their probabilities, weighting each participant by risk tolerance, converts the result back from logarithms, and rescales it so that it sums to one. Prices also depend on how total resources vary across outcomes, so even here the pooled forecast and the prices are two different objects.[8]

The choice of economy matters. Give two participants equal risk tolerance and event probabilities of 80% and 99%. Their ordinary average is about 90%. This economy instead averages the logarithms of their odds, 4 to 1 and 99 to 1, with equal weight, and converting that average back to a probability gives about 95%. If aggregate resources are the same whether or not the event happens, 95% is also the event's *normalised state price*: the price of one euro paid if the event happens, divided by the price of one euro paid for certain. Change the risk-sharing arrangement and the pooling rule can change too.[8]

<details>
<summary><strong>The mathematics:</strong> where the geometric pool comes from</summary>

Consider finitely many outcomes \(\omega\) and participants indexed by \(i\). Participant \(i\) has a strictly positive probability law \(p_i(\omega)\) and utility \(u_i(x)=-e^{-x/\tau_i}\), with constant absolute risk tolerance \(\tau_i>0\), measured in euros. Its final consumption or wealth in outcome \(\omega\) is \(x_i(\omega)\). All outcome-contingent transfers are tradable and there are no further position constraints.

Let \(\pi(\omega)>0\) be today's price of one euro paid only in outcome \(\omega\), and \(w_i\) participant \(i\)'s initial budget at those prices. The participant maximises expected utility subject to \(\sum_\omega\pi(\omega)x_i(\omega)\le w_i\). For an interior optimum, a positive budget multiplier \(\lambda_i\) gives

$$
\frac{p_i(\omega)}{\tau_i}e^{-x_i(\omega)/\tau_i}
=\lambda_i\pi(\omega),
$$

and hence, taking natural logarithms,

$$
x_i(\omega)=\tau_i\left[\ln p_i(\omega)-\ln\pi(\omega)
-\ln(\lambda_i\tau_i)\right].
$$

Write \(e(\omega)\) for total resources in that outcome and \(T=\sum_i\tau_i\) for aggregate risk tolerance. Market clearing requires \(\sum_i x_i(\omega)=e(\omega)\). Summing the preceding equation yields

$$
\pi(\omega)\propto
\left[\prod_i p_i(\omega)^{\tau_i/T}\right]e^{-e(\omega)/T}.
$$

The normalised geometric pool is the probability law

$$
\overline p(\omega)=
\frac{\prod_i p_i(\omega)^{\tau_i/T}}
{\sum_{\omega'}\prod_i p_i(\omega')^{\tau_i/T}}.
$$

State prices contain an additional resource factor: payments in outcomes with fewer total resources are valued more highly. Their normalisation is \(\pi(\omega)/\sum_{\omega'}\pi(\omega')\), and it coincides with \(\overline p\) only if \(e(\omega)\) is constant. Budgets determine the multipliers and the individual allocations; with beliefs, risk tolerances and aggregate resources fixed, they do not change this pool.[8]

For two equally risk-tolerant participants giving a binary event probabilities 80% and 99%,

$$
\overline p(\text{event})=
\frac{\sqrt{0.8\times0.99}}
{\sqrt{0.8\times0.99}+\sqrt{0.2\times0.01}}
\simeq0.952.
$$

Their event odds are \(0.8/0.2=4\) and \(0.99/0.01=99\). Equal weighting of log odds gives pooled odds \(\sqrt{4\times99}\); dividing those odds by one plus themselves gives the same probability.

</details>

Quotes at several maturities could also be used to estimate how quickly participants expect a disagreement to diminish, but only through a dynamic model linking future forecast differences to the quoted payments, and the estimate would depend on that model as much as on the quotes.

## Can a record of payments become evidence?

A five-year contract gives one five-year observation. Marking it to market every day does not turn it into thousands of independent tests. Learning faster requires genuinely new observations, with the forecasts committed before each one arrives.

There is a rigorous way to turn sequential forecast comparisons into an evidence record. Return to the bet that pays a non-negative multiple of its stake, rather than the signed contract in the table. Start an account with one euro. Before each observation, choose a bet whose expected payout under B's forecast, given the record so far, is no greater than the account balance being staked. Reinvest the payout, add no outside money, and never allow a negative balance. Under B's model, the expected next balance is then at most the present balance. A sufficiently large increase can be evidence against that model.[9]

Ville's inequality bounds how often this procedure could produce a misleadingly large balance. If B's model generates the observations, the probability that the account ever reaches €100 is at most one in a hundred. The bound already includes the possibility of checking after every observation and stopping when that balance is reached. It is not a 99% posterior probability that B is wrong. Independent observations are unnecessary: the forecast for each new observation must condition on the available past, and the bet must satisfy the expected-payout restriction under that conditional forecast. This allows, for example, a forecast of this year's defaults to depend on last year's economy.[9]

The bookkeeping is part of the result. Forecasts must come before outcomes, and the rules deciding which contracts count must come before the results. Losses stay in the account. Restarting after a bad year, or publishing only the contracts that went well, changes what is being tested. A proprietary method can choose the bets, but an auditor has to be able to check that the complete account followed the declared rules. A profitable trading book built with arbitrary prices and leverage is not an account of this kind, however good its returns.

How long would this take for our lenders? Imagine a fresh, statistically identical cohort at each five-year renewal, with the same forecasts and independent results. This is a deliberately simple, stationary experiment. The evidence account is a separate, notional ledger that reinvests its balance: with likelihood-ratio bets, each high-band outcome doubles it and each low-band outcome halves it, while the signed contract simply pays €10,000 one way or the other. The account first exceeds €100 when A's cumulative comparison payments reach €70,000. Under A's forecast, that takes 35 renewals on average: 175 years. The median is 29 renewals, and in about one case in nine it takes more than 60, or over three centuries. Under B's forecast, the chance of ever crossing is 1 in 128.

The 175 years is the expected wait for one evidence threshold in a sparse experiment. The contract itself pays after five years, and its protection can affect A's decisions from the day the terms are agreed. Each observation contributes 0.2 bits of evidence on average under A, the same 0.2 bits that set A's expected payment. Raising the monetary unit enlarges the transfers; it does nothing to speed up the evidence.

A well-kept account can produce strong evidence against B's forecast on the observations used for settlement. It cannot, however, tell apart explanations that give those observations the same probabilities. The rate at which genuinely informative observations arrive remains part of the investment problem.

<details>
<summary><strong>The mathematics:</strong> Ville's inequality and the 175 years</summary>

**The account.** Measure the account balance in units of its initial one-euro stake and put \(K_0=1\). Before observation \(t\), let \(q_t(y)\) be B's conditional probability of outcome \(y\), given everything observed so far. Choose non-negative multiples \(m_t(y)\), using only that past information, with \(\sum_y q_t(y)m_t(y)\le1\). After observing \(y_t\), set \(K_t=K_{t-1}m_t(y_t)\). Under the law \(Q\) specified by B's conditional forecasts,

$$
\mathbb E_Q[K_t\mid\text{past}]\le K_{t-1}.
$$

Such a process is called a non-negative *supermartingale*: given its past, its next balance has expectation no greater than its current balance.

**Ville's inequality.** Under the reference law \(Q\), for any chosen error bound \(0<\alpha<1\),

$$
\Pr_Q\big(K_t \ge 1/\alpha \text{ for some } t\big) \;\le\; \alpha .
$$

Proof. Let \(\tau\) be the first time the account reaches \(1/\alpha\), and fix a horizon \(n\). Stopping at the earlier of \(\tau\) and \(n\) cannot raise the expected balance above its starting value of 1 (the optional stopping theorem), and on the event \(\tau \le n\) the balance is at least \(1/\alpha\). So \(\Pr(\tau \le n)/\alpha \le 1\) for every \(n\), and letting \(n\) grow gives the result. With \(\alpha = 1/100\), the account reaches €100 with probability at most 1%.

**The lenders.** For independent renewals with fixed forecasts \(p=(0.2,0.4,0.4)\) and \(q=(0.4,0.4,0.2)\), use \(m(y)=p(y)/q(y)\). Let \(c=10{,}000\) euros per bit and let \(L_n\) be the cumulative signed comparison payment to A through \(n\) renewals. Then \(L_n=c\log_2K_n\). Each renewal adds −1, 0 or +1 to \(\log_2K_n\). The account crosses 100 when \(\log_2K_n\ge\log_2 100\simeq6.64\). Its logarithm is an integer in this example, so the first crossing is at seven bits, a balance of 128 times the initial stake and a net signed payment of €70,000.

Under A's law \(P\), the increments −1, 0, +1 have probabilities 0.2, 0.4, 0.4 and mean 0.2. Let \(S_n=\log_2K_n\), and let \(T\) be its first hitting time of seven. To apply Wald's identity at this possibly unbounded time, first show that \(\mathbb E_P[T]\) is finite. The event \(T>n\) implies \(S_n<7\). For \(n\ge70\), bounded independent increments give the Hoeffding bound \(\Pr_P(T>n)\le e^{-n/200}\). Summing these tail bounds establishes finite expectation. Since the walk reaches exactly seven at \(T\), Wald's identity now gives

$$
7=0.2\,\mathbb E[T],\qquad \mathbb E[T]=35.
$$

The median and tail probability can also be obtained without simulation. Under A's law, let \(v_n(j)\) be the probability of being at \(j<7\) after \(n\) renewals without having reached seven. Start with \(v_0(0)=1\), use

$$
v_{n+1}(j)=0.2v_n(j+1)+0.4v_n(j)+0.4v_n(j-1),\quad j<7,
$$

and discard mass absorbed at seven. Then \(\Pr(T>n)=\sum_{j<7}v_n(j)\). This deterministic recursion gives median 29 and \(\Pr(T>60)=0.11329248\).

Under B's law, the increments −1, 0, +1 have probabilities 0.4, 0.4, 0.2. Ignoring the zero increments leaves an upward probability of one third and a downward probability of two thirds. The probability that this downward-drifting walk ever reaches seven is \([(1/3)/(2/3)]^7=1/128\), about 0.78%, consistent with Ville's upper bound of 1%.

</details>

### What “eventually” means

> “But this long run is a misleading guide to current affairs. In the long run we are all dead. Economists set themselves too easy, too useless a task if in tempestuous seasons they can only tell us that when the storm is long past the ocean is flat again.”
>
> — John Maynard Keynes, *A Tract on Monetary Reform* (1923), Chapter III, p. 80.[10]

Suppose the renewals continue without a final date. For this next calculation, each lender specifies all its forecasts in advance and treats the renewals as independent. The probabilities may change from one renewal to the next, but they do not depend on results already observed, and every possible outcome has positive probability under both forecasts.

There are two questions. Could a rule given the *complete infinite history* identify which of the two probability models generated it, with probability one of being correct under either model? And do the expected net comparison payments, added up without discounting, remain finite? Kakutani's theorem answers the first question; the expected-payment calculation supplies the second. Together they give three cases.[11]

**No error-free identification, finite expected net total.** Even with the complete infinite history, no rule can select between the two models with probability one of being correct under each. The cumulative signed payments converge to a finite net amount, and each lender's expected own-side total is finite. The forecasts may differ at every renewal; the box gives an example in which those differences decrease sufficiently quickly.

**No error-free identification, an infinite expected net total on at least one side.** The statistical conclusion is the same, and the net total along almost every history is still finite. But rare, very large transfers make at least one lender's expected net total infinite. This concerns undiscounted payments. In the box's example, ordinary geometric discounting makes the expected discounted payments finite.

**Identification in the infinite-history limit.** Here the complete history does admit a rule that identifies the generating model with probability one under either law. As observations accumulate, the logarithmic comparison tends to plus infinity under A's law and minus infinity under B's. The lenders' unchanged forecasts, repeated independently, give this case. All three cases assume that one of the two forecasts is the true law.

The first two cases still allow strong evidence at an error rate chosen in advance; what they rule out is certainty. And even in the third case, nothing guarantees a verdict by any given date: every finite run of results remains possible under both forecasts. Our two parties did not need one. They agreed a five-year payment and can decide whether to renew it when the time comes.

> *The contract can settle long before the argument does.*

<details>
<summary><strong>The mathematics:</strong> infinite histories and expected net payments</summary>

**Setup.** At renewal \(k\), let \(p_k\) and \(q_k\) be A's and B's strictly positive probability vectors on a finite outcome set. All these vectors are specified before any results are observed. Renewals are independent under both models, so the laws of the complete history are the product measures \(P=\bigotimes_{k\ge1}p_k\) and \(Q=\bigotimes_{k\ge1}q_k\). Adaptive conditional forecasts need not produce product laws; the preceding supermartingale argument allows such adaptation, whereas the product theorem here does not automatically extend to it.

For outcomes \(Y_1,\ldots,Y_n\), define the likelihood ratio and cumulative signed payment

$$
R_n=\prod_{k=1}^n\frac{p_k(Y_k)}{q_k(Y_k)},\qquad
L_n=c\log_2R_n,
$$

where \(c>0\) is the euro amount per bit. Write \(D\) for relative entropy in bits. The *Hellinger affinity*

$$
\rho_k=\sum_y\sqrt{p_k(y)q_k(y)}
$$

lies in \((0,1]\), with value one exactly when the two forecasts agree.

**Kakutani's distinction.** The complete-history laws are either *equivalent*, meaning that they give probability zero to the same events, or *mutually singular*, meaning that an event has probability one under one law and zero under the other. Equivalence holds exactly when

$$
\prod_{k\ge1}\rho_k>0,
\quad\text{equivalently}\quad
\sum_{k\ge1}(1-\rho_k)<\infty.
$$

If the product is zero, the laws are singular. In the equivalent case \(R_n\) converges under either law to a finite, strictly positive limit, so \(L_n\) converges to a finite net total. In the singular case \(R_n\to\infty\) under \(P\) and \(R_n\to0\) under \(Q\), almost surely; the signed logarithmic total diverges in the corresponding direction.[11]

**Unchanged forecasts.** For the lenders,

$$
\rho=\sqrt{0.2\times0.4}+0.4+\sqrt{0.4\times0.2}
\simeq0.966<1.
$$

Thus \(\rho^n\to0\), and their product laws are singular. The likelihood-ratio account grows without bound almost surely under A's model and tends to zero almost surely under B's.

**Decreasing differences and finite expected totals.** Fix a strictly positive vector \(p\) and a nonzero vector \(h\) whose coordinates sum to zero. Assume \(p(y)+h(y)>0\) for each outcome, and set \(p_k=p\), \(q_k=p+h/k\). Each forecast is then strictly positive. Taylor expansion gives \(1-\rho_k\), \(D(p_k\|q_k)\) and \(D(q_k\|p_k)\) of order \(1/k^2\). The series are finite: the complete-history laws are equivalent and both expected net totals are finite.

**Equivalent histories with an infinite undiscounted expectation.** For \(k\ge1\), give each renewal a rare event and its complement. A assigns the rare event probability \(a_k=1/(k+1)^2\), while B assigns \(b_k=a_ke^{-k}\). Thus \(p_k=(a_k,1-a_k)\) and \(q_k=(b_k,1-b_k)\). Their entries are positive and \(1-\rho_k\) is of order \(1/k^2\), so the history laws are equivalent. However,

$$
\begin{aligned}
D(p_k\|q_k)
&=a_k\log_2\frac{a_k}{b_k}
+(1-a_k)\log_2\frac{1-a_k}{1-b_k}\\
&=\frac{k}{(k+1)^2\ln2}+O(k^{-2}).
\end{aligned}
$$

The leading term is of order \(1/k\), whose sum diverges. Under A, only finitely many rare events occur almost surely because \(\sum_k a_k<\infty\); the same is true under B. Each realised rare-event payment is finite, and the common-outcome payments have a summable magnitude of order \(1/k^2\). The net total is therefore finite almost surely, even though A assigns it an infinite expectation.

**The separate expectation question.** At each finite horizon,

$$
\mathbb E_P[L_n]=c\sum_{k=1}^nD(p_k\|q_k),\qquad
\mathbb E_Q[-L_n]=c\sum_{k=1}^nD(q_k\|p_k).
$$

Finite total Jeffreys divergence, the sum of both directional series, implies equivalent histories and finite own-side expectations of the terminal net amount. Equivalence alone does not imply finite expectations, as the rare-event example shows.

In that example, discounting renewal \(k\)'s payment by \(\beta^k\), for \(0<\beta<1\), makes the expected absolute discounted payments under A of order \(\beta^k/k\), a summable series. An infinite undiscounted expectation therefore does not imply an infinite present value.

</details>

## Who writes the test?

> “[A]s a rule, regulation is acquired by the industry and is designed and operated primarily for its benefit.”
>
> — George J. Stigler, “The Theory of Economic Regulation” (1971), p. 3, excerpt.[12]

Our lenders needed a default definition before they needed a logarithm. Once that definition moves payments, spreads or capital requirements, people have reasons to influence it. Excluding a particular restructuring, moving the observation date or changing how mergers are treated can shift money without changing anyone's view of the transition. Stigler argued that an industry tends to acquire the regulation written for it. The definitions behind a contract like this one face the same pressure, and even the technical appendix can become a site of negotiation.

A proper score makes honesty optimal when the expected score is all the forecaster cares about. In a market, a declared forecast can also move the entry price, the collateral required or the value of another position the forecaster holds, and those effects belong in the incentive calculation too. Research on market scoring rules shows that honest reporting is optimal for a trader who considers only the current trade, but not always for one who plans later trades; it depends on how the traders' information is related.[6] A good score therefore has to come with a price-formation procedure and controls against these outside incentives: depending on the design, disclosure, position limits or penalties.

The observed defaults and their reporting can also respond to the contract. A lender might delay recognising distress until after the fixing date, or change refinancing decisions in ways that alter which utilities default. Some responses could improve the underlying situation; others could improve only the recorded result. Goodhart's warning concerns a statistical regularity breaking down when it is used for control.[13]

So the rulebook needs a stated purpose and a revision history. Whom is the protection meant to serve? Which exposures does the chosen count leave out? Why trust this data provider, and what happens when its methods change? Each amendment should keep the old definition, the new one, the reason for the change and the treatment of contracts already outstanding. An institution that asks lenders to commit to forecasts in advance cannot keep the right to change its own test after seeing the results.

Access matters too. A bank with a technical team can argue for its preferred default definition in detail. The beneficiaries of a pension fund, whose protection depends on that definition, rarely have the time or expertise to argue back. A consultation that is formally open is not enough: the people who bear the unresolved risks need a practical way to contest how their exposure has been written down.

## Where it could be used first

None of this needs a public exchange to begin. Take a bank that publishes a view of the transition and also lends to the sector. Its published view and the assumptions in its lending can be compared, but only once both are translated into forecasts of something observable: defaults, investment, or another agreed record. A contract can then attach money to the comparison. It would not show whether the published view was sincere. And a payment between two parties does not by itself benefit anyone else; that requires useful insurance, a better allocation of capital, or investment that happens on better terms because of the contract.[5]

The utilities also offer observations closer to the physical transition itself: electricity delivered, fuel consumed and emissions under an agreed accounting boundary. Jean-Marc Jancovici has emphasised that energy's physical importance is not measured by its share of monetary expenditure.[15] A disagreement about whether these utilities can maintain output while reducing fuel use could be written as competing forecasts of those quantities. An authenticated annual record could then test that particular claim before a five-year default count arrives.

The activity covered by the measurement matters. A fall in emissions can result from closing a plant rather than improving its technology, so the record may need to specify electricity output, which plants are included and how that coverage changes. Physical quantities provide evidence against which forecasts can be assessed; the relationship between those quantities and cash flows still needs an economic explanation. A payment for forecast performance also differs from charging an emitter for environmental damage. The promising connection is specific: make financial commitments depend on declared, verifiable predictions about energy, materials and production, while separately identifying who bears the social costs.

Adoption could proceed in stages: internal diagnostics first, then bilateral contracts, and a public venue only if demand justifies one. At each stage the question is what changes in actual decisions. Does the new quote explain lending terms, collateral or investment beyond what ordinary prices already explain? Do the data and dispute procedures hold up when used by parties with every reason to challenge them? Those are questions about institutions, and the mathematics of the payment rule cannot answer them.

## What has actually been settled?

Five years on, eleven of the hundred utilities have defaulted. Under the original three-band contract, B pays A €10,000.

B still attributes most of the failures to interest rates rather than the industrial transition. The payment need not persuade B otherwise: both lenders had allowed for the high-default outcome, and their agreement was about how their different forecasts would be compared. What matters now is that the obligation has been honoured. A received money in the outcome to which it had assigned more weight, on terms that B was willing to accept before either knew the result.

To judge the value of that arrangement, however, we should return to the day it was signed. A lender exposed to utility failures could use the high-band payment to offset part of its losses, accepting the cost of the opposite payment when defaults stayed low. At a suitable price and scale, that protection could change which loans it was prepared to keep or make. A counterparty with a different forecast or a different balance sheet could take the other side. Their disagreement would then help determine how the risk was carried, while research into the transition continued. The contract could be useful years before the evidence became conclusive.

The same construction makes the comparison itself available for scrutiny. Instead of looking at two lending books and trying to infer what their owners believe, a third party can examine the forecasts, the observation on which they differ, and the terms on which that difference is being exchanged. Further research can improve those forecasts; better evidence can reveal a distinction the original settlement missed; a new contract can make that distinction available to investors. Each improvement has an identifiable consequence for what can be priced, held or transferred.

This is the constructive promise of contracts like this one: giving a financially consequential difference in understanding an exposure of its own, with terms that others can inspect and, where there is demand, trade. Whether a particular design earns its place depends on the decisions it improves and the protection it provides relative to the alternatives. The wider ambition is a financial system in which the work of understanding an uncertain future has more ways to affect the commitments made to it. Better understanding should be able to change what gets financed before it changes everybody's mind.

## References and notes

The utilities, default bands, probabilities and euro payments are constructed illustrations. The €10,000 unit uses base-two logarithms; another base changes only the monetary unit. The initial table and the conclusion use the original three-band contract with no fixed entry fee. Reservation-value comparisons settle all amounts on the same date, before costs, and assume expected-money maximisation for the isolated claim. The renewal figures use independent five-year observations of fresh statistically identical cohorts with unchanged forecasts; the mean of 35 renewals is exact, and an exact probability recursion gives the median and the one-in-nine tail.

For the capped example, the finer forecasts are A = (20%, 40%, 20%, 20%) and B = (40%, 40%, 18%, 2%), with payments clipped at two units: honest reporting yields A about €2,300 in expectation, and the best misreport about €4,000. None of these examples reports a live contract, a demonstrated investment return or a current regulatory rule.

Related reading: [All Roads Lead to Disagreement (I): Why Two Careful Analysts Can Still Disagree](https://aurelien-giroux.github.io/blog-finance/p/all-roads-lead-to-disagreement-1/) and [What Can a Market See?](https://aurelien-giroux.github.io/blog-finance/p/what-can-a-market-see/).

[1] Henri Poincaré, *Science and Hypothesis*, translated by W. J. Greenstreet (Walter Scott Publishing, 1905), Chapter III, p. 50 in the edition transcribed by the Brock University Mead Project. Poincaré wrote about the geometry of physical space. The text applies his remark to geometries on the space of probability forecasts, the subject of information geometry.

[2] José M. Bernardo, “Expected Information as Expected Utility”, *The Annals of Statistics* 7(3), 686–690 (1979), especially pp. 688–689; Tilmann Gneiting and Adrian E. Raftery, “Strictly Proper Scoring Rules, Prediction, and Estimation”, *Journal of the American Statistical Association* 102(477), 359–378 (2007). Locality means dependence on the reported law only through the probability or density assigned to the realised outcome. The finite-outcome uniqueness statement requires at least three outcomes, strict propriety and interior regularity. The proper-score/Fisher argument additionally requires a smooth convex score generator whose tangent Hessian is a fixed positive multiple of Fisher throughout the simplex interior. Propriety concerns maximising expected score; monetary risk aversion and other payoffs require separate incentive analysis.

[3] Yury Polyanskiy and Yihong Wu, *Information Theory*, MIT 6.441 course notes (2016), Chapters 2–3: relative entropy, its chain rule, mutual information and the Donsker–Varadhan variational representation. The stake argument assumes that the two laws give probability zero to the same outcomes and that the expected logarithm is finite. For the uncapped log comparison, each party's expected own-side gain is its directional relative entropy; their sum is the Jeffreys divergence. The observation split uses the average conditional relative entropy under the first law. The signal-value statement holds under the benchmark joint law, with the comparator and payment convention fixed and no signal-dependent entry price.

[4] N. N. Čencov, *Statistical Decision Rules and Optimal Inference* (American Mathematical Society, 1982); Hiroshi Nagaoka, “The Fisher Metric as a Metric on the Cotangent Bundle”, *Information Geometry* (2024), Theorem 7.1, DOI: 10.1007/s41884-023-00126-9. The uniqueness is for a family of metrics respecting the specified information-preserving Markov embeddings. Local Fisher geometry alone does not determine a global divergence.

[5] Paul Milgrom and Nancy Stokey, “Information, Trade and Common Knowledge”, *Journal of Economic Theory* 26(1), 17–27 (1982); Jack Hirshleifer, “The Private and Social Value of Information and the Reward to Inventive Activity”, *The American Economic Review* 61(4), 561–574 (1971), especially p. 561. The no-trade theorem (Milgrom and Stokey, Theorem 1, p. 21) assumes weakly risk-averse traders; “concordant” beliefs, meaning agreement on how signals relate to the payoff-relevant state, which is weaker than a common prior; an initial allocation that is Pareto-optimal relative to prior beliefs; and common knowledge that the payoff-state-contingent trade is feasible and weakly preferred by each. Its conclusion is that every trader is indifferent to the trade; strict risk aversion makes the trade zero. Hirshleifer separates private informational advantage from social value; disagreement alone establishes neither trading demand nor welfare improvement.

[6] Robin Hanson, “Combinatorial Information Market Design”, *Information Systems Frontiers* 5(1), 107–119 (2003); Yiling Chen, Stanko Dimitrov, Rahul Sami, Daniel M. Reeves, David M. Pennock, Robin Hanson, Lance Fortnow and Rica Gonen, “Gaming Prediction Markets: Equilibrium Strategies with a Market Maker”, *Algorithmica* 58(4), 930–969 (2010; online publication 2009). Market scoring rules already use differences between scores. The proposed comparison does not claim to invent that operation; it specifies the forecasts, financial purpose, settlement and governance together.

[7] David Blackwell, “Equivalent Comparisons of Experiments”, *The Annals of Mathematical Statistics* 24(2), 265–272 (1953). The finite comparison of experiments concerns all decision problems under its conditions and uses a state-independent stochastic kernel for garbling. For a proof of the finite theorem, see Henrique de Oliveira, “Blackwell's Informativeness Theorem Using Diagrams”, *Games and Economic Behavior* 109, 126–131 (2018).

[8] Michail Anthropelos and Constantinos Kardaras, “Equilibrium in Risk-Sharing Games”, *Finance and Stochastics* 21, 815–865 (2017), especially Sections 2.3–2.6 and Theorem 2.2. The text uses the competitive, complete-market exponential-utility benchmark, not the paper's strategic equilibrium. The paper's geometric price measure uses endowment-adjusted beliefs. Equivalently, keeping physical beliefs separate gives a risk-tolerance-weighted geometric pool together with a state-dependent aggregate-resource factor in state prices. Initial budgets are still required for the allocation.

[9] Glenn Shafer, Alexander Shen, Nikolai Vereshchagin and Vladimir Vovk, “Test Martingales, Bayes Factors and p-Values”, *Statistical Science* 26(1), 84–101 (2011), discussing Ville's inequality and non-negative evidence accounts. The threshold bound holds under the reference law for the complete, pre-registered account.

[10] John Maynard Keynes, *A Tract on Monetary Reform* (Macmillan, 1923), Chapter III, p. 80. Keynes was criticising long-run arguments in the quantity theory of money; the use here is an analogy.

[11] Shizuo Kakutani, “On Equivalence of Infinite Product Measures”, *Annals of Mathematics* 49(1), 214–224 (1948). For independent renewals with equivalent component laws, a positive product of Hellinger affinities, equivalently a finite sum of one minus those affinities, gives equivalence of the complete-history laws; a zero product gives singularity. The additional question of finite undiscounted expected log payments depends on the sum of the directional relative entropies, not on Kakutani's dichotomy alone. The product theorem applies to component laws specified independently of the realised history; it does not automatically extend to adaptive forecasts.

[12] George J. Stigler, “The Theory of Economic Regulation”, *The Bell Journal of Economics and Management Science* 2(1), 3–21 (1971), p. 3. The quotation is an excerpt from his statement of the paper's central thesis; the capitalised opening is marked with brackets.

[13] C. A. E. Goodhart, “The ECB and the Conduct of Monetary Policy: Goodhart's Law and Lessons from the Euro Area”, *Journal of Common Market Studies* 44(4), 757–778 (2006), DOI: 10.1111/j.1468-5965.2006.00661.x; Donald MacKenzie, *An Engine, Not a Camera: How Financial Models Shape Markets* (MIT Press, 2006). Goodhart's own restatement is used here for the control-pressure warning, rather than attributing a later popular paraphrase to the original 1975 paper.


[14] Gabriel Peyré and Marco Cuturi, *Computational Optimal Transport*, *Foundations and Trends in Machine Learning* 11(5–6), 355–607 (2019); author version arXiv:1803.00567v4. Section 2.6, Remark 2.30, equations (2.37)–(2.38) gives the one-dimensional cumulative-distribution formula. Section 6.1, Proposition 6.1 and equations (6.1)–(6.2) gives the one-potential Kantorovich–Rubinstein duality used in the second box. Sections 8.1 and 8.2.1 discuss convex-generator divergences and transport comparisons.

[15] Jean-Marc Jancovici, “[L'énergie, de quoi s'agit-il exactement ?](https://jancovici.com/transition-energetique/l-energie-et-nous/lenergie-de-quoi-sagit-il-exactement/)”, author website, first published 1 August 2011; accessed 26 September 2026. The cited observation concerns energy's physical role compared with its share of monetary expenditure. The contractual application is developed here, not attributed to Jancovici.

[16] John Duchi, *Statistics 311 / Electrical Engineering 377: Information Theory and Statistics*, Stanford University lecture notes, Chapter 8, Sections 8.1–8.3, especially equations (8.1.1)–(8.1.2) and the Cramér–Rao discussion in Section 8.2. These support the regular-model Fisher information, negative expected log-likelihood curvature and estimation-bound statements.