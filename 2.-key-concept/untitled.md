# Chapter 4: Potential sources of Bias

A statistic/estimated parameter is **biased** if it is calculated in such a way that is systematically different from the population parameter of interest.

* Parameter estimate systematically under/over-estimated
* p-value/type I error systematically under/over-estimated \(e.g. due to poor adjustment for multiplicity\)
* CI with CI level systematically below or above the target

## 4.1 Placebo effect and Blinding

Advantages:

* The blinding permits to avoid the placebo effect.\(conscious or subconscious influence\)
* The blinding allows to do a fair evaluation of outcomes.

Disadvantages:

* before enrolling a subject as knowing the next treatment to allocate may induce a **patient selection** according to the treatment ——Non deterministic randomization after eligibility has been established including informed consents prevents such bias.在确定合格性之后，包括知情同意在内的非确定性的随机化可以防止这种偏差。
* during treatment as knowing the treatment received may impact on a subjective assessment of the treatment effect by the patient or by the investigator ——Blinding prevents such bias. Blinding becomes less critical as the endpoint becomes objective such as temperature, amount of antigen in blood shortly after treatment. 蒙蔽可以防止这种偏见。在治疗后不久，由于终点变得客观，如温度、血液中抗原的数量，致盲变得不那么重要。

## 4.2 multiplicity poorly adjusted

Note that the absence of pre-specified analysis before conducting an analysis opens the door to multiplicity issue. Indeed had a pre-specification happens the analysis might have been different, considering different scenarios requiring adjustment of nominal type I error. Accordingly value of data driven analyses is limited to hypothesis generation.

请注意，在进行分析之前缺少预先指定的分析为多重性问题打开了大门。实际上，如果有一个预先规范，考虑到需要调整标称类型I错误的不同场景，分析可能会有所不同。因此，数据驱动分析的价值仅限于产生假设。

## 4.3 Compliance

### Definition

The compliance is the extent to which a person’s behaviour coincides treatment assignment or specification. Compliance and adherence are often used interchangeably.

### Main reasons that lead to lack of compliance

* Toxicity or side effects
* Lack of effect
* Involving life style/behavior change
* Complex or inconvenient interventions
* Insufficient or lack of understanding instructions
* Change of mind, refusal
* Lack of family support
* Lack of quality control

### Impact on a superiority trial

![](../.gitbook/assets/image%20%2818%29.png)

In superiority trials the **full analysis set is used** in the primary analysis \(apart from exceptional circumstances\) because it tends to **avoid over-optimistic estimates of efficacy** resulting from a per protocol analysis, since the non-compliers included in the full analysis set will generally diminish the estimated treatment effect.  
——在优势试验中，全分析集（full analysis set）被使用在主要分析中\(除特殊情况\),因为它往往会避免过于乐观估计药效，因为不服从者包含在在完整的分析集中，通常会减少估计的治疗效果。

### Impact on a non-inferiority trial

Poor compliance raises questions about the study validity in non-inferiority/equivalence studies. Analysis involving compliant subjects to be important in non-inferiority/equivalence objectives——涉及顺从受试者的分析在非劣效/等价目标中是重要的。

However, in an equivalence or non-inferiority trial use of the full analysis set is generally not conservative and its role should be considered very carefully.--然而，在等价性或非劣效性试验中，使用完整的分析集通常是不保守的，应该仔细考虑它的作用。

### How to improve the compliance in a study?

* Include quality control
* Keep the intervention as simple as possible.
* Choose motivated participants. Don’t drag people into the trial.
* **Run-in period**  
  – Helpful in stabilizing potential participants and wash-out pretreatment medications

  – Example: Blood sample pre-vaccination

* A truly informed participant appears to be a better adherer.
* On study reinforcement: by phone calls, mailed reminders, clinical visits, etc

### Indicators of compliance

Percent compliance in drug intake  
——% compliance = \# of pills taken / \# of pills should have been taken per protocol

Percent deviations  
——% of subjects with major protocol deviations

## 4.4 Missing Data

Missing data is recognised as a **critical source of bias**. This seriously jeopardizes the credibility of study result

There are difference source of missingness: treatment side effect, inefficacy, efficacy or other reason such as loss of follow-up. Not accounting for the missing data at week 12 would represent a substantial bias in the analysis.——缺失有不同的来源:治疗的副作用、无效、疗效或其他原因如失访。如果不考虑第12周丢失的数据，那么在分析中就会出现很大的偏差。

### Missing completely at random \(MCAR\)

If the probability of an observation being missing does not depend on observed or unobserved measurements then the missing observation is classified as MCAR.

Example, a subject has moved to another city for non-study reasons, then the subject would be considered as drop-out of a study. This subject’s data may be considered as MCAR because dropout was not in any way related to the endpoint of interest——例如，一名受试者因非研究原因搬到另一个城市，那么该受试者将被视为退出。该受试者的数据可以被视为MCAR，**因为退出与研究的endpoint没有任何关系**

In the MCAR situation, the analysis based on data available is unbiased. The MCAR situation is infrequent.——在MCAR的情况下，基于现有数据的分析是无偏的。MCAR的情况并不常见。

### Missing at random \(MAR\)

MAR corresponds to the situation where the missingness depends on the observed outcomes. In this case, whether or not a result is missing has nothing to do with the missing value itself but this is related to the values of observed results.——MAR对应的情况是，失踪取决于观察到的结果。在这种情况下，一个结果是否丢失与丢失的值本身无关，但是这与观察到的结果的值有关。

An example of MAR data could be an instance in which a subject had low antibody titre at a previous visit which led to revaccination \(rescue vaccination\). Thereafter the subject dropped out as the subject could not contribute to persistence of initial vaccination. In this case, missing data at future visits depends on the results observed previously.——MAR数据的一个例子可能是，一个受试者在上次来访时抗体滴度较低，导致再次接种\(救援接种\)。此后，该受试者退出，因为该受试者无法持续最初的疫苗接种（因为接种了两次）。在这种情况下，在未来的访问中丢失的数据取决于以前观察到的结果。

characteristics：

* missing does not depends on unobserved values
* In the MAR situation, statistical analyses should use the data available from the subjects to infer and account on the missing data \(e.g. repeated measurement methods such as GEE, MIXED, NLmixed; survival method\).——在MAR情况下，统计分析应使用从受试者那里可获得的数据来推断和解释缺失的数据\(举例：重复测量方法，如GEE、MIXED、NLmixed;生存方法\)。

### Missing not at random \(MNAR\)

The last scenario covers all other situations in which the missingness also depends on the unobserved outcomes.

An example of MNAR data could be a subject for which the observed immunological results were indicative of protection up to the occurrence of the illness of interest \(vaccine failure\). Thereafter the subject dropped out as the subject could not contribute to persistence of initial vaccination. In this case, missing data at future visits depend on an unobserved titre that was too low to protect the subject——MNAR数据的一个例子是，观察到的免疫学结果表明，在发生相关疾病\(疫苗失败\)之前，其可以起到保护作用。此后，该受试者退出，因为该受试者无法持续最初的疫苗接种（因为疫苗已经失效了）。在这种情况下，在未来的访问中丢失的数据取决于未观察到的不足以保护受试者的低滴度。

Analysis based on data available is biased

### Classification

In most cases it is difficult to work out whether the relationship between the missing value and the unobserved outcome is completely absent.——在大多数情况下，很难确定缺失值和未观察到的结果之间的关系是否完全不存在。

Available methods：

* Plan to limit missingness \(eg HAM-D every 4 weeks, query\)
* Evaluate comparability between groups with respect to missingness
* Investigate reason for missingness
* Evaluate impact of missingness trough sensitivity analysis for missingness that may not be at random  
  ——–using Complete case analysis \(drop incomplete case\)

  ——Last value carried forward

  ——**Imputation based on available data \(depending on type of variable use of mixed model, time to event specific methods, …\)**

  ——Imputation based on reason for missingness

### Multiple Imputation technique

Multiple imputation techniques\(估算技术\) are now available in standard statistical software \(e.g. SAS proc MI & proc MIANALYSIS\) allowing assessing impact of missing data.

#### principle

* Step 1: to generate N set of data in which missing data has been imputed based on an informative random mechanism——根据信息性随机机制，生成N组数据，其中缺失数据已被输入
* Step 2: to estimate the parameter of interest and its variance for each set of data——估计每组数据的相关参数及其方差
* Step 3: to obtain the final estimate as the mean of estimates over the set of data and to obtain its variance as the mean of variance + \(the variance between the estimates\).——获得最终估计值作为一组数据的估计值的平均值，并获得其方差作为方差的平均值+\(估计值之间的方差\)。

#### illustration

![](../.gitbook/assets/image%20%2876%29.png)

![](../.gitbook/assets/image%20%2836%29.png)

The graph illustrates the bias correction after Imputation of missing data while accounting for the relationship between X & E:

* Complete case: the 95% CI for the expected mean has a coverage below 40% due to the bias in the estimate.
* Replacing missing data by a single imputed value rectifies the bias but variance is underestimated leading to a CI with coverage below expectation.
* Multiple imputation rectifies the bias and allows a proper variance estimation leading to a CI with expected coverage.

## 4.5 Confounding factor

A confounding factor is a factor that is associated to the outcome and is not equally represented in the compared groups.

### Example 1

An example is provided below with smoking habit being confounding factor in the assessment of a treatment for lung cancer

* Associated to endpoint: smoking increases risk of cancer
* not equally represented in the compared groups

![](../.gitbook/assets/image%20%2867%29.png)

Confounding factor is the main drawback of non-randomized clinical trials. When these are known, **an analysis stratified** for this allows obtaining an unbiased estimate. Unfortunately these are usually unknown and the best way to prevent bias related to confounding factor is to use a randomization study design.

### Example 2

You may also have confounding factors in Randomized Clinical Trial \(RCT\) but these are less frequent as the randomization allows to assume each group has the same profile regarding the prognostic factors.——在随机临床试验\(RCT\)中，也可能存在混杂因素，但这些因素的发生频率较低，因为随机化允许假定每个组在预后因素方面具有相同的概况。

![](../.gitbook/assets/image%20%2843%29.png)

Another example is the analysis of a study involving 2 randomization steps that would not take into account the structure of the design. Comparing treatment B to treatment A without accounting for the enrolment waves will lead to the same confounding factor as non-randomized study.——另一个例子是对一项涉及两个随机步骤的研究的分析，该研究不考虑设计的结构。在不考虑录入比例的情况下比较治疗B和治疗A，将导致与非随机研究相同的混杂因素。

Option 1 : use all subjects  
Last 200 subjects in treatment C may be associated to confounding factor \(eg center effect\) since there was no randomization between A and C.

Option 2 : use first 300 subjects in treatment A & C——Less subjects but no risk of confounding factor

## 4.6 Model assumption

### Asymptotic normal assumptions

![](../.gitbook/assets/image%20%2891%29.png)

In the simulation presented below data based on known parameters \(incidence rate identical in 2 groups in the example below\) were generated repeatedly to investigate the performance of using an asymptotic p-value assumption below 2.5% to rule out the null hypothesis that the 2 groups are identical. Would the decision strategy properly control the type I error, the proportion of simulated data in which the null hypothesis is rejected would be below 2.5%. The simulations shows that the strategy based on an asymptotic p-value is associated to a type I error above 2.5%. The simulations also present the performance of using an exact p-value which properly control the type I error below 2.5% but may be conservative as the true type I error can be much lower than 2.5%.——在下面的仿真中，根据已知参数\(下例中两组的发病率相同\)反复生成数据，以考察使用小于2.5%的渐近p值假设来排除两组相同的原假设的性能。如果决策策略正确地控制了类型I的错误，那么拒绝原假设的模拟数据所占的比例将低于2.5%。仿真结果表明，基于渐近p值的策略与大于2.5%的I型误差相关。仿真结果还表明，使用精确的p值可以将I型误差控制在2.5%以下，但也可能是保守的，因为真正的I型误差可能远远低于2.5%

{% hint style="info" %}
Asymptotic methods are known for not controlling the type I error. While exact methods do, these methods are conservative.——众所周知，渐近方法不能控制I型误差。虽然精确的方法可以，但是这些方法是保守的。
{% endhint %}

### Other assumptions

It is important to be aware of the assumption underlying the analysis method used and the robustness of the method in case there are deviations from these assumptions.——重要的是要了解所使用的分析方法背后的假设，以及该方法在出现偏离这些假设的情况下的稳健性。

For instance, a t-test to compare two means from continuous variables is known to be robust to normality assumption with sample size above 30. However the power of a t-test based on common variance in the 2 groups compared is substantially impair by deviation from the assumption of common variance as illustrated below.——例如，用t检验来比较来自连续变量的两个平均值对样本容量大于30的正态性假设是稳健的。然而，基于两组的共同方差的t检验的效力，会因为下面所示的共同方差假设的偏差而大大削弱。

![](../.gitbook/assets/image%20%2868%29.png)

Likewise a proportional hazard model will provide low power in case of departure from the proportionality assumption.——同样地，比例风险模型在偏离比例假设的情况下将提供低功率。

### Robustness of analysis to model assumptions

Exact and non-parametric approaches are assumption free methods with good control of type I error. However these methods are conservative i.e. the true type I error may be substantially below the targeted type I error, thereby impacting negatively on the power.——精确法和非参数法是无假设的方法，具有良好的控制I型误差的能力。然而，这些方法是保守的，即真正的I型误差可能大大低于目标I型误差，从而对功率产生负面影响。

**Check assumption**——Whenever a primary analysis method relies on model assumption it is important to ensure these assumptions are valid.  

**Perform sensitivity analysis using less stringent method——**Robustness assessment is also named sensitivity analysis.  
       ①  Semi parametric method \(eg logrank\)  
       ②  Non parametric \(eg permutation test\)

### Assumption free method – sampling methods\(permutation test\)

Sampling methods such as bootstrap/Jacknife, permutation test are exact **non-parametric method** using the **distribution of observed data**. 

Permutation test is a non-parametric approach to **test H0: superiority between groups**

Basic principle:

* Under the null hypothesis, data from all groups come from the same distribution
* The distribution of the test statistic, such as mean difference, can be obtained from all possible data permutation.

#### Example 1 \(2 groups with 3 observations\):         Group A: 20,23,30            Group B: 10,15,18

Interested in testing if the mean of the group A is superior to the mean of group B. T-test is not appropriate, given the sample size.

If the group means are truly equal, then shifting the group labels will not have a big impact the sum of values observed in each group \(or mean with equal sample sizes\). Group difference will be null, positive or negative.

![](../.gitbook/assets/image%20%2889%29.png)

There are 6!=720 permutations considering all 6 positions as unique. Out of the 720 permutations, there are 20 unique combinations \(equal sample sizes\). The observed difference was the largest, leading to a p-value of 1/20.

#### Example 2 \(2 groups with 80 observations\):  Group 1: 61 responders / 80     Group 2: 45 responders / 80

Looking at all possible permutations may become difficult =&gt; **a random selection of permutation can be used**

Permutation test on difference in responder rate gives a p-value=0.012

T-test gives a p-value=0.007

## 4.7 statistical versus clinical significance

One of the most frequent pitfalls when interpreting the clinical trial results is to focus on p-value. Parameter estimates and confidence interval are more important than p-value, as these provide clinical insight of an effect. ——**在解释临床试验结果时，最常见的陷阱之一是关注p值。参数估计和置信区间比p值更重要，因为这些提供了临床效果的洞察力**

**P-values are also depending on parameterization** as shown in the example of a logistic regression on the effect of different covariables on seroprotection rate.

![](../.gitbook/assets/image%20%2835%29.png)

Odd ratio is in the same range for the treatment group \(binary variable\) and for BMI and Age \(continuous variables\) even though p-values are different. Having a lower power \(larger p-value\) for a binary effect is expected as binary covariable contains less information than a continuous covariable.

![](../.gitbook/assets/image%20%2858%29.png)

Now looking at the summary by age and BMI, it appears that although age and BMI are ‘statistically similar’ they cover different clinical relevance because age is covering a larger range \(larger SD i.e. Standard Deviation\) and thereby the effect is clinically more important than BMI.——现在看一下年龄和BMI的总结，虽然年龄和BMI在统计学上是相似的，但它们涵盖了不同的临床相关性，因为年龄覆盖的范围更大\(更大的SD，即标准差\)，因此其临床效果比BMI更重要。

## 4.8 [publication bias](https://en.wikipedia.org/wiki/Publication_bias)

Publication bias is a bias with regard to what is likely to be published, among what is available to be published. It has been observed that there is a tendency of researchers, editors, and pharmaceutical companies to handle the reporting of experimental results that are positive \(i.e. showing a significant finding\) differently from results that are negative \(i.e. supporting the null hypothesis\) or inconclusive, leading to a misleading bias in the overall published literature.——发表偏倚是指在更大可能发表和可以发表的内容之间存在的偏倚。已经注意到一种倾向，即研究,编辑,和制药公司处理报告的实验结果是积极的\(即显示出重大的发现\)不同于消极的结果\(即支持零假设\)或不确定，这种倾向导致了在整个文学出版的误导偏倚

Level of evidence of a \(published\) study result:

* Blinded, Randomized, pre-specified analysis, high compliance, robust results
* Randomized, pre-specified analysis, high compliance, robust results
* Non-Randomized, pre-specified analysis, high compliance, robust results
* All other

Statistical methods have been developed to detect publication bias and to perform a bias adjustment. This consists into a scatter plot of the estimated effect in a normalized scale versus the sample size or standard error of the effect. Without publication bias it is expected that the plot display a symmetric triangle.——已经发展了统计方法来检测发表偏倚并进行偏倚调整。这包括归一化尺度下的估计效果与样本大小或效果的标准误差的散点图。在没有发表偏倚的情况下，期望图显示一个对称三角形。

![](../.gitbook/assets/image%20%2834%29.png)

