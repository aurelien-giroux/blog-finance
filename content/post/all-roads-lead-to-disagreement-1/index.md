---
title: "All Roads Lead to Disagreement (I): Why Two Careful Analysts Can Still Disagree"
description: "Two analysts can share the data, the mathematics and the good faith, and still value the same asset differently. This is an essay about what is left over when everything that can be settled has been settled."
slug: "all-roads-lead-to-disagreement-1"
author: "Aurélien Giroux"
draft: false
date: 2026-09-21
math: false
categories:
  - Finance
  - Epistemology
---

> “About these matters there is no scientific basis on which to form any calculable probability whatever. We simply do not know.”
>
> — John Maynard Keynes, “The General Theory of Employment” (1937), p. 214.

Modern finance is technically magnificent and epistemically credulous.

The technical part is not in doubt. Calibration, hedging, optimisation and stress testing are real achievements, and they work precisely because nobody has to reopen the construction of the problem at every decision. But something is always settled before the valuation begins: which futures count as distinct, what evidence bears on them, which probabilistic model is adequate enough to use, and how much authority to give the current price. When those four choices are stable and widely shared, the machinery runs, and it runs extraordinarily well. That is exactly why the choices are easy to forget.

For long-dated assets exposed to structural change, the arrangement becomes difficult to defend. Climate transition, infrastructure exposed to contested policy, geopolitical fragmentation, technological obsolescence: each requires a commitment today to a future whose relevant features are themselves disputed. And the dispute is usually not about the arithmetic. Two analysts can agree on every number in front of them and still disagree about which mechanisms to represent, which relationships will carry forward, and which evidence deserves authority.

I did not arrive at epistemology by preference. I set out to build a valuation I could defend. Defending it required an account of the beliefs it rested on, and examining those beliefs required an account of how the problem had been posed in the first place. Epistemology arrived as a forced move.

Finance already has names for much of this difficulty. A scenario is a possible path. A stress test measures an exposure along it. Model uncertainty allows competing specifications. A market price gives the terms on which a claim trades. What none of them supplies is a way of comparing two serious accounts of the same financially consequential future — what could count as evidence between them, and what should follow when the comparison does not resolve.

I need a short name for “a serious account of the future”, and will use *probability picture*: a belief expressed as a probability law, or a probabilistic model that supplies one. In the Cox–Jaynes tradition, probabilities represent degrees of plausibility conditional on stated propositions and information, subject to demanding consistency requirements.[1] “Belief” here therefore means something much more disciplined than an opinion. But notice the order of operations. Probability theory can discipline a belief only after someone has decided what counts as an event and what counts as evidence. Those decisions come first, and the theory does not make them.

## Risk, Knightian uncertainty and radical uncertainty

> “There is a fundamental distinction between the reward for taking a known risk and that for assuming a risk whose value itself is not known.”
>
> — Frank H. Knight, *Risk, Uncertainty and Profit* (1921), p. 44.[2]

Three different things get called uncertainty, and the difference between them decides what kind of work a model can be asked to do.

**Risk**, in the standard sense, needs two things: outcomes described well enough for probabilities to have definite objects, and enough information about those outcomes for estimation and revision to mean something. Historical frequencies are one source of that information. Structural modelling, market observations and expert judgment are others. Given a reasonably stable description, expected utility, risk-neutral valuation and the familiar risk measures do useful work — and none of them requires anyone to know the true probabilities. Much of treasury practice, short-dated option trading and ordinary risk management lives here, in domains where evidence, convention and experience supply enough regularity to act on.

**Knightian uncertainty** is a difficulty inside an accepted description. We may know the relevant outcomes perfectly well and still have no defensible way to assign reliable probabilities to them. Ellsberg's comparison of bets with known and unknown probabilities makes the point sharply: an unchanged set of possible payoffs does not imply an unchanged decision problem. When Keynes wrote “We simply do not know”, he had in mind the prospect of a European war, or the rate of interest twenty years hence.[2] Finance meets related difficulties under other names — model risk, regime dependence, uncertain correlations. Caballero and Krishnamurthy give the point an explicitly financial form: in their model of a flight-to-quality episode, agents are uncertain how their own shocks relate to system-wide shocks, and each agent's individually conservative response leaves the economy collectively exposed.[3]

**Radical uncertainty** goes further: even the relevant outcomes, and the way they are organised, may be unsettled. A new technology, an institutional reaction or a political rupture can introduce a distinction that an established model never represented. A model of technological improvement may describe the incumbent technology with considerable sophistication and have no way at all to represent its displacement by another. Enlarging the family of models is then necessary — but the enlargement has to be chosen, and nothing in the old model guarantees that it supplies the right alternatives. Aydogan and co-authors draw the parallel distinction: uncertainty within a model, uncertainty among models, and uncertainty about whether the family contains an adequate model at all.[3] It is the third that concerns me here.

Scenarios are how the industry makes such questions tractable. They reduce an open future to conditional worlds that can be investigated, compared and revised, and their usefulness depends on the restriction they impose. Draw the family too narrowly and it excludes material possibilities. Draw it broadly enough that almost any decision can be defended and it stops discriminating between decisions at all.

That boundary is also institutional. Scientific assessments, central banks, regulators, accounting rules and market conventions between them help determine which observations and distinctions become usable in financial practice. A scenario need not exhaust the future to be useful. But neither its publication nor its inclusion in an official exercise supplies a probability that was absent from its construction.

Climate transition concentrates all three difficulties at once. Physical and engineering constraints coexist with political choices, technological change, and consequences that fall very unevenly across sectors and across the capital structure. For a long-lived commitment that is difficult to reverse, the two errors are not symmetric: underestimating transition risk can lock in an exposure before the repricing arrives, whereas overestimating it takes the more revisable form of an opportunity cost. Climate science, macroeconomic scenarios and financial evidence all constrain the problem, and none of them provides repeated observations of the complete transformation.[4] The practical task is to use that knowledge before the commitments have become irreversible, rather than to withhold judgment until the historical record has caught up with the question.

## Bayesian discipline

> “[Probability theory is] the optimal processing of incomplete information.”
>
> — Edwin T. Jaynes, *Probability Theory: The Logic of Science* (2003), p. xiii.[1]

The obvious objection to all of this is that models should face the data. They should. The objection only becomes interesting when you ask which claims the available observations are actually capable of testing.

George Frankfurter reports being told by the editor of a leading finance journal: “We in finance do not care much about philosophy. We care about data and what data can tell us.”[5] I have some sympathy for the impatience. But the remark skips a prior question. Before data can tell us anything about the decision in front of us, we have to establish what they measure, why the observations are comparable, and which conclusions the comparison warrants. In familiar settings those judgments can reasonably stay in the background. Under structural change they become part of the dispute. The editor has not dispensed with an epistemology. He has declined to examine the one he is using.

Plenty of evidence still bites. Historical defaults constrain a credit mechanism. Engineering rules out an impossible production path. An accounting identity exposes an investment scenario whose resources do not add up. None of this requires a completed climate transition, and all of it is worth doing.

What the record cannot supply is the repeated full experiment needed to validate every long-horizon implication of the model in the usual way. Asking a unique transformation to pass the evidential test of a recurring short-horizon process is asking the world for evidence it cannot produce — and then mistaking the impossibility for methodological virtue. Backtesting remains valuable wherever history is informative. It cannot warrant an extrapolation whose structural continuity it has not tested.

Tests have to be matched to the claims they support. A transition path that depends on an infeasible reallocation of labour or investment should fail its diagnostic even when its financial outputs look entirely familiar. A sound accounting identity, in the other direction, cannot establish the political likelihood of the policy path built around it. Rival specifications have to be examined, and the rules for revision fixed before the inconvenient observation arrives rather than after. That includes a distinction which is easy to lose: an error in a parameter is not the same thing as evidence that the proposed mechanism, or the whole family of models, is inadequate. Adding observations to the wrong exercise will not turn it into the right one.

Bayesian reasoning belongs to this larger practice, though the financial literature often invokes it in a much narrower sense. Give me a prior, a likelihood and a fixed family of hypotheses, and Bayes' rule determines exactly how the probabilities change when evidence arrives. It will also do that impeccably inside a model that omits the relevant possibility, treats an unsuitable data source as decisive, or owes its form to estimation convenience. The broader Bayesian project begins before the prior and continues after the posterior: what information should enter, which families deserve comparison, how their implications should be checked, and how to act when several pictures survive the check. Robust and ambiguity-sensitive methods contribute to that examination — but they too require reasons for the models and the departures they admit.[1,6]

Acting may require a single operative picture even when inference has not selected one uniquely. There are at least three ways to get one. You can average across a stated family. You can protect against its most adverse member. You can complete a partial description by maximum entropy, or by minimum relative entropy to a reference. These solve different decision problems and they need not agree.

Entropy-based completion is appropriate when the aim is to introduce as little unsupported structure as possible, relative to declared outcomes, constraints and a reference — formulating a prior, say, or completing an assessment once other evidence has been incorporated. What it contributes is a selection rule. The evidential basis remains the stated constraints and the reference, which is why naming the reference, and the assumptions made about dependence, is part of explaining what the principle has actually selected.[7]

Coherence has an organisational dimension too, and this is where it becomes uncomfortable in practice. An institution can be perfectly protected against a Dutch book — a combination of accepted bets that guarantees a loss — while running incompatible transition assumptions in disclosure, in investment and in risk management. Different purposes can justify different pictures. Departmental separation is not itself one of those justifications. Nor is revising a model in response to evidence the same thing as changing the rules of revision to accommodate an unwelcome result. The remedy is unglamorous: state which account governs which decision, and be able to defend its grounds when someone examines them again.[8]

“Since all models are wrong the scientist cannot obtain a ‘correct’ one by excessive elaboration,” wrote Box.[8] More parameters and more simulations examine a representation more thoroughly; they do not establish that it is adequate. A Bayesian analysis has to use the evidence as fully as it can within the models proposed, and at the same time examine where those models' assumptions came from: data, structural knowledge, institutional purpose, or a judgment nobody has resolved. This discipline reaches much further than updating. It is still not self-grounding.[8] Its limit is reached at the point where the available evidence and the applicable principles still permit more than one consequential representation.

That point is where the rest of this essay begins.

## The representational residue

> “My thesis, paradoxically, and a little provocatively, but nonetheless genuinely, is simply this: probability does not exist.”
>
> — Bruno de Finetti, *Theory of Probability* (1974), Preface.[9]

Why quote something so theatrical? Because probabilistic language encourages a tempting picture, and the theatre is the quickest way to break it open. The picture is this: once a model is coherent, carefully estimated and repeatedly revised, it becomes natural to speak as though there were a probability already sitting behind the evidence, waiting to be uncovered more accurately. De Finetti's own position is far stronger than anything I need — he rejected objective probability, not probability theory — but his provocation does the job. A probability is always a probability *of something*, conditional on some information, expressed in some representation of uncertainty. Those three ingredients have to be fixed before the calculus can operate at all.

The *representational residue* is what remains when logic, the available evidence and the applicable technical principles do not uniquely determine them. It can concern which states to distinguish, which features define similarity, which family of explanations to examine, or how to treat dependence. I want to be precise about the scope of the term: it names what remains genuinely unforced after the relevant discipline has done its work. It is not a licence to call every judgment a modeller makes a residue.[9]

Three independent arguments arrive at the same place.

**The first route is the representation of ignorance.** Bertrand's chord problem is the classic demonstration. Ask for the probability that a random chord of a circle is longer than the side of the inscribed equilateral triangle, and the answer depends on what “random” is taken to mean: pick two endpoints uniformly on the circumference and you get one third; pick a midpoint uniformly along a radius and you get one half; pick a midpoint uniformly inside the disc and you get one quarter. Same geometrical event, three defensible answers.

Finance encounters the same issue in an entirely ordinary place. An analyst with no view on a discount-rate gap represents that ignorance by spreading it uniformly. A colleague, equally without a view, spreads it uniformly over the associated valuation multiple instead. The set of possible valuations is identical. The probability weights on them are not. A change of coordinates that carries the law along with it would change nothing; choosing uniformity afresh in the new coordinates introduces a different law. Jaynes showed that a symmetry genuinely supplied by the problem can sometimes settle the choice. Where no such argument is available, “uninformative” is not an adequate description of what the analyst has assumed — it is a refusal to describe it.[1,10]

Similarity poses a related problem inside the same route. Goodman's “grue” and “bleen” show how descriptions that agree with every observation already made can imply different continuations; Watanabe shows how similarity judgments depend on the features a language makes available in the first place.[11] The financial version is mundane. One credit model groups firms by current industry. A second groups them by technological dependence. A third groups them by exposure to future policy. Two firms can be far apart under one classification and close under another, and the three models will not learn the same thing from the same default histories. Each classification can be perfectly coherent, and evidence can favour one over the others. Until it does, the classification remains one of the premises through which the data acquire predictive meaning at all.

**The second route concerns the problems a method is equipped to solve.** The no-free-lunch results deny any general advantage when methods are compared over unrestricted problem classes under the stipulated averaging assumptions.[12] The practical reading is that a successful method works because it exploits structure in the problems it actually encounters, so its record establishes competence within a domain. Take a credit model trained under gradual policy adjustment and apply it to an abrupt prohibition or a technological displacement, and a further structural judgment is required about which relationships survive the break. However impressive the record, the record cannot supply that judgment.

**The third route concerns the inputs to inference itself.** Cox–Jaynes consistency constrains probability assignments once the events or propositions at issue, and the information being conditioned on, have been specified — once, not before. Entropy-based selection likewise requires evidence constraints, a reference, and assumptions about how separate systems compose.[1,7] That last requirement is not a formality. If two sectors are independent, their information combines one way; if they share a policy exposure or a supply-chain dependence, the same marginal observations can support materially different joint losses. A rule can be uniquely justified for a stated inferential problem without selecting every feature of that problem for itself.[7]

None of this shows that all representations are equally defensible. Evidence can eliminate some. A symmetry can determine a measure. Stronger structural knowledge can settle an apparent ambiguity outright. What the three arguments share is narrower and more awkward: the success of a calculation within its premises does not establish that all of those premises were uniquely required. Enlarging the model family can improve the account without automatically settling the reasons for the enlargement. And the choice that remains is logical before it is institutional — a committee may have to make it, but the committee's need to decide is not what created the underdetermination.

Rationality does not supply the missing common starting point either. “It has become an article of faith among economists that differences in beliefs among rational individuals must be explained by different information,” writes Stephen Morris.[13] The results usually invoked for that faith are more conditional than the faith is. Aumann's agreement theorem depends on a common prior and common knowledge of the relevant posterior probabilities.[13] Blackwell and Dubins show that forecasts can merge as evidence accumulates when the forecasters' probability laws over complete future histories satisfy an absolute-continuity condition — roughly, when one does not rule out whole histories that the other still treats as possible.[13] Both conclusions inherit their assumptions. Rationality alone supplies neither a common starting point nor a timetable for agreement.

So continued disagreement is not, by itself, evidence of a residue. It calls first for the ordinary explanations: differences in information, differences in which histories each model permits at all, differences in updating, and plain error. Where those have been examined and the evidence still permits different consequential representations, the disagreement is not a failure of the inquiry. It is an outcome of it.

The residue also changes what institutions do with the resulting plurality, and this is where the consequences stop being methodological and start being financial. Comparing two probability pictures requires a purpose: a measure centred on ordinary predictive accuracy and one designed to give exceptional weight to tail events can rank the same disagreements differently. Selecting one picture for action then raises a second question, because averaging, protection against the adverse alternative, and entropic completion can produce different budgets and different capital requirements from the same inputs. The institution's mandate and its reasons have to determine which procedure it uses. Mathematics can establish what follows from the choice; but where the accepted premises leave the choice open, authority over it is part of the financial problem rather than a preliminary to it. It decides whose exposure appears in the assessment, which risk receives protection, and which consequences are left outside it.

## Prices and beliefs

At this point the market price looks like a way out of the analysts' disagreements. It is public, it is transactable, and it is disciplined by other people's capital — three things no spreadsheet can claim. Institutions need common prices to coordinate their positions, and a model claiming to value currently traded claims cannot simply ignore what they trade at. It is worth remembering that Bachelier began mathematical finance with conjectures about probability, not with a presumption that quotations disclosed the true law.[14] The difference between taking prices seriously and deferring to them matters most in exactly the case at issue here: when the price is observable and the reasons behind it are not.

Beliefs enter a price alongside wealth, risk bearing, endowments, funding conditions, mandates, hedging needs and horizons, and different combinations of these can sustain the same quotation. A deep order book establishes that a claim can be traded under prevailing conditions. It does not establish that the participants were able to express every relevant view, or that the marginal investor's horizon is anything like the horizon of the institution using the price. Even a sufficiently rich option surface reveals a valuation object — a state-price picture, under some extraction method — rather than a purified physical forecast.[14] State prices reflect both what people think will happen and how much a unit of money is worth to them when it does, which is why they cannot be read off directly as physical probabilities. And with finitely many liquid claims, the quotations can leave several valuation pictures compatible with them, so recovering one requires further restrictions or an explicitly stated selection rule.

This is not a merely hypothetical concern in climate finance. Stroebel and Wurgler surveyed 861 finance academics, practitioners and public-sector respondents, and found them at least twenty times more likely to say that markets underestimated climate risk than that they overestimated it.[15] The survey establishes widespread disagreement with prevailing pricing. It does not tell us whether the respondents were right, or why the gap arose. A model that reproduces market prices has established market consistency, which is a real property and a different one from the adequacy of the implied assessment for a long-horizon decision. Any discrepancy between physical probabilities and pricing weights still has to be interpreted through the valuation assumptions before anyone is entitled to call it mispricing.

> “The peculiar character of the problem of a rational economic order is determined precisely by the fact that the knowledge of the circumstances of which we must make use never exists in concentrated or integrated form, but solely as the dispersed bits of incomplete and frequently contradictory knowledge which all the separate individuals possess.”
>
> — Friedrich A. Hayek, “The Use of Knowledge in Society” (1945), p. 519.[14]

Hayek's account gives prices a substantial authority, but a different one from the authority usually claimed for them. They allow people with dispersed and incomplete knowledge to adjust their plans without requiring any one of them to understand the whole. That achievement depends on making coordination possible despite differences in knowledge. It does not turn the resulting price into a complete register of what is known. Grossman and Stiglitz locate a limit inside the economics of information itself: in their costly-information model, a price that revealed everything would remove the reward that sustains information acquisition in the first place.[16] Some knowledge therefore stays private for reasons internal to market equilibrium, not in spite of it.

The standard reply is that a well-founded objection would already have been traded upon. That reply assumes the disagreement can be expressed in a position the market permits.

*A mispricing sustained by a constraint that also binds you cannot be harvested by you.*

Short-sale bans, funding limits and performance-sensitive capital are the familiar cases, and Shleifer and Vishny worked through what they do to the arbitrageur.[17] But the principle is broader than any list of frictions. A financial system also determines which distinctions between probability pictures can be expressed at all — through admissible portfolios, contracts or hedges. If a more accurate belief differs from the prevailing one only along a dimension that no admissible position can load on, that accuracy is financially silent. The market can be efficient on the space it is allowed to trade and still have no selection mechanism whatsoever on the dimensions it excludes. The relevant failure is then not a distortion inside a market. It is a limit on what the market itself can express.

Prices also help determine the future against which their apparent prescience will later be judged. Merton's example is the solvent bank destroyed by withdrawals prompted by a rumour of insolvency. The everyday version is slower: financing conditions can prolong a technology, accelerate its deployment, or create a constituency resistant to its replacement, and restrictive finance can weaken the very activity whose prospects the price purported to assess. MacKenzie's *An Engine, Not a Camera* is the standard reference for this performative possibility.[18] Whatever the later evidence looks like, it bears some imprint of the earlier beliefs and valuations.

## Disagreement in financial decisions

None of this requires a new security. The analysis already has financial uses inside an institution as it stands.

An institution may discover that its own portfolio is difficult to reconcile with the transition assumptions it publishes, or that two of its scenario programmes imply incompatible labour, investment and default paths. That is a real diagnostic, and it establishes a material discrepancy without anyone having to put a price on it. Putting a price on it — a *premium wedge* — requires a further translation: the competing pictures must be used to value the same financial claim. Even then, the prices at which each side would individually be willing to trade, their reservation values, are distinct from the price at which a transaction might actually occur.

An investor may also express a view through existing assets, through underwriting or through a hedge. A relative-value position can rest on a perfectly well-founded epistemic thesis and still lose money, and still be exposed to risks that have nothing to do with the disagreement that motivated it. Arbitrage requires the much stronger case of claims whose quoted terms can be combined to guarantee a gain. The usefulness of better reasoning is not confined to that case, just as it is not contingent on anyone creating a market dedicated to disagreement. It can improve ordinary investment and risk decisions while making the grounds of those decisions explicit.

The distinctive question for a contract written on a disagreement is whether the comparison itself can be specified publicly. A counterparty may declare its own probability picture; alternatively, a comparator may be obtained from conventional markets under a stated extraction method. The participant's decision determines which aspect of the difference matters. The settlement observation determines which part of it can be tested. The source, timing and treatment of revisions all have to be fixed before the evidence arrives. And where a public observation fails to distinguish an important part of the dispute, that part simply stays outside the contract: pricing the observable component leaves the rest with the parties.

Such a contract could support either a position on a view or protection against the outcomes on which that view performs badly. What it would add is the public specification and administration of the comparison, rather than an intrinsically unreplicable cash flow — sufficiently complete state-contingent markets could reproduce the payment once its terms were known. Whether standardising it would attract genuine demand is a separate empirical question. In either case an exchange can decide whether a declaration supports the agreed settlement; it cannot certify the quality of a participant's entire account of the future. A dedicated market would not create responsibility for the underlying representation. The institution already carries that responsibility the moment it chooses a representation for a decision.[19]

## Conclusion

> “The recognition of the insuperable limits to his knowledge ought indeed to teach the student of society a lesson of humility.”
>
> — Friedrich A. Hayek, “The Pretence of Knowledge”, Nobel Memorial Lecture (1974), excerpt.[20]

When evidence and accepted principles leave more than one consequential probability picture standing, finance is in an awkward position. It cannot demand certainty from a forward-looking model while accepting the assumptions of current practice without examination. Both organise an unsettled future. Both owe an account of the evidence and the conventions they rely on. A rigorous inquiry may reject many representations, justify one for a particular use, and still leave consequential alternatives unresolved — and when it does, the disagreement that remains belongs to the analysis rather than counting against it. A price can coordinate a transaction in its presence. That accomplishment does not relieve an institution of judging the beliefs on which its decisions depend.

The obligations that follow are concrete. An institution should state the picture that governs the decision, explain which constraints support it, distinguish a deliberate selection from an empirical finding, and retain the material alternatives that have not been refuted. It can then identify which consequences are robust, which depend on an unresolved assumption, and what evidence would justify revision. Where the choice determines a valuation, a capital requirement, or whose losses enter a stress test, the reasons for it are part of financial accountability. Adopting the conventional picture without comment is not an escape from this; convention is one of the choices under examination.

Climate transition makes the stakes particularly clear, but the argument extends to every consequential commitment whose future the available record cannot uniquely determine. The practical task is to make the probability pictures explicit, isolate the disagreement that actually matters, establish what evidence could test it, and give it an appropriate financial consequence while keeping the unresolved part visible.

Hayek's closing appeal to humility was a warning against turning limited knowledge into a warrant for far-reaching control. In finance the same discipline requires that the authority claimed for a model, a price or a contract stay commensurate with what it can actually establish. Finance can coordinate under uncertainty while saying clearly what its models assume, what its evidence supports, what its contracts can observe, and what remains a matter of judgment. Carveth Read's standard remains apt: “It is better to be vaguely right than exactly wrong.”[20] For a financial system facing risks on a planetary scale, that is the difference between coordination disguised as knowledge and knowledge that has earned the right to coordinate.

## References

[1] Richard T. Cox, “Probability, Frequency and Reasonable Expectation”, *American Journal of Physics* 14, 1–13 (1946); Edwin T. Jaynes, *Probability Theory: The Logic of Science* (2003).

[2] Frank H. Knight, *Risk, Uncertainty and Profit* (1921); Daniel Ellsberg, “Risk, Ambiguity, and the Savage Axioms”, *The Quarterly Journal of Economics* 75, 643–669 (1961); John Maynard Keynes, “The General Theory of Employment”, *The Quarterly Journal of Economics* 51, 209–223 (1937), quotation p. 214.

[3] Ricardo J. Caballero and Arvind Krishnamurthy, “Collective Risk Management in a Flight to Quality Episode”, *The Journal of Finance* 63, 2195–2230 (2008); Ilke Aydogan, Loïc Berger, Valentina Bosetti and Ning Liu, “Three Layers of Uncertainty”, *Journal of the European Economic Association* 21, 2209–2236 (2023); John Kay and Mervyn King, *Radical Uncertainty* (2020); Francis X. Diebold, Neil A. Doherty and Richard J. Herring, eds., *The Known, the Unknown, and the Unknowable in Financial Risk Management* (2010).

[4] Emanuele Campiglio, Louis Daumas, Pierre Monnin and Adrian von Jagow, “Climate-Related Risks in Financial Assets”, *Journal of Economic Surveys* 37, 950–992 (2023); Stefano Giglio, Bryan Kelly and Johannes Stroebel, “Climate Finance”, *Annual Review of Financial Economics* 13, 15–36 (2021); Riccardo Rebonato, “Asleep at the Wheel? The Risk of Sudden Price Adjustments for Climate Risk”, *The Journal of Portfolio Management* 50(2), 48–63 (2023); Tristan Jourde and Quentin Moreau, *Systemic Climate Risk*, Banque de France (2025).

[5] George M. Frankfurter, review of John H. Cochrane's *Asset Pricing*, revised edition, *Journal of Economic Behavior & Organization* 60, 603–608 (2006).

[6] Itzhak Gilboa and David Schmeidler, “Maxmin Expected Utility with Non-Unique Prior” (1989); Fabio Maccheroni, Massimo Marinacci and Aldo Rustichini, “Ambiguity Aversion, Robustness, and the Variational Representation of Preferences” (2006); Lars Peter Hansen and Thomas J. Sargent, *Robustness* (2008) and “Structured Ambiguity and Model Misspecification” (2022).

[7] Edwin T. Jaynes, “Information Theory and Statistical Mechanics”, *Physical Review* 106, 620–630 (1957); John E. Shore and Rodney W. Johnson, “Axiomatic Derivation of the Principle of Maximum Entropy and the Principle of Minimum Cross-Entropy”, *IEEE Transactions on Information Theory* 26, 26–37 (1980); Constantino Tsallis, “Conceptual Inadequacy of the Shore and Johnson Axioms for Wide Classes of Complex Systems”, *Entropy* 17, 2853–2861 (2015).

[8] Brian Skyrms, *Causal Necessity* (1980); George E. P. Box, “Science and Statistics”, *Journal of the American Statistical Association* 71, 791–799 (1976), quotation p. 792; Persi Diaconis and David Freedman, “On the Consistency of Bayes Estimates”, *The Annals of Statistics* 14, 1–26 (1986).

[9] Bruno de Finetti, *Theory of Probability* (1974), Preface.

[10] Joseph Bertrand, *Calcul des probabilités* (1889); Edwin T. Jaynes, *Probability Theory: The Logic of Science* (2003).

[11] Nelson Goodman, *Fact, Fiction, and Forecast* (1955); Satosi Watanabe, *Knowing and Guessing* (1969).

[12] David H. Wolpert, “The Lack of A Priori Distinctions Between Learning Algorithms”, *Neural Computation* 8, 1341–1390 (1996); David H. Wolpert and William G. Macready, “No Free Lunch Theorems for Optimization”, *IEEE Transactions on Evolutionary Computation* 1, 67–82 (1997).

[13] Stephen Morris, “The Common Prior Assumption in Economic Theory”, *Economics and Philosophy* 11, 227–253 (1995), quotation p. 227; Robert J. Aumann, “Agreeing to Disagree”, *The Annals of Statistics* 4, 1236–1239 (1976); David Blackwell and Lester Dubins, “Merging of Opinions with Increasing Information”, *The Annals of Mathematical Statistics* 33, 882–886 (1962).

[14] Louis Bachelier, *Théorie de la spéculation* (1900); Friedrich A. Hayek, “The Use of Knowledge in Society”, *The American Economic Review* 35, 519–530 (1945); Douglas T. Breeden and Robert H. Litzenberger, “Prices of State-Contingent Claims Implicit in Option Prices”, *The Journal of Business* 51, 621–651 (1978).

[15] Johannes Stroebel and Jeffrey Wurgler, “What Do You Think about Climate Finance?”, *Journal of Financial Economics* 142, 487–498 (2021).

[16] Sanford J. Grossman and Joseph E. Stiglitz, “On the Impossibility of Informationally Efficient Markets”, *The American Economic Review* 70, 393–408 (1980).

[17] Andrei Shleifer and Robert W. Vishny, “The Limits of Arbitrage”, *The Journal of Finance* 52, 35–55 (1997).

[18] Robert K. Merton, “The Self-Fulfilling Prophecy”, *The Antioch Review* 8, 193–210 (1948); Donald MacKenzie, *An Engine, Not a Camera: How Financial Models Shape Markets* (2006).

[19] Kenneth J. Arrow, “Le rôle des valeurs boursières pour la répartition la meilleure des risques” (1953); Gérard Debreu, *Theory of Value* (1959).

[20] Friedrich A. Hayek, “The Pretence of Knowledge”, Nobel Memorial Lecture (1974); Carveth Read, *Logic: Deductive and Inductive*, 4th edition (1920).
