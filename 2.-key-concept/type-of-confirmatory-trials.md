# Chapter 2: Type of confirmatory trials

As described in section 2.5 in Part I, one of the typology to categorize clinical trials, consists in dissociating “Exploratory” from “Confirmatory” trials:

<table>
  <thead>
    <tr>
      <th style="text-align:left">Trials</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Exploratory Trial</td>
      <td style="text-align:left">
        <p>Clear and precise objectives BUT:</p>
        <p>&#x2022; Not always lead to simple test of predefined hypothesis</p>
        <p>&#x2022; They could require a more flexible approach (multiple end-points,
          changes in the analyses, etc.)</p>
        <p>&#x2022; Cannot be the basis of the formal proof of efficacy (but can
          contribute&#x2026;)</p>
        <p>&#x2022; They provide the basis to define the Hypothesis for Confirmatory
          Trials</p>
        <p>&#x2022; Multiple objectives</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Confirmatory trial</td>
      <td style="text-align:left">
        <p>Adequately controlled trial with a prespecified precise hypothesis:</p>
        <p>&#x2022; To provide EVIDENCE of efficacy or safety</p>
        <p>&#x2022; A limited number of questions</p>
        <p>&#x2022; One Primary Objective and a limited number of secondary objectives</p>
        <p>&#x2022; Highly standardized</p>
        <p>&#x2022; Variables of assessment should be pre-defined, sensitive, accepted,
          and limited in number (one primary variable)</p>
        <p>&#x2022; Sample size (n subjects) should be pre-defined and justified</p>
      </td>
    </tr>
  </tbody>
</table>In a confirmatory trial itself, there are both confirmatory objectives \(i.e., objectives associated to a hypothesis to be confirmed\) and exploratory objectives \(i.e., objectives aiming at describing endpoints/data, generating new ideas to confirm\).

## 2.1 Introduction

### What is a confirmatory trial?

An adequately controlled trial in which the study objective aims to confirm pre-specified hypotheses .

Confirmatory trials are intended to provide firm evidence in support of claims. Accordingly statistical methods are used to ensure that the risk of erroneously concluding is strictly controlled to be low an acceptable level \(usually 2.5%\)

Characteristics:

* A limited number of hypotheses to confirm
* Clear decision criteria
* Driving the sample size \(n subjects\)

### What is an exploratory trial?

A trial without hypothesis to confirm. The objectives entail data exploration. Tests of hypothesis may be carried out, but the choice of hypothesis may be data dependent.

Characteristics:

* Such trials cannot be the basis to prove efficacy
* Most confirmatory trials have also exploratory analyses suggesting hypotheses for later research.
* The protocol should make a clear distinction between confirmatory and exploratory objectives/analyses

### How to provide firm evidence for a confirmatory objective?

1. to define an endpoint ie the parameter measured
2. to formulate the hypotheses
3. to define the risk of errors
4. To define the decision criteria
5. To determine how endpoints are used to estimate the parameter of interest\(= estimand\)

### Endpoints

<table>
  <thead>
    <tr>
      <th style="text-align:left">type</th>
      <th style="text-align:left">description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">endpoint</td>
      <td style="text-align:left">
        <p>An endpoint or outcome measure is a measurement performed on each participant
          during the study to answer the study objectives.</p>
        <p></p>
        <p>&#x2022; Clear and specific definition of the endpoints in the protocol
          is critical to ensure the right information is collected during the study.</p>
        <p>&#x2022; Selection of the methods of outcome assessment should be accurate
          and certainly free of bias.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">clinical endpoint</td>
      <td style="text-align:left">
        <p>A clinical endpoint is a characteristic or variable that reflects how
          a patient feels, functions, or survives.</p>
        <p>
          <br />Type of variables:</p>
        <p>&#x2022; Quantitative--Laboratory variables, physiological measurements
          (blood pressure, body weight, &#x2026;), count of events (number fo episodes
          of a disease)</p>
        <p>&#x2022; Categorised--(ordered): rating scale, scores (symptoms: absent,
          mild, moderate, severe)</p>
        <p>&#x2022; Dichotomous--(binary): categorised variable with two classes
          (1/0, Yes/No, Presence/absence) only</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">surrogate endpoint</td>
      <td style="text-align:left">
        <p>A surrogate endpoint is an endpoint intended to substitute for a clinical
          endpoint.</p>
        <p></p>
        <p>&#x2022; A surrogate endpoint should be related to the clinical endpoint
          by mechanism of action or in the common disease/mechanism pathway.</p>
        <p>&#x2022; Must be validated based on reproducibility and clinical credibility.</p>
      </td>
    </tr>
  </tbody>
</table>Reasons for using surrogate endpoints:

* Less expensive
* Easier to measure
* Occur soon after the intervention in the disease process

A surrogate endpoint may not be of direct practical importance to the patient. A given disease process may have multiple markers that could be used as the surrogate endpoint. Or, more than one could be used.

![Examples](../.gitbook/assets/image%20%2869%29.png)

## 2.2 Reminder on Hypothesis Testing

![](../.gitbook/assets/image%20%2857%29.png)

The study is considered a success if we can reject Ho or we conclude Ha

The authorities want to control the Type I error: probability to say the study is a success when the product is not good.

The sponsor wants to minimize the type II error: probability not to be able to reject Ho while actually the product is good.

> Note that the type II error depends on a specific value of the parameter of interest within the Ha space, while the type I error is to be controlled below a given value for all values of parameter of interest belonging to H0. 请注意，第二类错误取决于备择假设空间中目标参数的特定值，而第一类错误则控制在属于零假设的所有目标参数值的给定值之下。因为我们要绝对控制I型错误，尽量最小化II型错误
>
> **Importantly, a clinical trial can only conclude with proper control of that the conclusion is wrong when H0 can be rejected. When H0 cannot be rejected, it is not correct to conclude that H0 is true with a risk or error below alpha as it might just be linked to a lack of power.  重要的是，临床试验只有在正确控制H0可被拒绝的情况下才能得出结论。当H0不能被拒绝时，就不能断定H0是正确的，风险或错误低于alpha值，因为它可能只是与缺乏动力有关。**

### decision criterion 1：based on a range of observed value of the estimated parameter

![type I error](../.gitbook/assets/image%20%2877%29.png)

Under the assumption that RR=1, the distribution of log\(RR\) is approximately normally distributed with 0 as mean. One can therefore define a range of value RR&gt;X so that the probability to have RR&gt;X when RR=1 is equal to α, type I error.

Note that for RR &lt; 1, the distribution curve will switch to the left and therefore the probability to have RR&gt; x is less than alpha for any true value of RR &lt; 1. The type I error is therefore well controlled to be below α

![Type II error](../.gitbook/assets/image%20%2844%29.png)

The type II error when RR=Y is the probability to observe RR&lt;=X when the true RR=Y. The power, when the true relative risk RR=Y, is the probability to observe RR&gt;x when RR=Y.

It is easy to understand how the power increases with the sample size. Indeed with an increased sample size, the distribution curve narrows on the X axis and therefore β decreases as the width of bell curve reduces and the critical x value shifts to the left.--随着样本量的增加，随着钟形曲线宽度的减小，临界X值向左移动，分布曲线在X轴上变窄。

### decision criterion 2：based on p-value

![one sided p-value](../.gitbook/assets/image%20%2826%29.png)

P-value is defined as the maximum probability to observe a value further distant from H0 than the observed value for true RR belonging to H0. In the above example, it is the probability that

                                                        $$p\ - value= Pr(\widetilde{RR} \geq \widetilde{rr}_{obs} | H_0)$$ 

It is easy to see that this decision criterion will lead to the same conclusion as the decision criterion based on a range of observed $$\widetilde{RR}$$ : if the $$Pr(\widetilde{RR} \geq \widetilde{RR}_{obs} | H_0)$$ is higher than α, the $$\widetilde{RR}_{obs}$$ is on the left side of the critical x value.

![2 sided-p-value](../.gitbook/assets/image%20%2813%29.png)

### decision criterion 3：based on confidence interval for the observed estimated parameter

A confidence interval \(CI\) is an observed interval, calculated from the observations and therefore varying from one observation to another. It has the property to include the parameter of interest with a probability equals to the confidence level

![](../.gitbook/assets/image%20%2829%29.png)

With the above example looking at the relative risk, a 95% CI for RR will cover the true value of the relative risk in 95% of the cases.

Confidence intervals are usually built with equal tails i.e. the probability that the CI is above the true RR is equal to the probability that the CI is below the true RR i.e. α/2 --置信区间通常具有相等的尾，即CI高于真实RR的概率等于CI低于真实RR的概率

Based on this principle, the lower limit of the \(1-2α\) CI of RR when $$\widetilde{RR}_{obs} =x$$ \(\(x being the threshold for decision criterion\) or when the one sided p-value = α the threshold will be equal to 1.

Accordingly a decision based on the \(1-2α\) CI being fully outside of the null hypothesis parameter space allows to control the type I error for a one sided test below α。换句话说，\(1-2α\) CI has a% to be above and below the true parameter.

> Note that if the CI has not equal tails, a one sided test based on CI will not necessarily control the type I error.

## 2.3 [Superiority/non-inferiority/difference/equivalence](https://zhuanlan.zhihu.com/p/26588986)

![](../.gitbook/assets/image%20%2814%29.png)

### Superiority\(one sided\)

In a superiority objective, the null hypothesis contains and is bounded by the identity between groups. 

![](../.gitbook/assets/image%20%2870%29.png)

{% hint style="danger" %}
The null hypothesis parameter space stops when groups are identical.

Warning: Superiority does not necessarily have clinical relevance.
{% endhint %}

### Clinical/Substantial Superiority

In a substantial superiority objective, the null hypothesis contains the identity between groups and is bounded by a value different from the identity between groups.

![](../.gitbook/assets/image%20%2890%29.png)

{% hint style="danger" %}
The null hypothesis parameter space stops when groups are identical.

Warning: Superiority does not necessarily have clinical relevance.
{% endhint %}

### Non-inferiority\(one sided\)

In a non-inferiority objective the identity between groups is excluded from the null hypothesis. In other words, it aims to demonstrate that the investigational product is not worse than the control by more than a pre-specified \(small\) amount.--在非劣效性目标中，组间的同一性被排除在原假设之外。换句话说，它的目的是证明研究的产品不会比对照组差超过预先指定的\(小\)量。

![](../.gitbook/assets/image%20%2850%29.png)

The two main reasons of using non-inferiority trials are:

1. Allow bringing on the market another medicine to ensure enough supply. This will typically happen with products used in large volume and, even more important, if interruption of the supply might impact public health \(e.g., vaccines\)
2. Allow bring on the market a treatment of same efficacy \(primary objective\) and presenting another benefit: Fewer side effect, Less invasive treatment administration, less costly, ….

### Difference\(two sided\)

![](../.gitbook/assets/image%20%2893%29.png)

{% hint style="danger" %}
The null hypothesis parameter space is ‘groups are identical’.

Warning: Difference does not have necessarily clinical relevance.
{% endhint %}

### Equivalence\(two sided\)

![](../.gitbook/assets/image%20%2833%29.png)

{% hint style="danger" %}
The null hypothesis parameter space excludes ‘groups are identical’ and is bounded on two sides.

Warning: Requires the definition of the margins based on clinical relevance.
{% endhint %}

### How to define Clinical Margin?

Non-inferiority and substantial superiority require defining a margin based on **statistical reasoning and clinical judgment**. Its specification is not an easy exercise but essential and one of the necessary elements to estimate the sample size. 

The clinical margin for non-inferiority should be smaller than the treatment effect against placebo.

Example: Efficacy over placebo led to CI for difference in % of responders between 80% & 100% =&gt; non inferiority margin could be 20%

> In a non-inferiority setting, too high margin increases the risk of bringing to market an inferior product while lower and more conservative margins requires larger sample size making the development challenging. --在非劣效环境中，过高的margin会增加将劣质产品推向市场的风险，而较低和较保守的margin则需要更大的样本量，这使得开发具有挑战性。

## 2.4 Considerations in superiority/difference and non-inferiority/equivalence trials

### Impact of compliance

Compliance & study quality impact differently when testing superiority or when testing non inferiority

Example:

* Reference response rate for placebo = 10%
* Reference response rate for active = 60%
* Non inferiority margin = 10% \(ie RH 0 at worse if response rate for active = 50% under full compliance\)
* Problem: If some subjects do not take the active product, the response rate under the active product will be lower than 60%

### Impact on population

According to [ICH E9](https://www.ema.europa.eu/en/documents/scientific-guideline/ich-e-9-statistical-principles-clinical-trials-step-5_en.pdf) and the[ CHMP](https://www.ema.europa.eu/en/documents/scientific-guideline/guideline-choice-non-inferiority-margin_en.pdf) , **the primary population for superiority should be the full population** without excluding enrolled patient such as poor compliers because

1. Exclusion may create bias in favor of one treatment group thereby compromising the randomization aiming to ensure comparable population is enrolled in all study groups.
2. Non-compliance would reduce the treatment difference. Therefore if superiority can be concluded one knows that superiority would have been concluded with subjects 100% compliant.

On the other hand, the population to consider for non-inferiority is both

1. The full population without excluding enrolled patient such as poor compliers because Exclusion may create bias in favor of one treatment group thereby compromising the randomization aiming to ensure comparable population is enrolled in all study groups.
2. The per-protocol cohort \(i.e. the population that complies with treatment\) as this is the population that allows to maximize treatment difference if this exists. The per-protocol cohort is usually considered for the primary analysis.

### Impact on sample size--Different hypothesis tests require different sample size!

![](../.gitbook/assets/image%20%2832%29.png)

Conclusion of the example:

1. Superiority to placebo is the less expensive in sample size
2. Superiority to active control is the most expensive
3. Ethic, feasibility & cost must be accounted in the choice of the design

