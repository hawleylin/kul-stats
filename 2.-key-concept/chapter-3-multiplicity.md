# Chapter 3: Multiplicity

## 3.1 Introduction

The **simplest** confirmatory study involves a single confirmatory objective involving **a single null hypothesis/primary endpoint/analysis** but such a trial is infrequent. Multiplicity occurs when there are multiple confirmatory objectives, null hypotheses, endpoints, methods or multiple analyses

Multiplicity can be categorized into two different types:

| Type OR | Type AND |
| :--- | :--- |
| HA: at least one of condition 1 **OR** condition 2 **OR** … is met | HA: condition 1 **AND** condition 2 **AND** … are met simultaneously |
| H0: condition 1 AND condition 2 AND … are met simultaneously | H0: At least one of condition 1 OR condition 2 OR … is met |

### Alternative hypothesis expressed with OR

In the Accutane example, aiming to show **difference** in relative risk translates to **H0: RR=1**. This can be seen as testing **H01: RR ≥ 1 AND H02: RR ≤ 1** with for instance the following alternative hypothesis **Ha1: RR = 2.5 OR Ha2: RR = 1/2.5.**

![Illustration of type I error impact for testing difference](../.gitbook/assets/image%20%285%29.png)

for testing each null hypothesis H01 and H02, the nominal type I error is $$\alpha$$   
the type I error for testing H01: RR ≥ 1 AND H02: RR ≤ 1 is $$2*\alpha$$

换句话说，under the hypothesis H0: RR=1, there is 2\*α risk to observe a value in the red area and there are 2α risk that the 2 sided \(1-2\*α\) confidence interval \(CI\) is outside the H0 area

{% hint style="info" %}
The type I error is above the maximum of nominal type I error of each individual null hypothesis while it is below the sum of nominal type I error.  
总的I 型错误大于每个nominal，小于nominal的总和

adjustment of type I used for each individual hypothesis testing is needed  
                                               ![](../.gitbook/assets/image%20%2812%29.png) 
{% endhint %}

![Illustration of type II error impact for testing difference](../.gitbook/assets/image%20%2848%29.png)

On the other hand, if the nominal type II error for testing H02 RR ≤ 1 is β, the type II error impact for testing H0: RR=1 is slightly below β.

{% hint style="info" %}
Type II is below the min of all nominal type II errors. --第II类误差小于每个零假设的小名义第II类误差
{% endhint %}

### Alternative hypothesis expressed with AND

In the Accutane example, aiming to show **equivalence** corresponds to testing **H01: log\(RR\) ≥ δ1 OR H02: log\(RR\) ≤ -δ2**  under , for instance, the alternative hypothesis that **Ha: RR = 1** 

![Illustration of type I error impact for testing equivalence](../.gitbook/assets/image%20%2846%29.png)

For testing each null hypothesis **H01 and H02**, the **nominal type I error is α**, as illustrated for **H02 log\(RR\) ≤-δ2** , then the **type I error** for testing **log\(RR\) ≥ δ1 OR H02: log\(RR\) ≤ -δ2** is **below α** 

because under the hypothesis **log\(RR\) ≥ δ1 OR H02: log\(RR\) ≤ -δ2** , there is less than α risk to observe a value in the red area and there are less than alpha risk that the 2 sided \(1-2\*α\) CI is outside the H0 area.

{% hint style="info" %}
The type I error is below the maximum of nominal type I errors of each individual null hypothesis.
{% endhint %}

![Illustration of type II error impact for testing equivalence](../.gitbook/assets/image%20%2838%29.png)

On the other hand if, the nominal type II error for each H01 and H02 hypothesis is β under the alternative that RR=1, the type II error testing **log\(RR\) ≥ δ1 OR H02: log\(RR\) ≤ -δ2** is **between β and 2\*β**.

{% hint style="info" %}
The type II error is above the maximum of nominal type II error of each individual null hypothesis while it is below the sum of nominal type II errors.

                                           ![](../.gitbook/assets/image%20%2866%29.png) 
{% endhint %}

### Examples

Type 1 \(OR\) multiplicity issues typically arise when:

* Comparing treatments within many subgroups 
* Analyzing multiple parameter endpoints 
* Analyzing the same parameter at multiple time points 
* Conducting **interim analyses**
* Comparisons between pairs of treatments when more than two treatments are being compared \(multiple comparisons\)

Type 2 \(AND\) multiplicity issues typically arise when:

* Showing equivalence with respect to multiple parameters
* Showing safety and efficacy
* Showing efficacy against multiple diseases

### Impact of multiplicity if not controlled

![](../.gitbook/assets/image%20%2821%29.png)

### Guidelines for confirmatory multiple objectives

Multiplicity needs to be addressed and we have formal guidance to indicate this: CPMP PtC and ICH E9

* « only… analyses envisaged in the protocol can be considered confirmatory »
* « \[for confirmatory trials\] each trial should address a limited number of questions »
* « make a clear distinction between confirmatory \[and\] exploratory analyses »

Multiplicity can be reduced by:

* Reducing the number of variables
* Using composite endpoints（注意：如果使用了multiple method，但只有一个endpoint的话，会产生multiplicity）
* Using summary statistics, …

If multiplicity still persists:

* « \[the analysis\] may necessitate adjustment of the type I error »
* « adjustment should always be considered and the details of any adjustment or … why adjustment is not thought necessary \[should be\] in the analysis plan »
* Note that this even applies to secondary endpoints which may become the basis for additional claims.

## 3.2 Techniques

![](../.gitbook/assets/image%20%2823%29.png)

### Non alpha adjustment techniques

Prioritize a priori to be able to conclude on a maximum of sub-objectives

* Test objective \#1 at global alpha level
* If significant, test objective \#2 at global alpha level
* If significant, test objective \#3 at global alpha level ......如果不显著，测试终止，不可继续

Take into account data structure

* Test dose effect in a dose-range study
* Test global effect in a factorial design

Combine endpoints

### Alpha adjustment techniques \(for OR type\)

#### Bonferroni

![](../.gitbook/assets/image%20%2892%29.png)

Advantages：simple and general

Disadvantages: This approach can be conservative since the type I error is below α

> As first example, if the null hypotheses are independent and α/N is used as nominal Type I error, the Type I error is actually  $$\boxed{[1-(1-\dfrac{\alpha}{N})^N]}$$ , This means that for N=100, α is actually 4.88% when the aim is to control this to be below 5%
>
> Note : Type I error=probability to reject H0 when H0 is true = 1- probability to not reject H0 when H0 is true= 1- sum\(probability to not reject H0i when H0 is true\) = $$\boxed{[1-(1-\dfrac{\alpha}{N})^N]}$$ 
>
> As second example, if the null hypotheses are strongly correlated and α/N is used, the Type I error will be close to α/N which is substantially below α

#### Holm

![](../.gitbook/assets/image%20%2880%29.png)

Advantages： simple，general and more powerful than Bonferroni

Disadvantages:

* Stochastic dependencies between the test statistics not taken into account
* No simple and obvious equivalence with simultaneous confidence intervals \(applies to all sequential methods\)

#### Hochberg

![](../.gitbook/assets/image%20%2878%29.png)

Advantages： simple，general and more powerful than Bonferroni and Horm

Disadvantages:

* Stochastic dependencies between the test statistics not taken into account
* Only valid under certain correlation assumptions \(“positive correlation” among the test statistics\)

![](../.gitbook/assets/image%20%2827%29.png)

#### generalizing - [propagation method](https://www.sciencedirect.com/science/article/pii/S1551714415300513?via%3Dihub)

#### 

### Alpha adjustment techniques \(for AND type\)

![](../.gitbook/assets/image%20%2883%29.png)

Based on this principle, the standard approach is to use an **unadjusted α** as nominal type I error for each individual hypothesis and to establish a hierarchy in the objectives to be able to increase the number of null hypothesis that can be rejected. The principle of the hierarchy is to test the first hypothesis. If the associated null hypothesis is rejected, the second hypothesis can be tested. If the associated null hypothesis is rejected, the 3rd hypothesis can be tested, etc.---建立层次结构的目标能够增加可拒绝的零假设数量。层次结构的原则是检验第一个假设。如果相关的原假设被拒绝，则可以检验第二个假设。如果相关的原假设被拒绝，则可以检验第三个假设，等等

The establishment of the hierarchy is based on clinical and statistical consideration.

> 例子：For instance a clinical trial involving 4 groups \(2 lots of the investigational product, an active control and a placebo\) aiming to show equivalence between 2 lots, non-inferiority of pooled lots versus an active control and superiority of pooled lots versus a placebo involved multiple hypotheses following the AND category. To maximize the number of null hypothesis rejected. Equivalence between lots would be tested first because this is the basis to allow pooling lots for the next comparison. Superiority to placebo would be tested second because it is higher power than testing non-inferiority to an active control and to provide credibility to testing non inferiority. Indeed if superiority cannot be demonstrated it means that the study has no ability to differentiate an inferior treatment from an active treatment and therefore results from a non-inferiority testing would be unreliable. The last objective tested in the hierarchy would be the non-inferiority of pooled lots versus the active control. 批次之间的等价性将首先进行测试，因为这是允许集中批次进行下一次比较的基础。接下来，检验与安慰剂相比的优越性将，因为它比主动对照的非劣效性检验具有更高的效力，并为非劣效性检验提供可信度。的确，如果不能证明优越性，就意味着这项研究没有能力区分较差的治疗和积极的治疗，因此，非劣效测试的结果将是不可靠的。在层次结构中测试的最后一个目标是混合抽签与主动对照的非劣效性。  
> 顺序：equivalence——superiority——non-inferiority

### Other approach to reduce multiplicity

The only other approach to reduce multiplicity is to simplify the objective/hypothesis. Below are few examples:

* Example 1: in a study involving 4 treatment groups, 1 dose of treatment A, 2 doses of treatment A, 3 doses of treatment A, a placebo, the effect of treatment A could be measured by testing the dose effect instead of comparing each dose to placebo.
* Example 2: in a study involving 2 groups \(treatment A and placebo\), aiming to show effect on multiple endpoints such as fatal cardiac arrest, stroke, arrhythmias, the primary endpoint could be defined as a composite endpoint involving the occurrence of any of these events.
* Example 3: in a study involving 2 groups \(treatment A and placebo\), aiming to show effect in different populations, the primary objective could be based on the combined populations.

## 3.3 Application to Interim analyses

### Definition

An interim analysis is any analysis intended to address a study objective\(s\) at any time prior to the formal completion of a trial.

Examination of data for cleaning or for monitoring the accumulation of the data is NOT an interim analysis.——注意：为清理或监测数据积累而对数据进行的检查不是一种期中分析。

### Advantages of Interim analyses

An interim analysis allows to kill bad products early

An interim analysis may allow early registration

### Error risk in interim analyses

However interim analyses involve multiplicity and thereby impacts on type I and II errors:

* **OR:** one will conclude that the study objective is reached either it met decision criterion at the interim analysis OR at the analyses foreseen at study completion. This type of interim analysis aims at concluding that the study objectives are reached earlier.——这种中期分析的目的是得出结论，即研究目标较早达成。
* **AND:** one will conclude that the study objective is reached because it met decision criterion at the interim analysis AND at the analyses foreseen at study completion. This type of interim analysis does not aims at concluding that the study objectives are reached earlier. This interim analysis is named interim analysis for futility.——这种中期分析的目的并不是要得出结论说，研究的目标是较早达成的。这种临时分析被称为期中无效分析。

#### ① Interim for success = OR

![](../.gitbook/assets/image%20%2872%29.png)

Main type I error adjustment

* Data increment  
  ——Group sequential = identical increment

  ——Alpha spending function = different increment

* Type I ——Pocock : identical for equal increment ——O’Brien-Fleming: between ——Peto: 0.1% for all interim

{% tabs %}
{% tab title="Introduction" %}
Since the data involved at the interim analysis is also planned to be part of subsequent analyses, the data correlation associated to the null hypotheses at interim and final analyses is known. This is why several statistical techniques have been developed to optimize the nominal alpha adjustment for such analyses. Like the Bonferroni adjustment, it is possible to adapt the nominal type I error of the interim and final analyses to control to overall type I error.——由于中期分析中涉及的数据也计划成为后续分析的一部分，因此中期和最终分析中与原假设相关的数据相关性是已知的。这就是为什么开发了几种统计技术来优化这种分析的名义阿尔法调整。就像Bonferroni调整一样，有可能调整中间和最终分析的名义类型I错误，以控制整个类型I错误。
{% endtab %}

{% tab title="Pocock method" %}
nominal type I errors for each analysis involving identical data increment \(eg first analysis involves N subjects, next one involves 2N subjects, next one involves 3N,…\) are identical
{% endtab %}

{% tab title="Peto method" %}
nominal type I errors for each interim analysis is set up to 0.1% so that the nominal type I error at final analysis is almost equal to α, the targeted type I error.
{% endtab %}

{% tab title="O’Brien-Fleming: " %}
This method is between the 2 previous methods in the way the nominal type I error is distributed. It is smaller at first interim analyses and increases with the next analyses.
{% endtab %}

{% tab title="Alpha spending functions" %}
This is a generalization of the above method involving other function determining the nominal type I error to use \(see slide below\). The functions represent the cumulative type I error used over the interim analyses. This approach allows adjusting the nominal type I error to analyses involving unequal data increments.--这是上述方法的推广，涉及到确定要使用的标称类型I错误的其他函数\(参见下面的幻灯片\)。这些函数表示在过渡分析期间使用的累积类型I错误。这种方法允许调整标称类型I的错误来分析不相等的数据增量。

![](../.gitbook/assets/image%20%283%29.png)
{% endtab %}
{% endtabs %}

#### Example 1：Group sequential = identical increment

![](../.gitbook/assets/image%20%281%29.png)

This example involves 3 interim analyses. The nominal p-value for each interim analysis is provided together with the nominal type I error allowing concluding that there is a treatment effect \(upper right table\).

The Pocock and O’Brien-Fleming methods allow concluding that there is a treatment effect at the second interim analysis. With Peto method, it is not possible to conclude until the 3 rd analysis.

#### Example 2：Group sequential = identical increment

![](../.gitbook/assets/image%20%2888%29.png)

This example involves also 3 interim analyses. The Pocock method does not allow concluding that there is a treatment effect. With Peto, O’Brien-Fleming methods it is possible to conclude at 3rd analysis

#### **Conclusions**：

* higher number of analyses leads to lower power
* A method with higher alpha spending like Pocock will allow concluding earlier but has less power.
* large early alpha increases chance to stop early but…  
  ——results may be less robust

  ——sample size may be too low to address other endpoints of interest

* Adjustment needed——Depending on the method selected, the clinical trial outcome may be different. The choice of the method can be seen itself as a multiplicity problem. As a consequence, analyses require pre-specified analysis plan with clear description of the primary method used to conclude on the study objectives.

#### ② Interim for failure/futility = AND

![](../.gitbook/assets/image%20%2887%29.png)

Yes if CI is below 1 at final——If observed GMC ratio is above the red curve, it is unlikely that this will happen. One can use this extra condition to limit cost in case of failure.

This extra condition will reduce power & type I error——alpha adjustment is not required but power will decrease with the number of interim

### Potential bias in interim analyses

#### ① Redefining the stopping boundary after having looked at the data

![](../.gitbook/assets/image%20%2882%29.png)

Yes for future way of spending a if it is ndependent from group difference observed at interim

![](../.gitbook/assets/image%20%2853%29.png)

If a sponsor has access to the interim results and decides to change the analysis strategy from scenario 1 to sceanrio 2 based on the interim results, the type I error is greater than 2.5%. Indeed the type I error for each analysis scenario is 2.5%. This type I error is a nominal type I error and the type I error is impacted by the ‘OR’ multplicity associated to the analysis scenari.——如果赞助者可以访问中期结果，并决定根据中期结果将场景1的分析策略更改为sceanrio 2，则类型I的错误大于2.5%。实际上，每个分析场景的类型I错误是2.5%。这种类型I错误是一种标称类型I错误，类型I错误受到与分析场景相关的“或”多重性的影响。

selecting among different strategies——need further adjustment for multiple strategies

#### ② Redefining the maximum sample size/information after having looked at the data

* Independent from group difference observed at interim =&gt; no penalty 
* data driven：O’Brien-Fleming rule, so interim p-value 0.02 decide to do final analysis shortly ——need further adjustment to control error

#### ③ Redefining the endpoint after having looked at the data

* Such change may be legitimate as all possible endpoint scenari are difficult to anticipate in advance and an unforeseen scenario may require a revision of the definition.  ——这种变化可能是合理的，因为所有可能的端点场景都很难提前预测，并且无法预见的场景可能需要修改定义。 ——前提：Independent from group difference observed at interim 
* However such a revision may also have been initiated as the sponsor observed a larger treatment effect with the revised definition. The latter is therefore a selection among different strategies thereby impacting the type I error. ——然而，由于主办者发现修订后的定义具有更大的治疗效果，因此这种修订也可能已经开始。因此，后者是对不同策略的选择，从而影响I型错误。 ——因此，need further adjustment for multiple endpoints

#### ④ Enrolment/follow-up profile change before versus after interim analysis!

* Such change is usual as centers are not enrolling in parallel at the same speed and centers are associated to patient profile. ——这种变化是常见的，因为中心不是以相同的速度并行注册的，中心与患者档案相关。 ——前提：Independent from group difference observed at interim ——或者说，sub-group specificity is unlikely 
* However such a change may be related to incentive from sponsor after having observed an beter response to treatment in the specific patient profile at interim analysis. The latter is therefore a selection among different strategies thereby impacting the type I error. ——然而，这种变化可能与赞助者的激励有关，因为在中期分析中，在特定的患者资料中观察到治疗效果更好。因此，后者是对不同策略的选择，从而影响I型错误。 ——possibility of sub-group specific results. Therefore, need adjustment for multiple subgroups

### Data Robustness：Interim data may not be representative of the final data

* over-representativity of drop-out ——Interim analysis including subjects with the primary outcome/endpoint may not be representative of the final data as dropped-out subjects, subjects providing outcome after a short follow-up will be over-represented.
* data quality & credibility of non-inferiority studies

  ——Interim analysis performed on unclean data, based on all subjects enrolled will tend to underestimate treatment effect.

* too limited for secondary endpoints \(eg safety, long term follow-up\)
* limited to few centers

A clear recommended is to perform an interim analysis on all subjects enrolled before a cut-off when all these subjects have completed their follow-up and data has been cleaned.

### Conclusions

* Interim analyses require special care to ensure error risks are controlled
* Attention to result dissemination \(threat for integrity of final results\)
* Attention to data quality/exhaustiveness

## 3.4 Application to Subgroup analyses

Sub-group analyses are frequent in the analysis of clinical trials. Because of the effort and cost involved in clinical trials, subgroups analyses are used to extract as much information as possible on the treatment effect. Such analyses, which assess the heterogeneity of treatment effects in subgroups of patients, may provide useful information for the care of patients and for future research. However, unless a strategy for controlling the Type I error associated to multiplicity in subgroup analysis has been set up, subgroup analyses lead to overstated and misleading results.——亚组分析在临床试验分析中经常出现。由于临床试验所涉及的努力和成本，亚组分析被用来提取尽可能多的关于治疗效果的信息。这些分析评估了患者亚组治疗效果的异质性，可能为患者的护理和未来的研究提供有用的信息。然而，除非已经建立了控制与子组分析中多重性相关的I型错误的策略，否则子组分析将导致夸大和误导的结果。

### Value of sub-group analysis for supporting an objective that has been reached

As indicated earlier, subgroup analyses are useful supportive analyses required by authorities. The sub-group should be pre-defined and these analysis support that the treatment effect seen in a clinical trial is not driven by a specific subgroup of subjects.——如前所述，亚组分析是当局需要的有用的支持性分析。应该预先定义亚组，这些分析支持在临床试验中看到的治疗效果不是由特定的受试者亚组驱动的。

<table>
  <thead>
    <tr>
      <th style="text-align:left">type</th>
      <th style="text-align:left">description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><a href="https://www.clinicaltrials.gov/ct2/show/NCT00480025?term=109493&amp;rank=1">Confirmatory</a>
      </td>
      <td style="text-align:left">sub-group analysis should be pre-planned with adequate procedure for controlling
        type I error</td>
    </tr>
    <tr>
      <td style="text-align:left">Exploratory</td>
      <td style="text-align:left">
        <p>Analysis on whole group failed: subgroup finding must be confirmed in
          either a new trial and all other similar trials (see meta-analysis)</p>
        <p></p>
        <p>Analysis on whole group succeeded: subgroup analysis allow to <b>investigate </b>whether
          the effect observed on the whole group is consistent and not driven by
          a <b>pre-defined subgroup</b>.</p>
        <p>
          <img src="../.gitbook/assets/image (71).png" alt/>
        </p>
        <p>In this case, claim on efficacy should be limited to Node positive subjects
          since there was no measurable effect in patient with Node negative.</p>
      </td>
    </tr>
  </tbody>
</table>









